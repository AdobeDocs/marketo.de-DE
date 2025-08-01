---
unique-page-id: 4720796
description: Retargeting mit Web-Personalization-Daten - Marketo-Dokumente - Produktdokumentation
title: Retargeting mit Web Personalization-Daten
exl-id: b5af1f84-2061-4d0d-9d1f-2fff9191f028
feature: Web Personalization
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 2%

---

# Retargeting mit [!DNL Web Personalization] Daten {#retargeting-with-web-personalization-data}

>[!AVAILABILITY]
>
>Website-Retargeting fällt jetzt unter die Kachel Web Personalization . Wenn Sie nur Retargeting erworben haben, wird diese Kachel angezeigt und Sie können auf das [!DNL Web Personalization] Produkt zugreifen, wobei **Retargeting** Funktionen aktiviert sind. Dadurch erhalten Sie Zugriff auf Kontoeinstellungen, die Retargeting-Seite, Segmente und zusätzliche Tracking-Seiten.

Remarketing zielt auf Interessenten ab, die Ihre Site in der Vergangenheit besucht haben, und zeigt Werbung an, die darauf basiert, wer sie sind und was sie getan haben. Personalisiertes Retargeting richtet sich an bestimmte Zielgruppen mit relevanten Anzeigen, die auf Branchen- und spezifischen Konten sowie auf bekannten Personendaten basieren.

Web Personalization hängt derzeit Daten an die folgenden Remarketing-Plattformen an:

* [Google](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-google.md)
* [Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)

[!DNL Web Personalization] sendet die folgenden Daten an die Remarketing-Plattformen, um Zielgruppen zu erstellen und Remarketing-Werbekampagnen auszuführen:

<table>
 <tbody>
  <tr>
   <th colspan="1">[!DNL Web Personalization] Daten</th>
  </tr>
  <tr>
   <th><p>Branche</p></th>
  </tr>
  <tr>
   <th><p>Gruppe (Unternehmen, KMU)</p></th>
  </tr>
  <tr>
   <th><p>Kategorie (Fortune 500/1000, Global 2000)</p></th>
  </tr>
  <tr>
   <th><p>ABM-Liste (benannte Kontolisten)</p></th>
  </tr>
  <tr>
   <th><p>Segmentierte Zielgruppe (basierend auf Segmenten)</p></th>
  </tr>
  <tr>
   <th><p>Web-Kampagnen angeklickt</p></th>
  </tr>
 </tbody>
</table>

## Remarketing-Konfiguration {#remarketing-configuration}

1. Navigieren Sie zu **[!UICONTROL Retargeting]**.

   ![](assets/one.png)

   >[!NOTE]
   >
   >Die Retargeting-Konfiguration erfolgt pro Domain oder Subdomain. Aktivieren Sie die anderen Domains, wenn Sie Daten von diesen Domains an die Retargeting-Plattform senden möchten.

1. Aktivieren Sie die Einstellungen für Google Analytics oder [!DNL Google Universal Analytics] pro Domain.

   >[!NOTE]
   >
   >Sie müssen das Google Retargeting-Tag auf Ihrer Website implementieren lassen.
   >
   >Wenn Sie Ihre Integration mit Web Personalization und Google Analytics bereits eingerichtet haben, müssen Sie diesen Teil nicht bearbeiten, da es sich um dieselbe Konfiguration unter „Kontoeinstellungen“ handelt.

   ![](assets/two.png)

1. Aktivieren Sie die Konfiguration für Facebook. Klicken Sie auf das Akkordeon [!DNL Facebook] und erweitern Sie es. Klicken Sie auf **[!UICONTROL Ein]**, um das entsprechende Ereignis und die entsprechenden Daten an Facebook Audience Manager zu senden. Klicken Sie auf **[!UICONTROL Speichern]**.

   >[!NOTE]
   >
   >Damit diese Funktion funktioniert, muss [[!DNL Facebook] Benutzerdefiniertes Zielgruppen-](https://developers.facebook.com/docs/ads-for-websites/website-custom-audiences/getting-started#install-the-pixel)) auf Ihrer Website installiert sein.

   ![](assets/three.png)

## Segmentierte Zielgruppe erstellen {#creating-segmented-audience}

Mit einer segmentierten Zielgruppe können Sie ein vorhandenes Segment als Zielgruppe auswählen, die für Retargeting-Kampagnen verwendet werden soll. Beispiel: Auswahl der Segmente „Bekannte Person“.

>[!TIP]
>
>Es ist nicht erforderlich, eine segmentierte Zielgruppe für Branchen- oder andere Daten zu erstellen, die bereits in der Domain-Konfiguration gesendet wurden. Es wird empfohlen, segmentierte Zielgruppen für Segmente zu verwenden, die auf Daten bekannter Personen basieren.

1. Klicken Sie **[!UICONTROL Segmentierte Zielgruppe erstellen]**.

   ![](assets/image2015-1-15-16-3a36-3a38.png)

1. Geben Sie den Zielgruppennamen ein, wählen Sie Kanäle aus und wählen Sie Segment aus der Liste der vorhandenen Segmente aus.

   ![](assets/image2015-1-15-16-3a40-3a17.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Sie haben nun die Retargeting-Einrichtung in [!DNL Web Personalization] abgeschlossen. Melden Sie sich bei Ihren Retargeting-Plattformen an, erstellen Sie Ihre Zielgruppen basierend auf diesen Daten und richten Sie Ihre Retargeting-Anzeigenkampagnen ein.
