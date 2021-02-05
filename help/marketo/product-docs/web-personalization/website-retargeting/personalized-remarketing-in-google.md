---
unique-page-id: 4720810
description: Personalisierte Remarketing in Google - Marketing Docs - Produktdokumentation
title: Personalisierte Remarketing in Google
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---


# Personalisierte Remarketing in Google {#personalized-remarketing-in-google}

Mit personalisierter Remarketing können Sie die Interaktion mit Ihren Benutzern mithilfe von RTP-Daten und der Leistungsfähigkeit der Google Analytics mit der Reichweite des Google Display-Netzwerks fortsetzen.

>[!PREREQUISITES]
>
>* Schließen Sie die Konfiguration [Retargeting mit Web-Personalisierungsdaten](retargeting-with-web-personalization-data.md) ab.
>* Lesen Sie die Dokumentation [Remarketing mit Google Analytics - Hilfe](https://support.google.com/analytics/topic/2611283?hl=en&amp;ref_topic=3413645)

>



## Erstellen einer Remarketing-Audience in Google {#creating-a-remarketing-audience-in-google}

1. Melden Sie sich bei Ihren Google Analytics an. Klicken Sie auf **Admin**, **Konto**, **Eigenschaft**. Klicken Sie auf **Audience Definitionen** und **Audiencen**.

   ![](assets/remarketing-ga-screenshots.jpg)

1. Klicken Sie auf **+Neue Audience**.

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **Linkkonfiguration**: Link zu Ihrem Google Adwords-Konto
1. **Audience** definieren: Klicken Sie auf Neu  **erstellen**.

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. Klicken Sie im Audiencen-Builder auf **Sequenzen** und **Suchen Sie die RTP-Daten** unter Benutzerdefinierte Dimensionen, Benutzerdefinierte Variablen, Ereignis.

>[!TIP]
>
>Wie finden Sie die RTP-Daten in Analytics, um Ihre Audience zu erstellen?
>
>Bei Google Analytics:
>
>* Benutzerdefinierte Variablen: Organisation, Industrie
>* Ereignis-Kategorie: Segment, Insightera-CTA, RTP-Remarketing
>* Ereignis-Beschriftung: Segmentname, Kampagnen-Name, Segmentname der Audience

>
>
In Google Universal Analytics:
>
>* Benutzerspezifische Dimensionen: Unternehmen, Industrie, Kategorie (Fortune 500,1000, Global 2000), Unternehmensgruppe (Enterprise, SMB), ABM-Liste (Liste für benannte Konten)
>* Ereignis-Kategorie: RTP-Segment, RTP-Kampagne RTP-Remarketing
>* Ereignis-Beschriftung: Segmentname, Kampagnen-Name, Segmentname der Audience

>



**Beispiel einer Remarketing-Audience aus RTP-Daten zur segmentierten Audience**

1. Klicken Sie auf **Sequenzen.**
1. Wählen Sie **Ereignis-Beschriftung.**
1. Geben Sie **Name der segmentierten Audience** ein (wie in RTP angezeigt).
1. Klicken Sie auf **Apply**.

![](assets/image2015-2-10-14-3a51-3a43.png)

**Audience von RTP-Branchendaten**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. Klicken Sie auf **Sequenzen**.
1. Wählen Sie** RTP-Industry**.
1. Geben Sie **Name der Branche** ein (z. B. Finanzdienstleistungen, Bildung...)
1. Klicken Sie auf **Apply**.
1. Geben Sie einen **Audiencen-Namen** ein. Klicken Sie auf **Speichern**.

![](assets/image2015-1-15-18-3a29-3a16.png)

## Erstellen einer Remarketing-Anzeigen-Kampagne in Google Adwords {#create-a-remarketing-ad-campaign-in-google-adwords}

1. Melden Sie sich bei **Google Adwords** an. Klicken Sie auf **Kampagnen** und wählen Sie **Nur Netzwerk anzeigen**.

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. Geben Sie **Kampagne Name** ein, wählen Sie **Typ Remarketing.**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. Geben Sie **Anzeigengruppenname,** **Erweiterte CPC** ein, wählen Sie **Remarketing-Liste**.

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. Klicken Sie auf Speichern und fahren Sie fort.
1. hinzufügen Sie Ihre Bild- oder Textanzeige und Beginn Ihrer Remarketing-Kampagne.

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!MORELIKETHIS]
>
>* [Retargeting mit Web-Personalisierungsdaten](retargeting-with-web-personalization-data.md)
>* [Personalisierte Remarketing in Facebook](personalized-remarketing-in-facebook.md)

