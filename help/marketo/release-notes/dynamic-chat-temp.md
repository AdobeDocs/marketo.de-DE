---
description: Dynamic Chat-Versionshinweise – Marketo-Dokumente – Produktdokumentation
title: Dynamic Chat-Versionshinweise
feature: Release Information, Dynamic Chat
hide: true
hidefromtoc: true
exl-id: 0a7e5cc9-f2a6-4721-bbdc-661249a2e2b6
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 68%

---

# Dynamic Chat-Versionshinweise {#dynamic-chat-release}

Die Versionen von Adobe Dynamic Chat basieren auf einem Modell der kontinuierlichen Bereitstellung, das einen besser skalierbaren Ansatz für die Bereitstellung von Funktionen ermöglicht. Manchmal gibt es mehrere Versionen in einem Monat, schauen Sie daher regelmäßig nach den aktuellsten Informationen.

Die Standardseite mit den Versionshinweisen für Marketo Engage [finden Sie hier](/help/marketo/release-notes/current.md){target="_blank"}.

## Version Juni 2025 {#june-2025-release}

### Überarbeitung der Routing-Logik {#routing-logic-revamp}

Die Routing-Logik des Live-Chats in Dynamic Chat wurde überarbeitet, um über alle Routing-Typen hinweg (Konto, benutzerdefiniert, Team und Round Robin) für ein intelligenteres und besser vorhersehbares Interaktionsverhalten zu sorgen. Die neue Logik vereinfacht Routing-Abläufe und verbessert Ausweichmöglichkeiten, wenn keine Agentinnen oder Agenten verfügbar sind.

#### Wichtige Verbesserungen im Routing-Verhalten

* **Bis zu zwei Interaktionsversuche pro Sitzung**

   * Das System versucht, eine Verbindung mit bis zu zwei Agenten herzustellen (höchstens), jedoch ausschließlich innerhalb der primären Routingregel.

   * Wenn ein Agent verfügbar ist, aber nicht reagiert (z. B. den Chat ablehnt oder verpasst), versucht das System, eine Verbindung zu einem anderen Agenten aus demselben Pool herzustellen.

   * Die Ausweichlogik (wie etwa Round Robin) wird nur aktiviert, wenn bei der ersten Auflösung keine geeigneten Agentinnen oder Agenten gefunden werden, jedoch nicht für ein erneutes Versuchen nach einer fehlgeschlagenen Interaktion.

* **Spezifisches Verhalten für eine Routing-Regel**

_**Konto-Routing**_

Wenn die E-Mail-Domain einer Besucherin oder eines Besuchers einem bekannten Konto zugeordnet ist, wird die als Agentin bzw. Agent zugeordnete Person immer priorisiert.

Wenn diese Person verfügbar ist, wird der Chat direkt an sie weitergeleitet.

Wenn sie nicht verfügbar ist, tut das System Folgendes:

* Es versucht nicht, eine andere Person als Agentin bzw. Agenten zu erreichen, auch wenn Round Robin als Ausweichlösung aktiviert ist.

Stattdessen gilt Folgendes:

* Zeigt den Besprechungskalender des zugeordneten Agenten an (falls aktiviert) oder:
* Kehrt zu einer Standardmeldung zurück (im schlimmsten Fall).

Die Routing-Regel auf Kartenebene (z. B. Team, Benutzerdefiniert) wird nur berücksichtigt, wenn das Konto-Routing nicht zulässig ist (keine übereinstimmende Domain oder Agent).

_**Benutzerdefiniertes/Team-Routing**_

Diese Regeln können mehrere geeignete Agentinnen oder Agenten zurückgeben.

Wenn der erste verfügbare Agent nicht interagiert, versucht das System einen weiteren Agenten aus derselben Liste.

Nur weil eine Person nicht reagiert, wird nicht gleich ein Round-Robin-Fallback ausgelöst.

Wenn sich keine Agentin bzw. kein Agent meldet, passiert Folgendes:

* Das System zeigt den Kalender der ersten Person an, die als Agentin bzw. Agent angefragt wurde (falls aktiviert).
– oder –
* Es zeigt die standardmäßige Fallback-Nachricht an.

_**Round-Robin-Routing**_

Bei Verwendung als primäre Routing-Regel führt das System Folgendes durch:

* Es versucht, die erste als Agentin bzw. Agent verfügbare Person aus dem Round-Robin-Pool zu kontaktieren.

* Wenn die erste Person nicht antwortet, erfolgt ein erneuter Versuch mit der am nächstbesten geeigneten Person.

Wenn Round Robin als Fallback verwendet wird, wird es nur aktiviert, wenn von der primären Regel keine Agentinnen oder Agenten aufgelöst werden.

_**Besuchererlebnis-Fluss**_

Das System prüft, ob Konto-Routing anwendbar ist.

* Falls ja und wenn eine Agentin oder ein Agent verfügbar ist, wird sofort eine Verbindung hergestellt.

* Wenn die Person nicht geeignet oder nicht verfügbar ist, wird mit der Routing-Regel auf Kartenebene fortgefahren.

Routingregel auf Kartenebene (benutzerdefiniert, Team, Round Robin) wurden ausgewertet.

* Geeignete Agentinnen und Agenten werden auf Verfügbarkeit geprüft (Berechtigungen, Status).

* Das System greift auf einen Agenten zu und versucht bei Bedarf einen zweiten Agenten aus derselben Regel.

* Wenn keine Interaktion erfolgreich ist, wird die Ausweichlogik angewendet:

   * Kalender-Fallback (falls aktiviert),
– oder –
   * Standardnachricht.

Round Robin wird als Ausweichlösung nur dann in Betracht gezogen, wenn keine geeigneten Agentinnen oder Agenten gemäß der primären Routing-Regel gefunden werden, aber nicht, wenn einzelne Agentinnen bzw. Agenten nicht reagieren.

##### Anwendungsszenarien {#use-cases}

_**Konto-Routing**_

<table><thead>
  <tr>
    <th>Typ</th>
    <th>Beispiel</th>
    <th>Ergebnis</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>Die Domain der Besucherin bzw. des Besuchers wird einem Konto zugeordnet. Für die als Agentin bzw. Agent zugeordnete Person ist der Live-Chat aktiviert und verfügbar.</td>
    <td>Der Chat stellt eine direkte Verbindung zur als Agentin bzw. Agent zugeordneten Person her.</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>Die als Agentin bzw. Agent zugeordnete Person ist nicht verfügbar, Round-Robin-Fallback ist aktiviert.</td>
    <td>Das System wählt einen verfügbaren Agenten über Round Robin aus und bindet ihn ein </td>
  </tr>
  <tr>
    <td>Keine Fallback-Agentin bzw. kein Fallback-Agent</td>
    <td>Die als Agentin bzw. Agent zugeordnete Person ist nicht verfügbar, kein Round-Robin-Fallback; Meeting-Buchung ist aktiviert.</td>
    <td>Das System zeigt den Kalender eines zugeordneten Agenten an oder zeigt eine standardmäßige Ausweichmeldung an</td>
  </tr>
</tbody></table>

_**Benutzerdefiniertes Routing**_

<table><thead>
  <tr>
    <th>Typ</th>
    <th>Beispiel</th>
    <th>Ergebnis</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>Benutzerdefinierte Logik löst eine Liste von Agentinnen und Agenten auf. Die erste Person ist verfügbar und akzeptiert den Chat.</td>
    <td>Chat stellt eine Verbindung zur ersten Agentin bzw. zum ersten Agenten her.</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>Benutzerdefinierte Regel löst keine Agenten auf. Round Robin Fallback ist aktiviert.</td>
    <td>Das System wählt über Round Robin einen verfügbaren Agenten aus und bindet ihn ein.</td>
  </tr>
  <tr>
    <td>Keine Fallback-Agentin bzw. kein Fallback-Agent</td>
    <td>Zwei Agentinnen bzw. Agenten wurden aufgelöst. Keine der beiden Personen akzeptiert den Chat; Fallback wird auf den Meeting-Kalender festgelegt.</td>
    <td>Zuerst versucht, den Kalender des Agenten anzuzeigen, oder die Standardfallback-Nachricht wird angezeigt.</td>
  </tr>
</tbody></table>

_**Team-Routing**_

<table><thead>
  <tr>
    <th>Typ</th>
    <th>Beispiel</th>
    <th>Ergebnis</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>Das Team umfasst Agentinnen und Agenten mit Live-Chat. Die erste verfügbare Person akzeptiert den Chat.</td>
    <td>Chat stellt eine Verbindung zu dieser Agentin bzw. diesem Agenten her.</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>Es ist keine Team-Agentin bzw. kein Team-Agent verfügbar und Round-Robin-Fallback ist aktiviert.</td>
    <td>Das System wählt einen Agenten aus dem Round-Robin-Pool aus und stellt eine Verbindung mit ihm her.</td>
  </tr>
  <tr>
    <td>Keine Fallback-Agentin bzw. kein Fallback-Agent</td>
    <td>Zwei Agentinnen bzw. Agenten verfügbar, aber keine der beiden Personen reagiert; Kalender-Fallback aktiviert.</td>
    <td>Zuerst versucht, den Kalender des Agenten anzuzeigen oder eine Ausweichmeldung auszulösen.</td>
  </tr>
</tbody></table>

_**Round-Robin-Routing**_

<table><thead>
  <tr>
    <th>Typ</th>
    <th>Beispiel</th>
    <th>Ergebnis</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>Round Robin Pool hat mehrere Agenten; der zweite Agent nimmt Chat an, nachdem der erste nicht.</td>
    <td>Chat stellt eine Verbindung zu einem zweiten Agenten her.</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>Im Round-Robin-Pool sind keine Agentinnen und Agenten verfügbar. Der Meeting-Kalender ist aktiviert.</td>
    <td>Der Kalender wird für den ersten Agenten in der Liste angezeigt (falls konfiguriert) oder die Fallback-Nachricht wird angezeigt.</td>
  </tr>
  <tr>
    <td>Keine Fallback-Agentin bzw. kein Fallback-Agent</td>
    <td>Keine verfügbaren Agentinnen und Agenten; Fallback ist deaktiviert.</td>
    <td>Dem Besucher wird eine statische Fallback-Nachricht angezeigt.</td>
  </tr>
</tbody></table>

### Pulse-Benachrichtigung {#pulse-notification}

Wenn ein Besucher die Verbindung zu einem Agenten anfordert, stellen wir ihm eine In-App-Browser-Benachrichtigung zur Verfügung. Manchmal verpassen Agentinnen und Agenten diese Chats jedoch.

Mit dieser Version kann die Live-Agentin bzw. der Live-Agent eine E-Mail-, Slack-, In-App- und Browser-Benachrichtigung erhalten, wenn eine neue Besucherin bzw. ein neuer Besucher am Chat interessiert ist.

1. Klicken Sie auf Ihrer Adobe Experience Cloud-Homepage auf das Kontosymbol und wählen Sie **Einstellungen** aus.

   ![](assets/dynamic-chat-june-2025-release-1.png)

1. Scrollen Sie nach unten zu _Benachrichtigungen_ und treffen Sie die gewünschten Dynamic Chat-Auswahlen.

   ![](assets/dynamic-chat-june-2025-release-2.png)

>[!NOTE]
>
>Der Inhalt einer Pulse-Benachrichtigung kann mit dem identisch sein, den wir für In-App- und Browser-Benachrichtigungen verwenden.
