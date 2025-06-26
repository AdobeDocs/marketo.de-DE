---
description: Dynamic Chat-Versionshinweise – Marketo-Dokumente – Produktdokumentation
title: Versionshinweise zu Dynamic Chat
feature: Release Information, Dynamic Chat
hide: true
hidefromtoc: true
source-git-commit: ce7142e471271dfb33b265e226b67bcc3b35594b
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 4%

---

# Versionshinweise zu Dynamic Chat {#dynamic-chat-release}

Adobe Dynamic Chat-Versionen basieren auf einem kontinuierlichen Bereitstellungsmodell, das einen besser skalierbaren Ansatz für die Bereitstellung von Funktionen ermöglicht. Manchmal gibt es mehrere Versionen in einem Monat, daher schauen Sie regelmäßig nach den aktuellsten Informationen.

Die Seite mit den standardmäßigen Versionshinweisen für Marketo Engage [finden Sie hier](/help/marketo/release-notes/current.md){target="_blank"}.

## Version Juni 2025 {#june-25-release}

### Überarbeitung der Routing-Logik {#routing-logic-revamp}

Die Live-Chat-Routing-Logik in Dynamic Chat wurde überarbeitet, um ein intelligenteres und vorhersehbareres Interaktionsverhalten über alle Routing-Typen (Account, Custom, Team und Round Robin) hinweg sicherzustellen. Die neue Logik vereinfacht Routing-Flüsse und verbessert die Fallback-Handhabung, wenn Agenten nicht verfügbar sind.

#### Wichtige Verbesserungen im Routing-Verhalten

* **Bis zu zwei Interaktionsversuche pro Sitzung**

   * Das System versucht, eine Verbindung mit höchstens zwei Agenten herzustellen, jedoch ausschließlich innerhalb der primären Routingregel.

   * Wenn ein Agent verfügbar ist, aber nicht reagiert (z. B. abgelehnt oder ausgelassen wird), versucht das System, einen zweiten Agenten aus demselben Pool zu verwenden.

   * Fallback-Logik (wie Round Robin) wird nur aktiviert, wenn während der ersten Auflösung keine geeigneten Agenten gefunden werden - nicht erneut versuchen nach einer fehlgeschlagenen Interaktion.

* **Routingregelspezifisches Verhalten**

_**Konto-Routing**_

Wenn die E-Mail-Domain eines Besuchers einem bekannten Konto zugeordnet ist, wird der zugeordnete Agent immer priorisiert.

Wenn der Agent verfügbar ist, wird der Chat direkt an ihn weitergeleitet.

Wenn der Agent nicht verfügbar ist, führt das System Folgendes aus:

Versucht keinen anderen Agenten, auch wenn Round Robin als Ausweichlösung aktiviert ist.

Stattdessen gilt Folgendes:

Zeigt den Besprechungskalender des zugeordneten Agenten an (falls aktiviert) oder

Kehrt zu einer Standardmeldung zurück (im schlimmsten Fall).

Die Routing-Regel auf Kartenebene (z. B. Team, Benutzerdefiniert) wird nur berücksichtigt, wenn das Konto-Routing nicht zulässig ist (keine übereinstimmende Domain oder Agent).

_**Benutzerdefiniertes/Team-Routing**_

Diese Regeln können mehrere geeignete Agenten zurückgeben.

Wenn der erste verfügbare Agent nicht interagiert, versucht das System einen weiteren Agenten aus derselben Liste.

Ein Round-Robin-Fallback wird nicht ausgelöst, nur weil ein Agent nicht reagiert hat.

Wenn keiner der Agenten eingreift:

Das System zeigt den Kalender des ersten Agenten an (falls aktiviert) oder

Zeigt die standardmäßige Fallback-Nachricht an.

_**Round Robin-Routing**_

Bei Verwendung als primäre Routingregel führt das System Folgendes durch:

Versucht, den ersten verfügbaren Agenten aus dem Round-Robin-Pool zu kontaktieren.

Wenn der erste nicht reagiert, versucht er es erneut mit dem nächstbesten geeigneten Agenten.

Wenn Round Robin als Fallback verwendet wird, wird er nur aktiviert, wenn keine Agenten von der primären Regel aufgelöst werden.

**Besuchererlebnis-Fluss**

Das System prüft, ob Konto-Routing anwendbar ist.

Wenn ja und der Agent verfügbar ist, → sofort eine Verbindung herzustellen.

Wenn nicht geeignet oder kein Agent verfügbar ist, → Sie mit der Routing-Regel auf Kartenebene fortfahren.

Routingregel auf Kartenebene (benutzerdefiniert, Team, Round Robin) wird ausgewertet.

Berechtigte Agenten werden auf Verfügbarkeit geprüft (Berechtigungen, Status).

Das System greift auf einen Agenten zu und versucht bei Bedarf einen zweiten Agenten aus derselben Regel.

Wenn keine Interaktion erfolgreich ist, wird → Fallback-Logik angewendet:

Kalender-Fallback (falls aktiviert) oder

Standardnachricht.

Ein Round-Robin-Fallback wird nur berücksichtigt, wenn keine geeigneten Agenten aus der primären Routing-Regel gefunden werden - nicht, wenn einzelne Agenten nicht reagieren.

**Nutzungsszenarios**

Konto-Routing

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

Benutzerdefiniertes Routing

<table><thead>
  <tr>
    <th>Typ</th>
    <th>Beispiel</th>
    <th>Ergebnis</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>TEXT</td>
    <td>TEXT</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>TEXT</td>
    <td>TEXT</td>
  </tr>
  <tr>
    <td>Kein Fallback-Agent</td>
    <td>TEXT</td>
    <td>TEXT</td>
  </tr>
</tbody></table>

Team-Routing

<table><thead>
  <tr>
    <th>Typ</th>
    <th>Beispiel</th>
    <th>Ergebnis</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>TEXT</td>
    <td>TEXT</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>TEXT</td>
    <td>TEXT</td>
  </tr>
  <tr>
    <td>Kein Fallback-Agent</td>
    <td>TEXT</td>
    <td>TEXT</td>
  </tr>
</tbody></table>

Round Robin-Routing

<table><thead>
  <tr>
    <th>Typ</th>
    <th>Beispiel</th>
    <th>Ergebnis</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Ideal</td>
    <td>TEXT</td>
    <td>TEXT</td>
  </tr>
  <tr>
    <td>Fallback (Round Robin)</td>
    <td>TEXT</td>
    <td>TEXT</td>
  </tr>
  <tr>
    <td>Kein Fallback-Agent</td>
    <td>TEXT</td>
    <td>TEXT</td>
  </tr>
</tbody></table>

### Impuls-Benachrichtigung {#pulse-notification}

Wenn ein Besucher die Verbindung zu einem Agenten anfordert, stellen wir dem Agenten heute eine In-App-Browser-Benachrichtigung zur Verfügung, aber Agenten fehlen oft diese Chats.

* Jetzt erhält der Live-Agent eine E-Mail-, Slack-, In-App- oder Browser-Benachrichtigung, wenn ein neuer Besucher am Chat interessiert ist

* Der Inhalt für die Pulse-Benachrichtigung kann dem entsprechen, was wir heute für die In-App- und Browser-Benachrichtigung verwenden

Das Verhalten sollte dasselbe sein wie aktuell, damit der Agent akzeptieren kann, wenn mehrere Agenten akzeptieren.
