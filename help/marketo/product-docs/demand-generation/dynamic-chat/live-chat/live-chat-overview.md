---
description: Live-Chat - Übersicht - Marketo-Dokumente - Produktdokumentation
title: Live-Chat - Übersicht
feature: Dynamic Chat
exl-id: 44e8b249-b534-4cec-a612-daa184acd266
source-git-commit: d88406c1f9d72c57a6d4f09934cbf685499ed198
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 1%

---

# Live-Chat - Übersicht {#live-chat-overview}

Live-Chat ermöglicht Besuchenden der Website, mit Ihren Vertriebsmitarbeitern in Echtzeit im Chat zu kommunizieren.

>[!NOTE]
>
>Live-Chat ist eine Testfunktion mit einer Lebenszeitbegrenzung von 100 Interaktionen für Benutzer des Dynamic Chat Select-Pakets. Wenn diese Grenze erreicht ist, werden alle Besucherinnen und Besucher, die einen Chat mit einem Live-Agenten anfordern, nicht verbunden sein und stattdessen die globale Fallback-Nachricht erhalten. Wenden Sie sich zur Erhöhung des Limits an Ihren Adobe-Kundenbetreuer, um die Paket-Upgrade-Optionen zu besprechen.

## Live-Chat-Agenten hinzufügen {#add-live-chat-agents}

Um mit dem Live-Chat zu beginnen, müssen Sie Ihre Live-Chat-Agenten als [Benutzer in der Adobe Admin Console](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user){target="_blank"} hinzufügen und ihnen die [Live-Chat-Berechtigung](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md){target="_blank"} erteilen. Danach können Sie eine &quot;[-Chat-Karte“ ](#using-the-live-chat-card) einem neuen oder vorhandenen Dialogfeld hinzufügen.

Wenn Besucherinnen und Besucher über Ihr Dialogfeld einen Chat mit einem Agenten anfordern, haben Agenten mehrere [Benachrichtigungsoptionen](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#live-chat-notifications){target="_blank"}. Wenn er auf die Benachrichtigung klickt, gelangt er zu seinem [Agenten-Posteingang](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"} wo er mit dem Besucher chatten kann.

>[!NOTE]
>
>Der Live-Agent-Avatar verwendet das Profilbild aus dem Adobe-Kontoprofil des Agenten. Gehen Sie wie folgt vor, um [ Bild ](https://helpx.adobe.com/de/manage-account/using/edit-adobe-account-personal-profile.html){target="_blank"} aktualisieren.

## Verwenden der Live-Chat-Karte {#using-the-live-chat-card}

Verwenden Sie die Live-Chat-Karte in [Stream-Designer](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md){target="_blank"} wenn Sie möchten, dass Besucherinnen und Besucher mit einem Live-Agenten chatten.

![](assets/live-chat-overview-1.png)

>[!IMPORTANT]
>
>Die Live-Chat-Karte muss immer die letzte Karte in der Filiale sein. Wenn die Karte an einer beliebigen Stelle in der Verzweigung platziert wird, könnte sie den Besucher überraschen, indem sie plötzlich mit einem Agenten verbunden wird.

### Bewährte Methoden {#best-practices}

* Verwenden Sie vor dem Live-Chat eine Fragekarte, um den Besucher zu fragen, ob er eine Verbindung herstellen möchte.
* Nachdem der Besucher der Verbindung zugestimmt hat, verwenden Sie die Datenerfassungskarte, um einige seiner Informationen zu erfassen, wie Vor-/Nachname, E-Mail-Adresse, Stellenbezeichnung usw. (Es wird empfohlen, mindestens Vornamen und E-Mail-Adresse anzufordern).

## Live-Chat-Kartenoptionen {#live-chat-card-options}

Wenn Sie im Stream auf die Live-Chat-Karte klicken, können Sie auswählen, wie der Besucher weitergeleitet wird. Wählen Sie aus Round Robin, einem Agenten, benutzerdefinierten Regeln oder einem Team.

![](assets/live-chat-overview-2.png)

<table> 
 <tbody> 
  <tr> 
   <td><b>Round-Robin</b></td>
   <td>Chats werden Agenten in sequenzieller Reihenfolge zugewiesen.</td>
  </tr> 
  <tr> 
   <td><b>Agent</b></td>
   <td>Wählen Sie einen bestimmten Agenten aus, um den Chat zu erhalten.</td>
  </tr>
    <tr> 
   <td><b>Benutzerdefinierte Regeln</b></td>
   <td>Alle benutzerdefinierten Regeln werden durchlaufen, wenn überlegt wird, wohin der Besucher weitergeleitet werden soll. Wenn sich der Besucher nicht für eine benutzerdefinierte Regel qualifiziert, erhält er die <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-management.md#live-chat-fallback" target="_blank">Live-Chat-Fallback-Nachricht</a>.</td>
  </tr> 
  <tr> 
   <td><b>Team</b></td>
   <td>Wählen Sie ein bestimmtes Team aus, um den Chat zu erhalten. Wenn diese Option ausgewählt ist, wird sie innerhalb dieses Teams Round Robin zugewiesen.</td>
  </tr>
 </tbody> 
</table>

## Live-Chat-Benachrichtigungen {#live-chat-notifications}

>[!IMPORTANT]
>
>Um Browser-Benachrichtigungen für Live-Chat zu erhalten, müssen alle Live-Chat-Agenten Browser-Benachrichtigungen für das Dynamic Chat aktivieren, wenn sie dazu aufgefordert werden.

### Aktivieren von Benachrichtigungen {#enabling-notifications}

Live-Chat-Agenten sehen bei der Anmeldung oben im Bildschirm ein Banner mit folgendem Text: „Aktivieren Sie Browser-Benachrichtigungen, um Live-Chat-Benachrichtigungen zu erhalten.“ Klicken Sie **Aktivieren**.

![](assets/live-chat-overview-4.png)

Live-Chat-Agenten werden dann vom Browser aufgefordert, Benachrichtigungen anzuzeigen. Klicken Sie **Zulassen**.

![](assets/live-chat-overview-5.png)

Wenn Kundendienstmitarbeiter keine Browser-Benachrichtigungen erhalten, selbst nachdem sie den Browser zugelassen haben, müssen sie möglicherweise Benachrichtigungen für den Browser in den Einstellungen für die Betriebssystembenachrichtigung aktivieren:

[Schritte für Mac](https://support.apple.com/guide/mac-help/change-notifications-settings-mh40583/mac){target="_blank"}

[Schritte für Windows](https://support.microsoft.com/en-us/windows/change-notification-settings-in-windows-8942c744-6198-fe56-4639-34320cf9444e){target="_blank"}

### Wenn ein Live-Chat an einen Agenten weitergeleitet wird {#when-a-live-chat-is-routed-to-an-agent}

Wenn ein Live-Chat an einen Agenten weitergeleitet wird, sehen sie ein blaues Banner am oberen Bildschirmrand, das sie auffordert, zu akzeptieren, sowie einen Benachrichtigungston, um verpasste Benachrichtigungen zu verhindern.

![](assets/live-chat-overview-3.png)

>[!TIP]
>
>Sie haben auch die Möglichkeit, Browser-Benachrichtigungen einzurichten, die Sie warnen, falls Sie nicht beim Dynamic Chat angemeldet sind.
>
>* Aktivieren von Browser-Benachrichtigungen in [Google Chrome](https://support.google.com/chrome/answer/3220216?hl=en&amp;co=GENIE.Platform%3DDesktop){target="_blank"}
>* Aktivieren von Browser-Benachrichtigungen in [Mozilla Firefox](https://support.mozilla.org/en-US/kb/push-notifications-firefox){target="_blank"}

### Benachrichtigungen zu fehlgeschlagenen Aktionen {#failed-action-notifications}

Wenn eine Aktion wie eine Besprechungsbuchung oder ein Live-Chat fehlschlägt, werden die Benutzer per E-Mail benachrichtigt.

![](assets/live-chat-overview-6.png)

### Zu beachtende Punkte {#things-to-note}

* Die Kundendienstmitarbeiter müssen innerhalb von 45 Sekunden antworten, bevor die Nachricht „Chat akzeptieren“ ihre Zeit verliert. Danach erhalten Besucher die [Fallback-Nachricht](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-management.md#live-chat-fallback){target="_blank"}. Beim Dynamic Chat von Prime-Abonnenten, bei denen die Routing-Option auf **Team** eingestellt ist, wird ein weiterer Agent versucht, bevor die Fallback-Nachricht angezeigt wird.
* Derzeit gibt es eine Beschränkung von 10 Live-Chats pro Agent.

>[!MORELIKETHIS]
>
>[Agent-Posteingang](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"}
