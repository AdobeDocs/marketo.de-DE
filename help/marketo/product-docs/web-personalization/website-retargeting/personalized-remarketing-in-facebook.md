---
unique-page-id: 4720917
description: Personalisiertes Remarketing in Facebook - Marketo-Dokumente - Produktdokumentation
title: Personalisiertes Remarketing in Facebook
exl-id: 47636afa-49df-40ba-8948-4f2850467c2f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 6%

---

# Personalisiertes Remarketing in Facebook {#personalized-remarketing-in-facebook}

Mit personalisiertem Remarketing können Sie mit RTP-Daten und der Leistungsfähigkeit von Facebook Remarketing erneut mit Ihren Benutzern interagieren.

>[!PREREQUISITES]
>
>* Führen Sie die [Retargeting mit Web-Personalisierungsdaten](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md) Setup
>* Überprüfen Sie die [](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) [Facebook-Dokumentation zu benutzerdefinierten Zielgruppen](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) und Remarketing.


## Erstellen einer Zielgruppe in Facebook {#creating-an-audience-in-facebook}

1. Navigieren Sie in Facebook zu Ihrem [Registerkarte &quot;Zielgruppe&quot;](https://www.facebook.com/ads/audience_manager) im Anzeigen-Manager.

1. Klicken **Instrumente** und wählen Sie **Zielgruppen**.

   ![](assets/one-1.png)

1. Klicken **Erstellen einer benutzerdefinierten Zielgruppe**.

   ![](assets/two-1.png)

1. Auswählen **Website-Traffic**.

   ![](assets/image2015-1-19-16-3a32-3a2.png)

1. Wählen Sie in der Liste Website-Traffic die Option **Benutzerdefinierte Kombination**.

   ![](assets/image2015-1-19-16-3a33-3a21.png)

1. Wählen Sie in der Liste &quot;Einschließen&quot;die Option **Ereignis**.

   ![](assets/image2015-1-19-16-3a34-3a9.png)

1. Wählen Sie in der Liste &quot;Ereignis&quot;die Option **RTP Remarketing** und wählen Sie einen Parameter aus.

   ![](assets/image2015-1-19-16-3a52-3a29.png)

1. Wählen Sie für dieses Beispiel Branche aus, die enthalten sein soll **Bildungswesen**. Eingabe **Bildungswesen** und bearbeiten **Im letzten** auf 180 Tage. Zielgruppenname eingeben: **Bildungswesen**. Klicken **Zielgruppe erstellen**.

   ![](assets/image2015-1-19-16-3a56-3a15.png)

1. Sie haben jetzt eine neue benutzerdefinierte Zielgruppe mit RTP-Daten in Facebook erstellt.

   ![](assets/image2015-1-19-16-3a59-3a2.png)

## RTP-Datenpunkte in Facebook {#rtp-data-points-in-facebook}

<table> 
 <tbody> 
  <tr> 
   <th>Veranstaltungsname</th> 
   <th> </th> 
  </tr> 
  <tr> 
   <td>RTP Remarketing</td> 
   <td> 
    <div> 
     <table> 
      <tbody> 
       <tr> 
        <th>Parameter</th> 
        <th>Wert </th> 
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
        <td colspan="1"><p>Konzern</p><p>KMU</p></td> 
       </tr> 
       <tr> 
        <td>Branche</td> 
        <td><p>Verteidigung</p><p>Aus- und Weiterbildung</p><p>Finanzdienstleistungen</p><p>Regierung</p><p>Gesundheitswesen, Pharma, Biotech</p><p>Software und Internet</p><p>etc.. (gemäß RTP Industry Options)</p></td> 
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

## Targeting Ihrer Zielgruppe mit einer Anzeige {#target-your-audience-with-an-ad}

Weitere Informationen finden Sie unter [Dokumentation zu facebook](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#target-your-audience).

1. Wechseln Sie zum Anzeigen-Manager, klicken Sie auf **Werbeanzeige erstellen**.

   ![](assets/image2015-1-19-17-3a10-3a19.png)

1. Auswählen **Personen auf Ihre Website schicken** als Ziel Ihrer Kampagne.

   ![](assets/image2015-1-19-17-3a11-3a20.png)

1. Geben Sie Ihre Website-URL ein.

   ![](assets/image2015-1-19-17-3a12-3a39.png)

1. Erstellen Sie Ihr Anzeigenset. Wählen Sie eine benutzerdefinierte Zielgruppe aus der Liste der von Ihnen erstellten Zielgruppen aus, z. B. die Bildungsbranche.

   ![](assets/image2015-1-19-17-3a18-3a13.png)

1. Wählen Sie alle anderen Anzeigenset-Optionen aus, legen Sie Ihr Budget fest und definieren Sie Ihre Anzeigenmotive.

   ![](assets/image2015-1-19-17-3a19-3a25.png)

1. Sie sind nun mit einer personalisierten Remarketing-Kampagne in Facebook eingerichtet.

>[!MORELIKETHIS]
>
>* [Retargeting mit Web-Personalisierungsdaten](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Personalisiertes Remarketing in Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)

