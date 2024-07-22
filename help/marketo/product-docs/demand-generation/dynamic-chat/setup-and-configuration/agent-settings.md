---
description: Agenteneinstellungen - Marketo-Dokumente - Produktdokumentation
title: Agenteneinstellungen
feature: Dynamic Chat
exl-id: a782ef9b-6a89-448a-8bd9-f127ceea3bf5
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 2%

---

# Agenteneinstellungen {#agent-settings}

Konfigurieren Sie Ihren Kalender und legen Sie die Verfügbarkeit von Meetings/Live-Chat fest.

>[!PREREQUISITES]
>
>Stellen Sie sicher, dass Ihren Agenten die entsprechenden [Berechtigungen](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md){target="_blank"} gewährt wurden.

![](assets/agent-settings-1.png)

## Verbindungskalender {#connect-calendar}

Verbinden Sie im Tab Kalenderkonfiguration Ihren Outlook- oder Gmail-Kalender mit der Terminplanung im Chat.

![](assets/agent-settings-2.png)

Sobald der Kalender eines Benutzers mit der Dynamic Chat verbunden ist, wird er der Warteschlange hinzugefügt und sein Kalender steht Website-Besuchern zur Verfügung, um Termine zu planen.

>[!NOTE]
>
>Sie können einen Kalender pro Benutzer verbinden. Wenn Sie Meetings auf mehreren Kalendern erhalten möchten, müssen Sie mehrere Benutzer hinzufügen und sie jeweils dazu bewegen, ihre Kalender zu verbinden.

Benutzer können auch den Text der Einladung anpassen, die dem Besucher gesendet wird, wenn er einen Termin im Kalender des Benutzers einplant. Sie können auch das Kontrollkästchen am unteren Rand aktivieren, um einen Google-Treffer- oder Microsoft Teams-Link einzuschließen (je nachdem, welcher Kalender verbunden war).

![](assets/agent-settings-3.png)

>[!TIP]
>
>Verwenden Sie das Token-Symbol (geschweifte Klammern), um Ihre Bestätigungs-E-Mails für die Buchung von Meetings anhand von Personen- oder Firmenattributen zu personalisieren.

### Berechtigungen {#permissions}

Durch die Konfiguration mit Outlook erhalten Sie die folgenden Berechtigungen zum Dynamic Chat:

* Vollständiger Zugriff auf Ihre Kalender
* Anmelden und Profil lesen
* Beibehalten des Zugriffs auf die Daten, auf die Sie Zugriff gewährt haben
* E-Mail-Einstellungen lesen

Die Konfiguration mit Google gewährt die folgenden Berechtigungen für Dynamic Chat:

* Kalender erstellen, ändern oder löschen
* Aktualisieren einzelner Kalenderereignisse
* Ändern Sie Ihre Einstellungen, einschließlich der Benutzer, die Ihre Ereignisse sehen können.
* Ändern der Zielgruppe des Kalenders
* Zugriff auf Ihren Namen, Ihre E-Mail-Adresse, Ihre Spracheinstellung und Ihr Profilbild

## Verfügbarkeit von Konferenzbuchungen {#meeting-booking-availability}

Legen Sie Ihre Zeitzone und die Zeit/den Wochentag fest, um Sitzungsbuchungen zu erhalten.

![](assets/agent-settings-4.png)

<table> 
 <tbody> 
  <tr> 
   <td><b>Meeting-Dauer</b></td>
   <td>Bestimmt, wie lange Besucher in den verfügbaren Sitzungsplätzen sehen.</td>
  </tr> 
  <tr> 
   <td><b>Pufferzeit zwischen Meetings</b></td>
   <td>Zeit, die Sie als Puffer für nach dem Meeting eingestellt haben. Wenn Sie es für 30 Minuten festlegen, kann niemand ein Meeting mit Ihnen bis 30 Minuten nach dem geplanten Ende eines Meetings in Ihrem Kalender buchen.</td>
  </tr>
 </tbody> 
</table>

>[!TIP]
>
>Sie können mehrere Zeitblöcke am selben Tag auswählen (z. B. Freitag von 8a-12p _und_ 1p-5p), indem Sie rechts auf das Symbol **+** klicken.

## Verfügbarkeit von Live-Chat {#live-chat-availability}

Legen Sie Ihre Zeitzone und Zeit/Tag der Woche fest, um Live-Chats zu empfangen.

![](assets/agent-settings-5.png)

Wenn Sie bei der App angemeldet sind, erhalten Sie eine In-App-Benachrichtigung über einen eingehenden Chat. Wenn Sie nicht angemeldet sind, erhalten Sie eine Browserbenachrichtigung (wenn Sie [eingerichtet haben](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#live-chat-notifications){target="_blank"}).

>[!IMPORTANT]
>
>Der Umschalter [Verfügbarkeit](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#availability-toggle){target="_blank"} im Agent-Posteingang **überschreibt**, was Sie auf der Registerkarte &quot;Live-Chat-Verfügbarkeit&quot;eingegeben haben. Wenn Sie also von 1p bis 5p geplant sind, aber eine kurze Pause um 3p machen müssen, müssen Sie Ihre Agenteneinstellungen nicht ändern. Der Umschalter &quot;Verfügbarkeit&quot;behält den Status, bis Sie ihn manuell ändern oder der nächste Zeitblock in Ihrer Verfügbarkeit erreicht ist.

>[!TIP]
>
>Sie können mehrere Zeitblöcke am selben Tag auswählen (z. B. Freitag von 8a-12p _und_ 1p-5p), indem Sie rechts auf das Symbol **+** klicken.
