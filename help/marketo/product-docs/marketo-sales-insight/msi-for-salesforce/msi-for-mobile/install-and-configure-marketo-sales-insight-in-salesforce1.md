---
unique-page-id: 7511512
description: Installieren und Konfigurieren von MarketingTo Sales Insight in Salesforce1 - Marketing Docs - Produktdokumentation
title: Installieren und Konfigurieren von MarketingTo Sales Insight in Salesforce1
translation-type: tm+mt
source-git-commit: 972cf9769ac751d9abfd5665975703dcd07930f0
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---


# Installieren und Konfigurieren von Marketo Sales Insight in Salesforce1 {#install-and-configure-marketo-sales-insight-in-salesforce}

>[!NOTE]
>
>Bestehende Kunden, bitte [Upgrade Ihres MSI-Pakets](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md), bevor Sie fortfahren!

>[!PREREQUISITES]
>
>Wenn Sie Salesforce Enterprise/Unlimited haben:
>
>* [Schritt 1 von 3: hinzufügen Marketo-Felder an Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Schritt 2 von 3: Erstellen eines Salesforce-Benutzers für Marketing (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Schritt 3 von 3: Connect Marketing und Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
>* [Konfigurieren von MarketingTo Sales Insight in Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

>
>
Wenn Sie Salesforce Professional haben:
>
>* [Konfigurieren von Marketo Sales Insight in Salesforce Professional Edition](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)

>



>[!NOTE]
>
>Marketo Sales Insight in Salesforce1 beinhaltet: Beste Wetten, Interessentenfeed, interessante Momente und Hinzufügen zur Kampagne von Marketo.

## Salesforce1 Mobile App {#enable-the-salesforce1-mobile-app} aktivieren

1. Klicken Sie auf **Setup** und dann **Mobile Administration**.

   ![](assets/image2015-4-21-15-3a29-3a22.png)

1. Klicken Sie auf **Salesforce1**.

   ![](assets/image2015-4-21-15-3a30-3a51.png)

1. Klicken Sie auf **Salesforce1 Settings**.

   ![](assets/image2015-4-21-15-3a32-3a21.png)

1. Klicken Sie auf **Aktivieren Sie die mobile Browser-App Salesforce1**.

   ![](assets/image2015-4-21-15-3a34-3a27.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/image2015-4-21-15-3a42-3a48.png)

1. Wählen Sie **Mobile Administration**.

   ![](assets/image2015-4-22-11-3a10-3a14.png)

1. Klicken Sie auf **Mobiles Navigationsmenü verwalten**.

   ![](assets/image2015-4-22-11-3a13-3a10.png)

1. Wählen Sie **Marketo** und **Hinzufügen** aus, um die Menüelemente **Ausgewählte** anzuzeigen.

   ![](assets/image2015-4-22-14-3a55-3a37.png)

1. Wählen Sie **Marketo**, verschieben Sie es **Nach oben** in den gewünschten Bereich und klicken Sie auf **Speichern**.

   ![](assets/image2015-4-22-17-3a20-3a56.png)

## Veraltete Markierung für benutzerdefiniertes Objekt ausblenden {#hide-outdated-marketo-custom-object}

1. Klicken Sie auf **Setup**.

   ![](assets/image2015-4-22-15-3a13-3a48.png)

1. Wählen Sie **Benutzer verwalten**.

   ![](assets/image2015-5-5-11-3a13-3a45.png)

1. Wählen Sie **Profil**.

   ![](assets/image2015-5-5-11-3a15-3a21.png)

1. Klicken Sie auf **Bearbeiten** der gewünschten Profil.

   ![](assets/image2015-5-5-13-3a51-3a36.png)

1. Wählen Sie unter **Tab-Einstellungen** _first_ **Marketo**.

   ![](assets/image2015-5-5-13-3a55-3a36.png)

1. Wählen Sie **Ausgeblendetes Register**.

   ![](assets/image2015-5-5-14-3a2-3a29.png)

   >[!NOTE]
   >
   >Achten Sie darauf, die Registerkarte Marketo für alle gewünschten Profil auszublenden!

## Tabs {#customize-tabs} anpassen

1. Klicken Sie auf **+**.

   ![](assets/image2015-4-22-17-3a14-3a49.png)

1. Klicken Sie auf **Meine Registerkarten anpassen**.

   ![](assets/image2015-4-22-17-3a16-3a22.png)

1. Wählen Sie **Marketo** und **Hinzufügen** auf den ausgewählten Registerkarten aus.

   ![](assets/image2015-4-22-17-3a17-3a15.png)

1. Wählen Sie **Marketo**, verschieben Sie es **Nach oben** in den gewünschten Bereich und klicken Sie auf **Speichern**.

   ![](assets/image2015-4-22-18-3a29-3a47.png)

## Seitenlayouts anpassen {#customize-page-layouts}

1. Klicken Sie auf **Setup**.

   ![](assets/image2015-4-22-17-3a26-3a56.png)

1. Klicken Sie auf **Setup**, geben Sie **Seitenlayouts** ein und klicken Sie unter &quot;Interessenten&quot;auf **Seitenlayouts**.

   >[!NOTE]
   >
   >Wiederholen Sie die Schritte für jedes Seitenlayout, das Ihr Unternehmen verwendet (Marketing, Vertrieb usw.). für Kontakt-, Konto- und Opportunity-Objekte.

   ![](assets/image2015-4-22-17-3a34-3a33.png)

1. Klicken Sie auf **Bearbeiten**, um Änderungen am Interessentenlayout vorzunehmen.

   ![](assets/image2015-4-22-17-3a44-3a0.png)

1. Klicken Sie auf **Visualforce-Seiten** und ziehen Sie dann **Lead Mobile** in den Abschnitt &quot;Mobilkarten&quot;.

   ![](assets/image2015-4-22-17-3a49-3a37.png)

1. Ändern Sie die Höhe in 66 und klicken Sie auf **OK**.

   ![](assets/image2015-4-22-17-3a52-3a15.png)

1. Klicken Sie auf **Felder** und ziehen Sie **Hinzufügen auf Marketo-Kampagne** in den Abschnitt **Marketingto Sales Insight**.

   ![](assets/configure-step-6.png)

   >[!TIP]
   >
   >Geben Sie &quot;Hinzufügen zu&quot;in die Schnellsuche ein, um die Hinzufügen zur Kampagne von Marketo leicht zu finden.

1. Klicken Sie auf **Speichern**.

   ![](assets/image2015-4-22-18-3a1-3a56.png)

Phew! Sie sind endlich fertig mit der Installation von Marketo Sales Insight für Salesforce1! Geh voraus und gib dir einen Pat auf die Rückseite.

>[!MORELIKETHIS]
>
>* [Beste Einsätze in Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/best-bets-in-salesforce1.md)
>* [Interessante Momente in Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/interesting-moments-in-salesforce1.md)
>* [Senden von E-Mail-Nachrichten und Kampagnen- und Watchlist-Aktionen in Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/send-marketo-email-and-campaign-and-watchlist-actions-in-salesforce1.md)

