---
description: Live-Chat-Übersicht - Marketo-Dokumente - Produktdokumentation
title: Live-Chat-Übersicht
feature: Dynamic Chat
exl-id: 44e8b249-b534-4cec-a612-daa184acd266
source-git-commit: d88406c1f9d72c57a6d4f09934cbf685499ed198
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 1%

---

# Live-Chat-Übersicht {#live-chat-overview}

Der Live-Chat ermöglicht es Website-Besuchern, mit Ihren Vertriebsmitarbeitern in Echtzeit Chat-Gespräche zu führen.

>[!NOTE]
>
>Für diejenigen auf dem Dynamic Chat Select-Paket ist der Live-Chat eine Testfunktion mit einer Lebensdauer von 100 Interaktionen. Wenn diese Grenze erreicht ist, werden alle Besucher, die einen Chat mit einem Live-Agenten anfordern, nicht verbunden und erhalten stattdessen die globale Ausweichmeldung. Wenden Sie sich an Ihren Adobe-Kundenbetreuer, um die Optionen für ein Package-Upgrade zu besprechen.

## Hinzufügen von Live-Chat-Agenten {#add-live-chat-agents}

Um mit dem Live-Chat zu beginnen, müssen Sie Ihre Live-Chat-Agenten als [Benutzer in der Adobe Admin Console](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user){target="_blank"} hinzufügen und ihnen die [Berechtigung zum Live-Chat](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md){target="_blank"} erteilen. Danach können Sie eine [Live-Chat-Karte](#using-the-live-chat-card) zu einem neuen oder vorhandenen Dialogfeld hinzufügen.

Wenn Besucher über Ihr Dialogfeld anfordern, mit einem Agenten zu chatten, haben Agenten mehrere [Benachrichtigungsoptionen](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#live-chat-notifications){target="_blank"}. Wenn sie auf die Benachrichtigung klicken, gelangen sie zum [Agenten-Posteingang](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"}, wo sie mit dem Chat mit dem Besucher beginnen können.

>[!NOTE]
>
>Der Live-Agent-Avatar verwendet das Profilbild aus dem Adobe-Kontoprofil des Agenten. Um das Bild zu aktualisieren, führen Sie [diese Schritte](https://helpx.adobe.com/de/manage-account/using/edit-adobe-account-personal-profile.html){target="_blank"} aus.

## Verwenden der Live-Chat-Karte {#using-the-live-chat-card}

Verwenden Sie die Live-Chat-Karte im [Stream-Designer](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md){target="_blank"}, wenn Sie möchten, dass Besucher mit einem Live-Agenten chatten.

![](assets/live-chat-overview-1.png)

>[!IMPORTANT]
>
>Die Live-Chat-Karte muss immer die letzte Karte im Zweig sein. Wenn die Karte an einem zufälligen Punkt im Zweig platziert wird, kann dies den Besucher überraschen, indem er sie plötzlich mit einem Agenten verbindet.

### Bewährte Methoden {#best-practices}

* Verwenden Sie eine Fragenkarte vor der Live-Chat-Karte und fragen Sie den Besucher, ob er eine Verbindung herstellen möchte.
* Nachdem der Besucher einer Verbindung zugestimmt hat, verwenden Sie die Datenerfassungskarte, um einige seiner Informationen zu sammeln, z. B. Vor-/Nachname, E-Mail-Adresse, Berufsbezeichnung usw. (Es wird empfohlen, mindestens Vorname und E-Mail-Adresse anzufordern).

## Optionen für Live-Chat-Karten {#live-chat-card-options}

Durch Klicken auf die Live-Chat-Karte im Stream können Sie festlegen, wie der Besucher weitergeleitet wird. Wählen Sie aus dem runden Rund-Rund-Rad, einem Agenten, benutzerdefinierten Regeln oder einem Team.

![](assets/live-chat-overview-2.png)

<table> 
 <tbody> 
  <tr> 
   <td><b>Round-Robin</b></td>
   <td>Chats werden Agenten in sequenzieller Reihenfolge zugewiesen.</td>
  </tr> 
  <tr> 
   <td><b>Agent</b></td>
   <td>Wählen Sie einen bestimmten Agenten, um den Chat zu erhalten.</td>
  </tr>
    <tr> 
   <td><b>Benutzerspezifische Regeln</b></td>
   <td>Alle benutzerspezifischen Regeln werden durchlaufen, wenn überlegt wird, wohin der Besucher weitergeleitet werden soll. Wenn der Besucher nicht für eine benutzerspezifische Regel qualifiziert ist, erhält er die <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-management.md#live-chat-fallback" target="_blank">Live-Chat-Fallback-Meldung</a>.</td>
  </tr> 
  <tr> 
   <td><b>Team</b></td>
   <td>Wählen Sie ein bestimmtes Team aus, um den Chat zu erhalten. Wenn diese Option ausgewählt ist, wird ihr innerhalb des Teams ein rundes Rotationssymbol zugewiesen.</td>
  </tr>
 </tbody> 
</table>

## Live-Chat-Benachrichtigungen {#live-chat-notifications}

>[!IMPORTANT]
>
>Um Browser-Benachrichtigungen für Live-Chat zu erhalten, müssen alle Live-Chat-Agenten Browserbenachrichtigungen für Dynamic Chat aktivieren, wenn sie dazu aufgefordert werden.

### Aktivieren von Benachrichtigungen {#enabling-notifications}

Live-Chat-Agenten sehen oben auf dem Bildschirm ein Banner, in dem sie sich anmelden: &quot;Bitte aktivieren Sie Browser-Benachrichtigungen, um Live-Chat-Benachrichtigungen zu erhalten&quot;. Klicken Sie auf **Aktivieren**.

![](assets/live-chat-overview-4.png)

Die Live-Chat-Agenten werden dann vom Browser aufgefordert, Benachrichtigungen anzuzeigen. Klicken Sie auf **Allow**.

![](assets/live-chat-overview-5.png)

Wenn Agenten keine Browser-Benachrichtigungen erhalten, auch wenn sie dies im Browser zulassen, müssen sie möglicherweise Benachrichtigungen für den Browser in den Benachrichtigungseinstellungen des Betriebssystems aktivieren:

[Schritte für Mac](https://support.apple.com/guide/mac-help/change-notifications-settings-mh40583/mac){target="_blank"}

[Schritte für Windows](https://support.microsoft.com/en-us/windows/change-notification-settings-in-windows-8942c744-6198-fe56-4639-34320cf9444e){target="_blank"}

### Wenn ein Live-Chat zu einem Agenten weitergeleitet wird {#when-a-live-chat-is-routed-to-an-agent}

Wenn ein Live-Chat an einen Agenten weitergeleitet wird, wird ihm oben im Bildschirm ein blaues Banner angezeigt, in dem er zur Annahme aufgefordert wird, sowie ein Benachrichtigungston, der dazu beiträgt, verpasste Benachrichtigungen zu vermeiden.

![](assets/live-chat-overview-3.png)

>[!TIP]
>
>Sie können auch Browser-Benachrichtigungen einrichten, die Sie benachrichtigen, falls Sie nicht bei Dynamic Chat angemeldet sind.
>
>* Browserbenachrichtigungen in [Google Chrome](https://support.google.com/chrome/answer/3220216?hl=en&amp;co=GENIE.Platform%3DDesktop){target="_blank"} aktivieren
>* Browserbenachrichtigungen in [Mozilla Firefox](https://support.mozilla.org/en-US/kb/push-notifications-firefox){target="_blank"} aktivieren

### Fehlgeschlagene Aktionsbenachrichtigungen {#failed-action-notifications}

Wenn eine Aktion wie die Buchung eines Meetings oder ein Live-Chat fehlschlägt, werden die Benutzer per E-Mail benachrichtigt.

![](assets/live-chat-overview-6.png)

### Zu beachten {#things-to-note}

* Agenten haben 45 Sekunden Zeit, um zu antworten, bevor die &quot;Chat akzeptieren&quot;-Nachricht eine Zeitüberschreitung aufweist. Danach erhalten Besucher die [Ausweichmeldung](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-management.md#live-chat-fallback){target="_blank"}. Bei Dynamic Chat Prime-Abonnenten, für die die Routing-Option auf **Team** festgelegt ist, wird ein weiterer Agent versucht, bevor die Ausweichmeldung angezeigt wird.
* Derzeit sind 10 Live-Chats pro Agent erlaubt.

>[!MORELIKETHIS]
>
>[Agent-Posteingang](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"}
