---
description: Dynamic Chat-Versionshinweise – Marketo-Dokumente – Produktdokumentation
title: Versionshinweise zu Dynamic Chat
feature: Release Information, Dynamic Chat
hide: true
hidefromtoc: true
exl-id: 0a7e5cc9-f2a6-4721-bbdc-661249a2e2b6
source-git-commit: 5dbc3add8acaae02f25c1f9b9ae39ecfc1aaf259
workflow-type: tm+mt
source-wordcount: '900'
ht-degree: 3%

---

# Versionshinweise zu Dynamic Chat {#dynamic-chat-release}

Adobe Dynamic Chat-Versionen basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren Ansatz für die Bereitstellung von Funktionen ermöglicht. Manchmal gibt es mehrere Versionen in einem Monat, daher schauen Sie regelmäßig nach den aktuellsten Informationen.

Die Seite mit den standardmäßigen Versionshinweisen für Marketo Engage [finden Sie hier](/help/marketo/release-notes/current.md){target="_blank"}.

## Version Juni 2025 {#june-2025-release}

### Überarbeitung der Routing-Logik {#routing-logic-revamp}

Die Live-Chat-Routing-Logik in Dynamic Chat wurde überarbeitet, um ein intelligenteres und vorhersehbareres Interaktionsverhalten über alle Routing-Typen (Account, Custom, Team und Round Robin) hinweg sicherzustellen. Die neue Logik vereinfacht Routing-Flüsse und verbessert die Fallback-Handhabung, wenn Agenten nicht verfügbar sind.

#### Wichtige Verbesserungen im Routing-Verhalten

* **Bis zu zwei Interaktionsversuche pro Sitzung**

   * Das System versucht, eine Verbindung mit bis zu zwei Agenten herzustellen (höchstens), jedoch ausschließlich innerhalb der primären Routingregel.

   * Wenn ein Agent verfügbar ist, aber nicht reagiert (z. B. den Chat ablehnt oder verpasst), versucht das System, eine Verbindung zu einem anderen Agenten aus demselben Pool herzustellen.

   * Fallback-Logik (wie Round Robin) wird nur aktiviert, wenn während der ersten Auflösung keine geeigneten Agenten gefunden werden, nicht erneut versuchen nach einer fehlgeschlagenen Interaktion.

* **Routingregelspezifisches Verhalten**

_&#x200B;**Konto-Routing**&#x200B;_

Wenn die E-Mail-Domain eines Besuchers einem bekannten Konto zugeordnet ist, wird der zugeordnete Agent immer priorisiert.

Wenn der Agent verfügbar ist, wird der Chat direkt an ihn weitergeleitet.

Wenn der Agent nicht verfügbar ist, führt das System Folgendes aus:

* Versucht keinen anderen Agenten, auch wenn Round Robin als Ausweichlösung aktiviert ist.

* Stattdessen gilt Folgendes:

   * Zeigt den Besprechungskalender des zugeordneten Agenten an (falls aktiviert),
&#x200B;- oder -
   * Kehrt zu einer Standardmeldung zurück (im schlimmsten Fall).

Die Routing-Regel auf Kartenebene (z. B. Team, Benutzerdefiniert) wird nur berücksichtigt, wenn das Konto-Routing nicht zulässig ist (keine übereinstimmende Domain oder Agent).

_&#x200B;**Benutzerdefiniertes/Team-Routing**&#x200B;_

Diese Regeln können mehrere geeignete Agenten zurückgeben.

Wenn der erste verfügbare Agent nicht interagiert, versucht das System einen weiteren Agenten aus derselben Liste.

Ein Round-Robin-Fallback wird nicht ausgelöst, nur weil ein Agent nicht reagiert.

Wenn keiner der Agenten eingreift:

* Das System zeigt den Kalender des ersten Agenten an (falls aktiviert).
&#x200B;- oder -
* Zeigt die standardmäßige Fallback-Nachricht an.

_&#x200B;**Round Robin-Routing**&#x200B;_

Bei Verwendung als primäre Routingregel führt das System Folgendes durch:

* Versucht, den ersten verfügbaren Agenten aus dem Round-Robin-Pool zu kontaktieren.

* Wenn der erste Agent nicht antwortet, versucht er es erneut mit dem nächstbesten geeigneten Agenten.

Wenn Round Robin als Fallback verwendet wird, wird er nur aktiviert, wenn keine Agenten von der primären Regel aufgelöst werden.

_&#x200B;**Besuchererlebnis-Fluss**&#x200B;_

Das System prüft, ob Konto-Routing anwendbar ist.

* Wenn ja und der Agent verfügbar ist, wird sofort eine Verbindung hergestellt.

* Wenn der Agent nicht geeignet oder nicht verfügbar ist, fährt er mit der Routing-Regel auf Kartenebene fort.

Routingregel auf Kartenebene (benutzerdefiniert, Team, Round Robin) wird ausgewertet.

* Berechtigte Agenten werden auf Verfügbarkeit geprüft (Berechtigungen, Status).

* Das System greift auf einen Agenten zu und versucht bei Bedarf einen zweiten Agenten aus derselben Regel.

* Wenn keine Interaktion erfolgreich ist, wird eine Ausweichlogik angewendet:

   * Kalender-Fallback (falls aktiviert),
&#x200B;- oder -
   * Standardnachricht.

Ein Round-Robin-Fallback wird nur berücksichtigt, wenn keine geeigneten Agenten aus der primären Routing-Regel gefunden werden, nicht, wenn einzelne Agenten nicht reagieren.

##### Anwendungsfälle {#use-cases}

_&#x200B;**Konto-Routing**&#x200B;_

<table><thead>
  <tr>
    <th>Typ</th>
    <th>Beispiel</th>
    <th>Ergebnis</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>Die Domain des Besuchers wird einem Konto zugeordnet. Für den zugeordneten Agenten ist der Live-Chat aktiviert und verfügbar</td>
    <td>Der Chat stellt eine direkte Verbindung zum zugeordneten Agenten her</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>Zugeordneter Agent ist nicht verfügbar, Round Robin Fallback ist aktiviert</td>
    <td>System wählt einen verfügbaren Agenten über Round Robin aus und bindet ihn ein </td>
  </tr>
  <tr>
    <td>Kein Fallback-Agent</td>
    <td>Zugeordneter Agent ist nicht verfügbar, kein Round Robin Fallback; Besprechungsbuchung ist aktiviert</td>
    <td>Das System zeigt den Kalender des zugeordneten Agenten an oder zeigt eine standardmäßige Ausweichmeldung an.</td>
  </tr>
</tbody></table>

_&#x200B;**Benutzerdefiniertes Routing**&#x200B;_

<table><thead>
  <tr>
    <th>Typ</th>
    <th>Beispiel</th>
    <th>Ergebnis</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>Benutzerdefinierte Logik löst eine Liste von Agenten auf. Der erste Agent ist verfügbar und akzeptiert Chat.</td>
    <td>Chat stellt eine Verbindung zum ersten Agenten her.</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>Benutzerdefinierte Regel löst keine Agenten auf, Round Robin Fallback ist aktiviert.</td>
    <td>Das System wählt einen verfügbaren Agenten über Round Robin aus und bindet ihn ein.</td>
  </tr>
  <tr>
    <td>Kein Fallback-Agent</td>
    <td>Zwei Agenten wurden aufgelöst. Keiner akzeptiert Chat, Fallback wird auf den Besprechungskalender festgelegt.</td>
    <td>Der Kalender des zuerst getesteten Agenten wird angezeigt oder es wird eine standardmäßige Fallback-Nachricht angezeigt.</td>
  </tr>
</tbody></table>

_&#x200B;**Team-Routing**&#x200B;_

<table><thead>
  <tr>
    <th>Typ</th>
    <th>Beispiel</th>
    <th>Ergebnis</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>Das Team umfasst Agenten mit Live-Chat. Der erste verfügbare Agent akzeptiert den Chat.</td>
    <td>Chat stellt eine Verbindung zu diesem Agenten her.</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>Es ist kein Team-Agent verfügbar und Round Robin Fallback ist aktiviert.</td>
    <td>Das System wählt einen Agenten aus dem Round Robin Pool aus und stellt eine Verbindung mit ihm her.</td>
  </tr>
  <tr>
    <td>Kein Fallback-Agent</td>
    <td>Zwei Agenten verfügbar, aber keiner von beiden ist eingebunden; Kalenderfallback aktiviert.</td>
    <td>Der Kalender des zuerst getesteten Agenten wird angezeigt oder es wird eine Fallback-Nachricht ausgelöst.</td>
  </tr>
</tbody></table>

_&#x200B;**Round Robin-Routing**&#x200B;_

<table><thead>
  <tr>
    <th>Typ</th>
    <th>Beispiel</th>
    <th>Ergebnis</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>Round Robin Pool hat mehrere Agenten; zweiter Agent nimmt Chat an, nachdem der erste nicht.</td>
    <td>Chat stellt eine Verbindung zum zweiten Agenten her.</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>Im Round Robin Pool sind keine Agenten verfügbar. Der Besprechungskalender ist aktiviert.</td>
    <td>Der Kalender wird für den ersten Agenten in der Liste angezeigt (falls konfiguriert), oder es wird eine Fallback-Nachricht angezeigt.</td>
  </tr>
  <tr>
    <td>Kein Fallback-Agent</td>
    <td>Keine verfügbaren Agenten; Fallback ist deaktiviert.</td>
    <td>Dem Besucher wird eine statische Fallback-Nachricht angezeigt.</td>
  </tr>
</tbody></table>

### Impuls-Benachrichtigung {#pulse-notification}

Wenn ein Besucher die Verbindung zu einem Agenten anfordert, stellen wir dem Agenten eine In-App-Browser-Benachrichtigung zur Verfügung. Aber manchmal verpassen Agenten diese Chats.

Mit dieser Version kann der Live-Agent eine E-Mail-, Slack-, In-App- und Browser-Benachrichtigung erhalten, wenn ein neuer Besucher am Chat interessiert ist.

1. Klicken Sie auf Ihrer Adobe Experience Cloud-Homepage auf das Kontosymbol und wählen Sie **Voreinstellungen** aus.

   ![](assets/dynamic-chat-june-2025-release-1.png)

1. Scrollen Sie nach unten zu _Benachrichtigungen_ und wählen Sie die gewünschten Dynamic Chat aus.

   ![](assets/dynamic-chat-june-2025-release-2.png)

>[!NOTE]
>
>Der Inhalt einer Pulse-Benachrichtigung kann mit dem identisch sein, den wir für In-App- und Browser-Benachrichtigungen verwenden.
