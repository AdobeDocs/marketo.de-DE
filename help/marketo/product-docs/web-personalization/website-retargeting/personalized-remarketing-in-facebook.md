---
unique-page-id: 4720917
description: Personalisiertes Remarketing in Facebook - Marketo-Dokumente - Produktdokumentation
title: Personalisiertes Remarketing in Facebook
exl-id: 47636afa-49df-40ba-8948-4f2850467c2f
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 8%

---

# Personalisiertes Remarketing in [!DNL Facebook] {#personalized-remarketing-in-facebook}

Personalisiertes Remarketing ermöglicht Ihnen die erneute Interaktion mit Ihren Benutzern mithilfe von RTP-Daten und der Leistungsfähigkeit von Facebook-Remarketing.

>[!PREREQUISITES]
>
>* Schließen Sie das Setup [Retargeting mit Web Personalization-Daten](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md) ab
>* Lesen Sie die [](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) [Facebook-Dokumentation zu benutzerdefinierten Zielgruppen](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) und Remarketing.

## Erstellen einer Zielgruppe in [!DNL Facebook] {#creating-an-audience-in-facebook}

1. Wechseln Sie in [!DNL Facebook] zur Registerkarte [Zielgruppe](https://www.facebook.com/ads/audience_manager) in Ads Manager.

1. Klicken Sie auf **[!UICONTROL Tools]** und wählen Sie **[!UICONTROL Zielgruppen]** aus.

   ![](assets/one-1.png)

1. Klicken Sie **[!UICONTROL Benutzerdefinierte Zielgruppe erstellen]**.

   ![](assets/two-1.png)

1. Wählen Sie **[!UICONTROL Website-Traffic]** aus.

   ![](assets/image2015-1-19-16-3a32-3a2.png)

1. Wählen Sie in [!UICONTROL  Liste „Website]Traffic“ **[!UICONTROL Benutzerdefinierte Kombination]** aus.

   ![](assets/image2015-1-19-16-3a33-3a21.png)

1. Wählen Sie in der Liste Einschließen die Option **[!UICONTROL Ereignis]** aus.

   ![](assets/image2015-1-19-16-3a34-3a9.png)

1. Wählen Sie in der [!UICONTROL Ereignis]-Liste **[!UICONTROL RTP-Remarketing]** aus und wählen Sie einen Parameter aus.

   ![](assets/image2015-1-19-16-3a52-3a29.png)

1. Wählen Sie für dieses Beispiel [!UICONTROL Branche] aus, um **[!UICONTROL Bildung]** einzuschließen. Geben Sie **[!UICONTROL Bildung]** ein und bearbeiten Sie **[!UICONTROL In den letzten]** auf 180 Tage. Geben Sie den Zielgruppennamen ein: **Education Industry**. Klicken Sie **[!UICONTROL Zielgruppe erstellen]**.

   ![](assets/image2015-1-19-16-3a56-3a15.png)

1. Sie haben jetzt eine neue benutzerdefinierte Zielgruppe mit RTP-Daten in [!DNL Facebook] erstellt.

   ![](assets/image2015-1-19-16-3a59-3a2.png)

## RTP-Datenpunkte in [!DNL Facebook] {#rtp-data-points-in-facebook}

<table> 
 <tbody> 
  <tr> 
   <th>Ereignisname</th> 
   <th> </th> 
  </tr> 
  <tr> 
   <td>RTP-Remarketing</td> 
   <td> 
    <div> 
     <table> 
      <tbody> 
       <tr> 
        <th>Parameter</th> 
        <th>Wert</th> 
       </tr> 
       <tr> 
        <td>ABM-Liste</td> 
        <td>(Name der kontobasierten Liste)</td> 
       </tr> 
       <tr> 
        <td colspan="1">Kategorie</td> 
        <td colspan="1"><p>Fortune 500</p><p>Fortune 1000</p><p>Global 2000</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">Gruppe</td> 
        <td colspan="1"><p>Enterprise</p><p>KMU</p></td> 
       </tr> 
       <tr> 
        <td>Branche</td> 
        <td><p>Verteidigung</p><p>Aus- und Weiterbildung</p><p>Finanzdienstleistungen</p><p>Regierung</p><p>Gesundheitswesen, Pharma, Biotechnologie</p><p>Software und Internet</p><p>etc… (gemäß RTP Industry-Optionen)</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">Segmentierte Zielgruppe</td> 
        <td colspan="1">(Name der in RTP erstellten segmentierten Zielgruppe)</td> 
       </tr> 
      </tbody> 
     </table> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## Targeting Ihrer Audience mit einer Anzeige {#target-your-audience-with-an-ad}

Weitere Informationen finden Sie [Dokumentation von Facebook](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#target-your-audience).

1. Wechseln Sie zum Anzeigen-Manager und klicken Sie auf **[!UICONTROL Anzeige erstellen]**.

   ![](assets/image2015-1-19-17-3a10-3a19.png)

1. Wählen Sie **[!UICONTROL Personen auf Ihre Website senden]** als Ziel Ihrer Kampagne aus.

   ![](assets/image2015-1-19-17-3a11-3a20.png)

1. Geben Sie Ihre Website-URL ein.

   ![](assets/image2015-1-19-17-3a12-3a39.png)

1. Erstellen Sie Ihr Anzeigen-Set. Wählen Sie in der Liste der von Ihnen erstellten Zielgruppen eine benutzerdefinierte Zielgruppe aus, z. B. „Bildungsindustrie“.

   ![](assets/image2015-1-19-17-3a18-3a13.png)

1. Wählen Sie alle anderen Anzeigenset-Optionen aus, legen Sie Ihr Budget fest und definieren Sie Ihre Werbe-Kreativen.

   ![](assets/image2015-1-19-17-3a19-3a25.png)

1. Sie haben nun in [!DNL Facebook] eine personalisierte Remarketing-Kampagne eingerichtet.

>[!MORELIKETHIS]
>
>* [Retargeting mit Web Personalization-Daten](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Personalisiertes Remarketing in Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)
