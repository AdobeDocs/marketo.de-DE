---
description: Live-Chat-Übersicht - Marketo-Dokumente - Produktdokumentation
title: Live-Chat-Übersicht
feature: Dynamic Chat
exl-id: 44e8b249-b534-4cec-a612-daa184acd266
source-git-commit: 870dd6df82c605fffa6681d68867354084988bcd
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 2%

---

# Live-Chat-Übersicht {#live-chat-overview}

Der Live-Chat ermöglicht es Website-Besuchern, mit Ihren Vertriebsmitarbeitern in Echtzeit Chat-Gespräche zu führen.

## Hinzufügen von Live-Chat-Agenten {#add-live-chat-agents}

Um mit dem Live-Chat zu beginnen, müssen Sie Ihre Live-Chat-Agenten als [Benutzer in Adobe Admin Console](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user){target="_blank"} and give them the [Live Chat permission](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md){target="_blank"}. Danach können Sie eine [Live-Chat-Karte](#using-the-live-chat-card) in ein neues oder vorhandenes Dialogfeld.

Wenn Besucher über Ihr Dialogfeld einen Chat mit einem Agenten anfordern, haben Agenten mehrere [Benachrichtigungsoptionen](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#live-chat-notifications){target="_blank"}. When they click on the notification, they'll be taken to their [Agent Inbox](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"} wo sie beginnen können, mit dem Besucher zu chatten.

>[!NOTE]
>
>Der Live-Agent-Avatar verwendet das Profilbild aus dem Adobe-Kontoprofil des Agenten. Gehen Sie wie folgt vor, um das Bild zu aktualisieren [diese Schritte](https://helpx.adobe.com/manage-account/using/edit-adobe-account-personal-profile.html){target="_blank"}.

## Verwenden der Live-Chat-Karte {#using-the-live-chat-card}

Verwenden Sie die Live-Chat-Karte im [Stream-Designer](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md){target="_blank"} wenn Sie möchten, dass Besucher mit einem Live-Agenten chatten.

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
   <td><b>Agentin oder Agent</b></td>
   <td>Wählen Sie einen bestimmten Agenten, um den Chat zu erhalten.</td>
  </tr>
    <tr> 
   <td><b>Benutzerspezifische Regeln</b></td>
   <td>Alle benutzerspezifischen Regeln werden durchlaufen, wenn überlegt wird, wohin der Besucher weitergeleitet werden soll. Wenn der Besucher sich nicht für eine benutzerspezifische Regel qualifiziert, erhält er die Variable <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-management.md#live-chat-fallback" target="_blank">Fallback-Meldung zum Live-Chat</a>.</td>
  </tr> 
  <tr> 
   <td><b>Team</b></td>
   <td>Wählen Sie ein bestimmtes Team aus, um den Chat zu erhalten. Wenn diese Option ausgewählt ist, wird ihr innerhalb des Teams ein rundes Rotationssymbol zugewiesen.</td>
  </tr>
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Agenten-Posteingang](/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md){target="_blank"}
