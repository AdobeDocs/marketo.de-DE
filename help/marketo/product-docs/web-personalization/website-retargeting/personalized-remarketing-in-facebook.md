---
unique-page-id: 4720917
description: Personalisierte Remarketing in Facebook - Marketing Docs - Produktdokumentation
title: Personalisierte Remarketing in Facebook
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

---


# Personalisierte Remarketing in Facebook {#personalized-remarketing-in-facebook}

Mit personalisierter Remarketing können Sie mithilfe von RTP-Daten und der Leistungsfähigkeit von Facebook Remarketing wieder mit Ihren Benutzern interagieren.

>[!PREREQUISITES]
>
>* Führen Sie die [Einrichtung zur Retargeting mit Web-Personalisierungsdaten](retargeting-with-web-personalization-data.md) durch
>* Lesen Sie die [](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel) Facebook-Dokumentation zu benutzerdefinierten [](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel)Zielgruppen und Remarketing.

>



## Erstellen einer Audience in Facebook {#creating-an-audience-in-facebook}

1. Gehen Sie in Facebook im Anzeigen-Manager zur Registerkarte &quot; [Audience&quot;](https://www.facebook.com/ads/audience_manager) .
1. Klicken Sie auf **Tools** und wählen Sie **Audiencen** aus.

   ![](assets/one-1.png)

1. Klicken Sie auf Benutzerspezifische Audience **erstellen**.

   ![](assets/two-1.png)

1. Wählen Sie **Website-Traffic**.

   ![](assets/image2015-1-19-16-3a32-3a2.png)

1. Wählen Sie in der Liste Website-Traffic** Benutzerdefinierte Kombination**.

   ![](assets/image2015-1-19-16-3a33-3a21.png)

1. Wählen Sie in der Liste &quot;Einschließen&quot;die Option **Ereignis**.

   ![](assets/image2015-1-19-16-3a34-3a9.png)

1. Wählen Sie in der Liste Ereignis **RTP Remarketing **und wählen Sie einen Parameter aus.

   ![](assets/image2015-1-19-16-3a52-3a29.png)

1. Wählen Sie für dieses Beispiel &quot;Branche&quot;aus, um **Bildung** einzuschließen. Geben Sie **Education** ein und bearbeiten Sie **In der letzten** 180 Tage. Audience eingeben: **Bildungsbranche**. Klicken Sie auf Audience **erstellen**.

   ![](assets/image2015-1-19-16-3a56-3a15.png)

1. Sie haben jetzt eine neue benutzerspezifische Audience mit RTP-Daten in Facebook erstellt.

   ![](assets/image2015-1-19-16-3a59-3a2.png)

## RTP-Datenpunkte in Facebook {#rtp-data-points-in-facebook}

<table> 
 <tbody> 
  <tr> 
   <th>Name des Ereignisses</th> 
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
        <th>Wert</th> 
       </tr> 
       <tr> 
        <td>ABM-Liste</td> 
        <td>(Name der kontogestützten Liste)</td> 
       </tr> 
       <tr> 
        <td colspan="1">Kategorie</td> 
        <td colspan="1"><p>Fortune 500</p><p>Fortune 1000</p><p>Global 2000</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">Gruppe</td> 
        <td colspan="1"><p>Unternehmen</p><p>SMB</p></td> 
       </tr> 
       <tr> 
        <td>Branche</td> 
        <td><p>Verteidigung</p><p>Bildungswesen</p><p>Finanzdienstleistungen</p><p>Regierung</p><p>Gesundheitswesen, Pharma, Biotech</p><p>Software und Internet</p><p>etc... (gemäß RTP Industry Options)</p></td> 
       </tr> 
       <tr> 
        <td colspan="1">Segmentierte Audience</td> 
        <td colspan="1">(Name der segmentierten Audience, die in RTP erstellt wurde)</td> 
       </tr> 
      </tbody> 
     </table> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

## Zielgruppe Ihrer Audience mit einer Anzeige {#target-your-audience-with-an-ad}

Weitere Informationen finden Sie in der Dokumentation zu [Facebook](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#target-your-audience).

1. Gehen Sie zum Anzeigen-Manager und klicken Sie auf **Anzeige** erstellen.

   ![](assets/image2015-1-19-17-3a10-3a19.png)

1. Wählen Sie Personen zu Ihrer Kampagne **senden** aus.

   ![](assets/image2015-1-19-17-3a11-3a20.png)

1. Geben Sie Ihre Website-URL ein.

   ![](assets/image2015-1-19-17-3a12-3a39.png)

1. Erstellen Sie Ihren Anzeigensatz. Wählen Sie eine benutzerdefinierte Audience aus der Liste der von Ihnen erstellten Audiencen, z. B. Bildungsbranche.

   ![](assets/image2015-1-19-17-3a18-3a13.png)

1. Wählen Sie alle anderen Anzeigensatzoptionen aus, legen Sie Ihr Budget fest und definieren Sie Ihre Anzeigenkreativen.

   ![](assets/image2015-1-19-17-3a19-3a25.png)

1. Sie sind jetzt alle mit einer personalisierten Remarketing-Kampagne in Facebook eingerichtet.

>[!NOTE]
>
>**Verwandte Artikel**
>
>* [Retargeting mit Web-Personalisierungsdaten](retargeting-with-web-personalization-data.md)
>* [Personalisierte Remarketing in Google](personalized-remarketing-in-google.md)

>



