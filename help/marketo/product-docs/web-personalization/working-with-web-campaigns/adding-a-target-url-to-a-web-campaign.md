---
unique-page-id: 6094879
description: Hinzufügen einer Ziel-URL zu einer Web-Kampagne - Marketo-Dokumente - Produktdokumentation
title: Hinzufügen einer Ziel-URL zu einer Web-Kampagne
exl-id: 5fbb3f12-1474-46c3-8315-8d081422e154
feature: Web Personalization
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 1%

---

# Hinzufügen einer Ziel-URL zu einer Web-Kampagne {#adding-a-target-url-to-a-web-campaign}

Unter der Seite Kampagne festlegen befindet sich eine Ziel-URL, die die spezifischen URLs definiert, unter denen eine Web-Kampagne angezeigt wird.

## Hinzufügen einer Ziel-URL für Dialog- oder Widget-Web-Kampagnen {#adding-a-target-url-for-dialog-or-widget-web-campaigns}

1. Gehen Sie zu **[!UICONTROL Web-Kampagnen]**.

   ![](assets/web-campaigns-hand-5.jpg)

1. Wählen **[!UICONTROL Neue Web-Kampagne erstellen]**.

   ![](assets/create-new-web-campaign-hand.jpg)

1. Fügen Sie einen **[!UICONTROL Kampagnennamen“]**. Wählen Sie ein **[!UICONTROL Zielsegment]** aus. Fügen Sie **[!UICONTROL Target-URL]** hinzu.

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
   <td colspan="1" rowspan="1"><strong>[!UICONTROL Beliebige Seite]</strong></td>
   <td colspan="1" rowspan="1"><p>Kampagne darf auf jeder Seite angezeigt werden.</p></td>
  </tr>
  <tr>
   <td colspan="1" rowspan="1"><p><strong>[!UICONTROL URL-Parameter beim Abgleichen einschließen]</strong></p></td>
   <td colspan="1" rowspan="1">Fügen Sie einen URL-Parameter hinzu, um Kampagnen-URLs, die diesen Parameter enthalten, abzugleichen und anzuzeigen. Z. B. campaign=cpc</td>
  </tr>
 </tbody>
</table>

## Hinzufügen mehrerer URLs zur Ziel-URL {#adding-multiple-urls-to-target-url}

Durch Klicken auf das Pluszeichen (![—](assets/image2015-2-18-8-3a40-3a59.png)) wird das Dialogfeld [!UICONTROL Eingabe mehrerer Werte] geöffnet, um mehrere URLs hinzuzufügen. Fügen Sie pro Zeile eine URL hinzu.

![](assets/image2015-2-23-18-3a15-3a57.png)

>[!NOTE]
>
>* Web-Kampagnen für Dialogfelder und Widgets können Optionen für beliebige Seiten und Platzhalter (&#42;) verwenden.
>* In erweiterten Anwendungsfällen können In-Zone-Web-Kampagnen Platzhalter am Ende des URL-Pfads verwenden. Beispiel: [www.marketo.com/software/personalization/*](https://www.marketo.com/software/web-personalization/)
>* URL unterscheidet zwischen Groß- und Kleinschreibung

## Hinzufügen einer Ziel-URL für In-Zone-Web-Kampagnen {#adding-a-target-url-for-in-zone-web-campaigns}

1. Gehen Sie zu **[!UICONTROL Web-Kampagnen]**.

   ![](assets/web-campaigns-hand-5.jpg)

1. Wählen **[!UICONTROL Neue Web-Kampagne erstellen]**.

   ![](assets/create-new-web-campaign-hand.jpg)

1. Fügen Sie einen **[!UICONTROL Kampagnennamen“]**. Wählen Sie ein **[!UICONTROL Zielsegment]** aus. Fügen Sie **[!UICONTROL Target-URL]** hinzu.

   >[!NOTE]
   >
   >Ziel-URL mit In-Zonen muss eine oder mehrere bestimmte URLs definieren. In erweiterten Anwendungsfällen können In-Zone-Web-Kampagnen Platzhalter am Ende des URL-Pfads verwenden. Beispiel: [www.marketo.com/software/personalization/*](https://www.marketo.com/software/web-personalization/)

   ![](assets/set-web-campaign-multiple-hands.jpg)

>[!MORELIKETHIS]
>
>* [Erstellen einer Dialogfeldkampagne](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-dialog-web-campaign.md)
>* [Erstellen einer RTP-Zone in Campaign](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-in-zone-web-campaign.md)
>* [Erstellen einer RTP-Widget-Kampagne](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/create-a-new-widget-web-campaign.md)
