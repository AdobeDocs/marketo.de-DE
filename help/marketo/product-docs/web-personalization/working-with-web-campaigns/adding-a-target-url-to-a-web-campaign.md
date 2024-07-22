---
unique-page-id: 6094879
description: Hinzufügen einer Target-URL zu einer Webkampagne - Marketo Docs - Produktdokumentation
title: Hinzufügen einer Target-URL zu einer Web-Kampagne
exl-id: 5fbb3f12-1474-46c3-8315-8d081422e154
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 3%

---

# Hinzufügen einer Target-URL zu einer Web-Kampagne {#adding-a-target-url-to-a-web-campaign}

Eine Target-URL befindet sich unter der Seite &quot;Kampagne festlegen&quot;und definiert die spezifischen URLs, auf denen eine Web-Kampagne erscheinen soll.

## Hinzufügen einer Target-URL für Dialogfeld- oder Widget-Web-Kampagnen {#adding-a-target-url-for-dialog-or-widget-web-campaigns}

1. Wechseln Sie zu **Web-Kampagnen**.

   ![](assets/web-campaigns-hand-5.jpg)

1. Wählen Sie **Neue Webkampagne erstellen** aus.

   ![](assets/create-new-web-campaign-hand.jpg)

1. Fügen Sie einen **Kampagnennamen** hinzu. Wählen Sie ein **Zielsegment** aus. Fügen Sie **Ziel-URL** hinzu.

   ![](assets/set-web-campaign-hands.jpg)

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">Name</th> 
   <th colspan="1" rowspan="1">Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1"><strong>Beliebige Seite</strong></td> 
   <td colspan="1" rowspan="1"><p>Lassen Sie zu, dass die Kampagne auf allen Seiten angezeigt wird.</p></td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1"><p><strong>URL-Parameter beim Abgleich einbeziehen</strong></p></td> 
   <td colspan="1" rowspan="1">Fügen Sie den URL-Parameter hinzu, der mit der Kampagne auf URLs, einschließlich dieses Parameters, übereinstimmt und diese anzeigt. Z. B. campaign=cpc</td> 
  </tr> 
 </tbody> 
</table>

## Hinzufügen mehrerer URLs zur Target-URL {#adding-multiple-urls-to-target-url}

Wenn Sie auf das Pluszeichen (![—](assets/image2015-2-18-8-3a40-3a59.png)) klicken, wird das Dialogfeld &quot;Eintrag für mehrere Werte&quot;geöffnet, um mehrere URLs hinzuzufügen. Fügen Sie pro Zeile eine URL hinzu.

![](assets/image2015-2-23-18-3a15-3a57.png)

>[!NOTE]
>
>* Web-Kampagnen für Dialogfeld und Widget können die Optionen Beliebige Seite und Platzhalter (&#42;) verwenden.
* In erweiterten Anwendungsfällen können In-Zone-Webkampagnen Platzhalter am Ende des URL-Pfads verwenden. Beispiel: [www.marketo.com/software/personalization/*](https://www.marketo.com/software/web-personalization/)
* Bei URL wird zwischen Groß- und Kleinschreibung unterschieden

## Hinzufügen einer Ziel-URL für In-Zone-Web-Kampagnen {#adding-a-target-url-for-in-zone-web-campaigns}

1. Gehen Sie zu **Web** **Kampagnen**.

   ![](assets/web-campaigns-hand-5.jpg)

1. Wählen Sie **Neue Webkampagne erstellen** aus.

   ![](assets/create-new-web-campaign-hand.jpg)

1. Fügen Sie einen **Kampagnennamen** hinzu. Wählen Sie ein **Zielsegment** aus. Fügen Sie **Ziel-URL** hinzu.

   >[!NOTE]
   >
   Ziel-URL mit In-Bereichen muss eine bestimmte URL oder URLs definieren. In erweiterten Anwendungsfällen können In-Zone-Webkampagnen Platzhalter am Ende des URL-Pfads verwenden. Beispiel: [www.marketo.com/software/personalization/*](https://www.marketo.com/software/web-personalization/)

   ![](assets/set-web-campaign-multiple-hands.jpg)

>[!MORELIKETHIS]
>
* [Erstellen einer Dialogfeldkampagne](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
* [Erstellen eines RTP in einer Bereichskampagne](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-in-zone-web-campaign.md)
* [Erstellen einer RTP-Widget-Kampagne](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
