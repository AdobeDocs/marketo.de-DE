---
unique-page-id: 4720796
description: Retargeting mit Web-Personalisierungsdaten - Marketo-Dokumente - Produktdokumentation
title: Retargeting mit Web-Personalisierungsdaten
exl-id: b5af1f84-2061-4d0d-9d1f-2fff9191f028
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Retargeting mit Web-Personalisierungsdaten {#retargeting-with-web-personalization-data}

>[!AVAILABILITY]
>
>Website-Retargeting fällt jetzt unter die Kachel Web-Personalisierung . Wenn Sie nur Retargeting gekauft haben, sehen Sie diese Kachel und greifen Sie auf das Web Personalization-Produkt zu mit **only** Targeting-Funktionen aktiviert. Dadurch erhalten Sie Zugriff auf Kontoeinstellungen, die Retargeting-Seite, Segmente und zusätzliche Tracking-Seiten.

Remarketing richtet sich an potenzielle Kunden, die Ihre Site in der Vergangenheit besucht haben, wobei Display-Werbung darauf basiert, wer sie sind und was sie getan haben. Personalisierte Retargeting zielt auf spezifische Zielgruppen mit relevanten Anzeigen basierend auf der Branche, spezifischen Konten und bekannten Personendaten ab.

Web-Personalisierung hängt derzeit Daten an die folgenden Remarketing-Plattformen an:

* [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)
* [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

Web-Personalisierung sendet die folgenden Daten an die Remarketing-Plattformen, um Zielgruppen zu erstellen und Remarketing-Werbekampagnen durchzuführen:

<table> 
 <tbody> 
  <tr> 
   <th colspan="1">Web-Personalisierungsdaten</th> 
  </tr> 
  <tr> 
   <th><p>Branche</p></th> 
  </tr> 
  <tr> 
   <th><p>Gruppe (Enterprise, SMB)</p></th> 
  </tr> 
  <tr> 
   <th><p>Kategorie (Fortune 500/1000, Global 2000)</p></th> 
  </tr> 
  <tr> 
   <th><p>ABM-Liste (Namenskontenlisten)</p></th> 
  </tr> 
  <tr> 
   <th><p>Segmentierte Zielgruppe (basierend auf Segmenten)</p></th> 
  </tr> 
  <tr> 
   <th><p>Webkampagnen angeklickt</p></th> 
  </tr> 
 </tbody> 
</table>

## Remarketing-Konfiguration {#remarketing-configuration}

1. Navigieren Sie zu **Retargeting**.

   ![](assets/one.png)

   >[!NOTE]
   >
   >Die Retargeting-Konfiguration erfolgt pro Domäne oder Subdomäne. Aktivieren Sie die anderen Domänen, wenn Sie Daten von diesen Domänen an die Retargeting-Plattform senden möchten.

1. Aktivieren Sie Einstellungen für Google Analytics oder Google Universal Analytics pro Domäne.

   >[!NOTE]
   >
   >Sie müssen das Google Retargeting-Tag auf Ihrer Website implementieren lassen.
   >
   >Wenn Sie Ihre Integration mit Web-Personalisierung und Google Analytics bereits eingerichtet haben, müssen Sie diesen Teil nicht bearbeiten, da er unter &quot;Kontoeinstellungen&quot;dieselbe Konfiguration aufweist.

   ![](assets/two.png)

1. Aktivieren Sie die Konfiguration für Facebook. Klicken Sie auf das Facebook-Akkordeon und erweitern Sie es. Klicken Sie auf **on** , um das entsprechende Ereignis und die entsprechenden Daten an den Facebook-Audience Manager zu senden. Klicken **Speichern**.

   >[!NOTE]
   >
   >Sie müssen [Facebook Custom Audience Pixel](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel)installiert, damit diese Funktion funktioniert.

   ![](assets/three.png)

## Erstellen einer segmentierten Zielgruppe {#creating-segmented-audience}

Mit einer segmentierten Zielgruppe können Sie ein vorhandenes Segment als Zielgruppe für Retargeting-Kampagnen auswählen. Wählen Sie beispielsweise die Segmente Bekannte Person aus.

>[!TIP]
>
>Es ist nicht erforderlich, eine segmentierte Zielgruppe für Branchen- oder andere Daten zu erstellen, die bereits über die Domänenkonfiguration gesendet wurden. Es ist am besten, segmentierte Zielgruppen für Segmente zu verwenden, die auf bekannten Personendaten basieren.

1. Klicken **Segmentierte Zielgruppe erstellen**.

   ![](assets/image2015-1-15-16-3a36-3a38.png)

1. Geben Sie den Zielgruppennamen ein, wählen Sie Kanäle aus und wählen Sie Segment aus der Liste der vorhandenen Segmente aus.

   ![](assets/image2015-1-15-16-3a40-3a17.png)

1. Klicken **Speichern**.

   Sie haben nun die Retargeting-Einrichtung in Web-Personalisierung abgeschlossen, sich bei Ihren Retargeting-Plattformen angemeldet, Ihre auf diesen Daten basierenden Audiences erstellt und Ihre Retargeting-Werbekampagnen eingerichtet.
