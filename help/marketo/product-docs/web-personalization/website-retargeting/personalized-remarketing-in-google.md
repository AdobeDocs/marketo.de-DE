---
unique-page-id: 4720810
description: Personalisiertes Remarketing in Google - Marketo-Dokumente - Produktdokumentation
title: Personalisiertes Remarketing in Google
exl-id: cc733f43-161d-41e4-afdf-8b5217700810
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 4%

---

# Personalisiertes Remarketing in Google {#personalized-remarketing-in-google}

Personalisiertes Remarketing ermöglicht es Ihnen, mit Ihren Benutzenden erneut über RTP-Daten und die Leistungsfähigkeit von Google Analytics mit der Reichweite des Google Display Network zu interagieren.

>[!PREREQUISITES]
>
>* Abschließen der Konfiguration [Retargeting mit  [!DNL Web Personalization] Data](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* Google Analytics Lesen Sie [&#x200B; Dokumentation zu Remarketing mit &#x200B;](https://support.google.com/analytics/topic/2611283?hl=en&ref_topic=3413645) Hilfe.

## Erstellen einer Remarketing-Zielgruppe in Google {#creating-a-remarketing-audience-in-google}

1. Melden Sie sich bei Ihrer Google Analytics an. Klicken Sie auf **[!UICONTROL Admin]**, **[!UICONTROL Account]**, **[!UICONTROL property]**. Klicken Sie auf **[!UICONTROL Zielgruppendefinitionen]** und **[!UICONTROL Zielgruppen]**.

   ![](assets/remarketing-ga-screenshots.jpg)

1. Klicken Sie auf **[!UICONTROL +Neue Zielgruppe]**.

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **[!UICONTROL Link-Konfiguration]**: Verknüpfung zu Ihrem [!DNL Google Adwords]. **[!UICONTROL Zielgruppe definieren]**: Klicken Sie auf **[!UICONTROL Neu erstellen]**.

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. Klicken Sie in Audience Builder auf **[!UICONTROL Sequenzen]** und **[!UICONTROL Suchen der RTP-Daten]** unter [!UICONTROL Benutzerdefinierte Dimensionen], [!UICONTROL UICONTROL [ !]Benutzerdefinierte -Variablen], [!UICONTROL Ereignisse].

>[!TIP]
>
>Wie finde ich die RTP-Daten in Analytics, um Ihre Audience zu erstellen?
>
>In Google Analytics:
>
>* Benutzerdefinierte Variablen: Organisation, Branche
>* Ereigniskategorie: Segment, InsightsA-CTA, RTP-Remarketing
>* Ereignisbezeichnung: Segmentname, Kampagnenname, Name der segmentierten Zielgruppe
>
>In Google Universal Analytics:
>
>* Benutzerdefinierte Dimensionen: Organisation, Branche, Kategorie (Fortune 500.1000, Global 2000), Gruppe (Unternehmen, KMU), ABM-Liste (benannte Kontenliste)
>* Ereigniskategorie: RTP-Segment, RTP-Kampagne RTP-Remarketing
>* Ereignisbezeichnung: Segmentname, Kampagnenname, Name der segmentierten Zielgruppe

**Beispiel einer Remarketing-Zielgruppe aus segmentierten RTP-Zielgruppendaten**

1. Klicken Sie auf **[!UICONTROL Sequenzen].**
1. Wählen Sie **[!UICONTROL Ereignisbeschriftung].**
1. Geben Sie **[!UICONTROL Name der segmentierten Zielgruppe]** ein (wie in RTP angezeigt).
1. Klicken Sie auf **[!UICONTROL Übernehmen]**.

![](assets/image2015-2-10-14-3a51-3a43.png)

**Beispiel einer Zielgruppe aus RTP-Branchendaten**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. Klicken Sie auf **[!UICONTROL Sequenzen]**.
1. Wählen Sie **[!UICONTROL RTP-Industry]** aus.
1. Geben Sie **Name der Branche** ein (z. B. [!UICONTROL Finanzdienstleistungen], [!UICONTROL Bildung]…).
1. Klicken Sie auf **[!UICONTROL Übernehmen]**.
1. Geben Sie einen **[!UICONTROL Zielgruppennamen]** ein. Klicken Sie auf **[!UICONTROL Speichern]**.

![](assets/image2015-1-15-18-3a29-3a16.png)

## Erstellen einer Remarketing-Anzeigenkampagne in [!DNL Google Adwords] {#create-a-remarketing-ad-campaign-in-google-adwords}

1. Beim **[!DNL Google Adwords]** anmelden. Klicken Sie auf **[!UICONTROL Kampagnen]** und wählen Sie **[!UICONTROL Nur Netzwerk anzeigen]**.

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. Geben Sie **[!UICONTROL Kampagnennamen]** ein und wählen Sie **[!UICONTROL Typ Remarketing].**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. Geben Sie **[!UICONTROL Anzeigengruppenname] ein** geben Sie **[!UICONTROL Enhanced CPC]** ein und wählen Sie **[!UICONTROL Remarketing-Liste]**.

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. Klicken Sie auf **[!UICONTROL Speichern]** und fortfahren.
1. Fügen Sie Ihre Bild- oder Textanzeige hinzu und starten Sie Ihre Remarketing-Kampagne.

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!MORELIKETHIS]
>
>* [Retargeting mit [!DNL Web Personalization] Daten](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Personalisiertes Remarketing in [!DNL Facebook]](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)
