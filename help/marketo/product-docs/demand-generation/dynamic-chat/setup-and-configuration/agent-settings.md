---
description: Agenteneinstellungen - Marketo-Dokumente - Produktdokumentation
title: Agenteneinstellungen
feature: Dynamic Chat
exl-id: a782ef9b-6a89-448a-8bd9-f127ceea3bf5
source-git-commit: 8cc63658ddd0e5b6343dc690d4009d4466250998
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 1%

---

# Agenteneinstellungen {#agent-settings}

Konfigurieren Sie Ihren Kalender und legen Sie die Verfügbarkeit von Meetings/Live-Chats fest.

>[!PREREQUISITES]
>
>Stellen Sie sicher, dass Ihren Agenten die entsprechenden [Berechtigungen“ ](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md){target="_blank"} wurden.

![](assets/agent-settings-1.png)

## Kalender verbinden {#connect-calendar}

Verbinden Sie auf der Registerkarte Kalenderkonfiguration Ihren Outlook- oder Gmail-Kalender zur Verwendung bei der Terminplanung im Chatbot.

![](assets/agent-settings-2.png)

Sobald der Kalender eines Benutzers mit Dynamic Chat verbunden ist, wird er zur Warteschlange hinzugefügt und sein Kalender steht Website-Besuchern zur Terminplanung zur Verfügung.

>[!NOTE]
>
>Pro Benutzer kann ein Kalender verbunden werden. Wenn Sie Meetings über mehrere Kalender empfangen möchten, müssen Sie mehrere Benutzer hinzufügen und sie jeweils mit ihren Kalendern verbinden lassen.

Benutzer können auch den Textkörper der Einladung anpassen, die an den Besucher gesendet wird, wenn sie einen Termin im Kalender des Benutzers planen. Sie können auch das Kontrollkästchen unten aktivieren, um einen Google Meet- oder Microsoft Teams-Link einzufügen (je nachdem, welcher Kalender verbunden wurde).

![](assets/agent-settings-3.png)

>[!TIP]
>
>Verwenden Sie das Token-Symbol (geschweifte Klammern), um Ihre Bestätigungs-E-Mails für die Besprechungsbuchung mit Personen- oder Firmenattributen zu personalisieren.

### Berechtigungen {#permissions}

Durch die Konfiguration mit Outlook werden Dynamic Chat die folgenden Berechtigungen gewährt:

* Vollständiger Zugriff auf Ihre Kalender
* Anmelden und Profil lesen
* Beibehaltung des Zugriffs auf Daten, auf die Sie Zugriff gewährt haben
* Mailbox-Einstellungen lesen

Durch die Konfiguration mit Google werden Dynamic Chat die folgenden Berechtigungen gewährt:

* Kalender erstellen, ändern oder löschen
* Aktualisieren einzelner Kalenderereignisse
* Ändern Sie Ihre Einstellungen, einschließlich der Personen, die Ihre Ereignisse sehen können.
* Ändern, für wen der Kalender freigegeben wird
* Zugriff auf Ihren Namen, Ihre E-Mail-Adresse, Ihre Spracheinstellungen und Ihr Profilbild

## Verfügbarkeit der Meeting-Buchung {#meeting-booking-availability}

Legen Sie Ihre Zeitzone und Zeit/Wochentag-Verfügbarkeit fest, um Besprechungsbuchungen zu erhalten.

![](assets/agent-settings-4.png)

<table> 
 <tbody> 
  <tr> 
   <td><b>Meeting-Dauer</b></td>
   <td>Legt fest, wie lange Besucherinnen und Besucher in Ihren verfügbaren Meeting-Slots sehen werden.</td>
  </tr> 
  <tr> 
   <td><b>Pufferzeit zwischen Meetings</b></td>
   <td>Die Zeit, die Sie als Puffer für nach dem Meeting festlegen. Wenn Sie die Dauer auf 30 Minuten festlegen, kann bis 30 Minuten nach dem geplanten Ende einer Besprechung in Ihrem Kalender niemand eine Besprechung mit Ihnen buchen.</td>
  </tr>
 </tbody> 
</table>

>[!TIP]
>
>Sie können mehrere Zeitblöcke am selben Tag auswählen (z. B. Freitag von 8a-12p _und_ 1p-5p), indem Sie auf das **+** rechts klicken.

## Live-Chat-Verfügbarkeit {#live-chat-availability}

Legen Sie Ihre Zeitzone und Zeit/Wochentag-Verfügbarkeit fest, um Live-Chats zu erhalten.

![](assets/agent-settings-5.png)

Wenn Sie bei der App eingeloggt sind, erhalten Sie eine In-App-Benachrichtigung über einen eingehenden Chat. Wenn Sie nicht angemeldet sind, erhalten Sie eine Browser-Benachrichtigung (wenn Sie [eingerichtet haben](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#live-chat-notifications){target="_blank"}).

>[!IMPORTANT]
>
>* Der Umschalter [Verfügbarkeit](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#availability-toggle){target="_blank"} im Agenten-Posteingang **überschreibt** was auf der Registerkarte _Verfügbarkeit des Live-Chat_ eingegeben wird. Wenn der Agent also von 1p-5p verfügbar ist, aber eine kurze Pause bei 3p einlegen muss, müssen die Agenteneinstellungen nicht geändert werden. Der Status des Verfügbarkeits-Umschalters bleibt erhalten, bis er manuell geändert wird, bis der nächste Zeitblock in der Verfügbarkeit des Agenten erreicht wird, oder bis Mitternacht in der angegebenen Zeitzone des Agenten (weitere Informationen finden Sie im nächsten Aufzählungszeichen).
>
>* Wenn der Agent den Umschalter Verfügbarkeit verwendet, um den Status in „Verfügbar“ zu ändern, wird sein Status um Mitternacht in der in seinem Verfügbarkeitsplan angegebenen Zeitzone automatisch zurückgesetzt (wechselt zu „Nicht verfügbar„). Wenn keine Zeitzone angegeben ist, wird standardmäßig UTC (Coordinated Universal Time) verwendet.

>[!TIP]
>
>Sie können mehrere Zeitblöcke am selben Tag auswählen (z. B. Freitag von 8a-12p _und_ 1p-5p), indem Sie auf das **+** rechts klicken.

## Agentprofil-Foto

Ein Agent kann zwar sein eigenes Profilfoto hochladen, diese Aktion wird jedoch nicht in Dynamic Chat ausgeführt. Sie müssten zu `account.adobe.com/profile` navigieren. Weitere Informationen finden Sie [Kontoprofil aktualisieren](https://helpx.adobe.com/de/manage-account/using/edit-adobe-account-personal-profile.html).

>[!NOTE]
>
>Das in `experience.adobe.com` angezeigte Profilbild wird **nicht**.
