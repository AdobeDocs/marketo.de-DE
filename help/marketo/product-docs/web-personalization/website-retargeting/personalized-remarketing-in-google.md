---
unique-page-id: 4720810
description: Personalisiertes Remarketing in Google - Marketo-Dokumente - Produktdokumentation
title: Personalisiertes Remarketing in Google
exl-id: cc733f43-161d-41e4-afdf-8b5217700810
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Personalisiertes Remarketing in Google {#personalized-remarketing-in-google}

Mit personalisiertem Remarketing können Sie mithilfe von RTP-Daten und der Leistungsfähigkeit von Google Analytics mit dem Google Display Network erneut mit Ihren Benutzern interagieren.

>[!PREREQUISITES]
>
>* Führen Sie die [Retargeting mit Web-Personalisierungsdaten](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md) Konfiguration
>* Überprüfen [Hilfe zum Remarketing mit Google Analytics](https://support.google.com/analytics/topic/2611283?hl=en&amp;ref_topic=3413645) Dokumentation.

## Erstellen einer Remarketing-Zielgruppe in Google {#creating-a-remarketing-audience-in-google}

1. Melden Sie sich bei Ihren Google Analytics an. Klicks **Admin**, **Konto**, **Eigenschaft**. Klicken Sie auf **Zielgruppendefinitionen** und **Zielgruppen**.

   ![](assets/remarketing-ga-screenshots.jpg)

1. Klicks **+Neue Zielgruppe**.

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **Link-Konfiguration**: Link zu Ihrem Google Adwords -Konto. **Zielgruppe definieren**: Klicken **Neu erstellen**.

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. Klicken Sie im Audience Builder auf **Sequenzen** und **RTP-Daten suchen** unter &quot;Benutzerdefinierte Dimensionen&quot;, &quot;Benutzerdefinierte Variablen&quot;, &quot;Ereignisse&quot;.

>[!TIP]
>
>Wie finden Sie die RTP-Daten in Analytics, um Ihre Zielgruppe zu erstellen?
>
>In Google Analytics:
>
>* Benutzerdefinierte Variablen: Organisation, Branche
>* Ereigniskategorie: Segment, Insight-CTA, RTP-Remarketing
>* Ereignisbezeichnung: Segmentname, Kampagnenname, Segmentierter Zielgruppenname
>
>In Google Universal Analytics:
>
>* Benutzerdefinierte Dimensionen: Unternehmen, Branche, Kategorie (Fortune 500,1000, Global 2000), Gruppe (Enterprise, SMB), ABM-Liste (Namenskontenliste)
>* Ereigniskategorie: RTP-Segment, RTP-Kampagne RTP-Remarketing
>* Ereignisbezeichnung: Segmentname, Kampagnenname, Segmentierter Zielgruppenname

**Beispiel einer Remarketing-Zielgruppe aus segmentierten RTP-Zielgruppendaten**

1. Klicks **Sequenzen.**
1. Auswählen **Ereignisbezeichnung.**
1. Eingabe **Name der segmentierten Zielgruppe** (wie in RTP angezeigt).
1. Klicks **Anwenden**.

![](assets/image2015-2-10-14-3a51-3a43.png)

**Beispiel einer Zielgruppe aus RTP-Branchendaten**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. Klicks **Sequenzen**.
1. Auswählen **RTP-Branche**.
1. Eingabe **Name der Branche** (Beispiel: Finanzdienstleistungen, Bildung...).
1. Klicks **Anwenden**.
1. Geben Sie eine **Zielgruppenname**. Klicks **Speichern**.

![](assets/image2015-1-15-18-3a29-3a16.png)

## Erstellen einer Remarketing-Anzeigenkampagne in Google Adwords {#create-a-remarketing-ad-campaign-in-google-adwords}

1. Anmelden bei **Google Adwords**. Klicken Sie auf **Kampagnen** auswählen **Nur Netzwerk anzeigen**.

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. Eingabe **Kampagnenname**, Auswahl **Typ Remarketing**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. Eingabe **Anzeigengruppenname,** enter **Verbessertes CPC**, Auswahl **Remarketing-Liste**.

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. Klicken Sie auf Speichern und fahren Sie fort.
1. Fügen Sie Ihre Bild- oder Textanzeige hinzu und starten Sie Ihre Remarketing-Kampagne.

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!MORELIKETHIS]
>
>* [Retargeting mit Web-Personalisierungsdaten](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Personalisiertes Remarketing in Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)
