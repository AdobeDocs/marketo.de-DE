---
unique-page-id: 7511512
description: Installieren und Konfigurieren von Marketo Sales Insight in Salesforce1 - Marketo Docs - Produktdokumentation
title: Installieren und Konfigurieren von Marketo Sales Insight in Salesforce1
exl-id: 9f26e90b-3199-4ef8-92bc-95e8bd81f1c5
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# Installieren und Konfigurieren von Marketo Sales Insight in Salesforce1 {#install-and-configure-marketo-sales-insight-in-salesforce}

>[!NOTE]
>
>Bestehende Kunden, bitte [MSI-Paket aktualisieren](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) bevor Sie fortfahren!

>[!PREREQUISITES]
>
>Wenn Sie Salesforce Enterprise/Unlimited haben:
>
>* [Schritt 1 von 3: Hinzufügen von Marketo-Feldern zu Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Schritt 2 von 3: Erstellen eines Salesforce-Benutzers für Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Schritt 3 von 3: Verbinden von Marketo und Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
>* [Konfigurieren von Marketo Sales Insight in Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)
>
>Wenn Sie Salesforce Professional haben:
>
>* [Konfigurieren von Marketo Sales Insight in Salesforce Professional Edition](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)
>

>[!NOTE]
>
>Marketo Sales Insight in Salesforce1 umfasst: Best Bets, Lead-Feed, interessante Momente und Add to Marketo Campaign.

## Salesforce1 Mobile App aktivieren {#enable-the-salesforce1-mobile-app}

1. Klicks **Einrichtung** und dann **Mobile Administration**.

   ![](assets/image2015-4-21-15-3a29-3a22.png)

1. Klicks **Salesforce1**.

   ![](assets/image2015-4-21-15-3a30-3a51.png)

1. Klicks **Salesforce1-Einstellungen**.

   ![](assets/image2015-4-21-15-3a32-3a21.png)

1. Klicks **Mobile Browser-App Salesforce1 aktivieren**.

   ![](assets/image2015-4-21-15-3a34-3a27.png)

1. Klicks **Speichern**.

   ![](assets/image2015-4-21-15-3a42-3a48.png)

1. Auswählen **Mobile Administration**.

   ![](assets/image2015-4-22-11-3a10-3a14.png)

1. Klicks **Navigationsmenü für Mobilgeräte verwalten**.

   ![](assets/image2015-4-22-11-3a13-3a10.png)

1. Auswählen **Marketo** und **Hinzufügen** und **Ausgewählt** Menüeinträgen.

   ![](assets/image2015-4-22-14-3a55-3a37.png)

1. Auswählen **Marketo**, verschieben **up** zu einem gewünschten Bereich hinzu und klicken Sie auf **Speichern**.

   ![](assets/image2015-4-22-17-3a20-3a56.png)

## Veraltetes benutzerdefiniertes Marketo-Objekt ausblenden {#hide-outdated-marketo-custom-object}

1. Klicks **Einrichtung**.

   ![](assets/image2015-4-22-15-3a13-3a48.png)

1. Auswählen **Benutzer verwalten**.

   ![](assets/image2015-5-5-11-3a13-3a45.png)

1. Auswählen **Profile**.

   ![](assets/image2015-5-5-11-3a15-3a21.png)

1. Klicken Sie auf **edit** alle gewünschten Profile.

   ![](assets/image2015-5-5-13-3a51-3a36.png)

1. under **Registerkarteneinstellungen**, wählen Sie die _first_ **Marketo**.

   ![](assets/image2015-5-5-13-3a55-3a36.png)

1. Auswählen **Registerkarte ausgeblendet**.

   ![](assets/image2015-5-5-14-3a2-3a29.png)

   >[!NOTE]
   >
   >Vergewissern Sie sich, dass die Registerkarte Marketo für alle gewünschten Profile ausgeblendet wird!

## Anpassen von Registerkarten {#customize-tabs}

1. Klicken **+**.

   ![](assets/image2015-4-22-17-3a14-3a49.png)

1. Klicks **Benutzerdefinierte Registerkarten**.

   ![](assets/image2015-4-22-17-3a16-3a22.png)

1. Auswählen **Marketo** und **Hinzufügen** auf die ausgewählten Registerkarten.

   ![](assets/image2015-4-22-17-3a17-3a15.png)

1. Auswählen **Marketo**, verschieben **up** zu einem gewünschten Bereich hinzu und klicken Sie auf **Speichern**.

   ![](assets/image2015-4-22-18-3a29-3a47.png)

## Seitenlayouts anpassen {#customize-page-layouts}

1. Klicks **Einrichtung**.

   ![](assets/image2015-4-22-17-3a26-3a56.png)

1. Klicks **Einrichtung**, Typ **Seitenlayouts** und klicken Sie auf **Seitenlayouts** unter &quot;Leads&quot;.

   >[!NOTE]
   >
   >Wiederholen Sie die Schritte für jedes Seitenlayout, das Ihr Unternehmen verwendet (Marketing, Vertrieb usw.). für Kontakt-, Konto- und Opportunity-Objekte.

   ![](assets/image2015-4-22-17-3a34-3a33.png)

1. Klicks **Bearbeiten** , um Änderungen am Lead-Layout vorzunehmen.

   ![](assets/image2015-4-22-17-3a44-3a0.png)

1. Klicks **Visualforce-Seiten** und ziehen Sie **Lead Mobile** in den Bereich Karten für Mobilgeräte .

   ![](assets/image2015-4-22-17-3a49-3a37.png)

1. Ändern Sie die Höhe in 66 und klicken Sie auf **OK**.

   ![](assets/image2015-4-22-17-3a52-3a15.png)

1. Klicks **Felder** und ziehen **Zu Marketo Campaign hinzufügen** der **Marketo Sales Insight** Abschnitt.

   ![](assets/configure-step-6.png)

   >[!TIP]
   >
   >Geben Sie &quot;Hinzufügen zu&quot;in die Schnellsuche ein, um die Suche nach Hinzufügen zu Marketo Campaign zu vereinfachen.

1. Klicks **Speichern**.

   ![](assets/image2015-4-22-18-3a1-3a56.png)

Phew! Sie haben die Installation von Marketo Sales Insight für Salesforce1 abgeschlossen! Mach weiter und gib dir einen PFAD auf den Rücken.

>[!MORELIKETHIS]
>
>* [Beste Betten in Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/best-bets-in-salesforce1.md)
>* [Interessante Momente in Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/interesting-moments-in-salesforce1.md)
>* [Senden von Marketo-E-Mail- und -Campaign- und Watchlist-Aktionen in Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/send-marketo-email-and-campaign-and-watchlist-actions-in-salesforce1.md)
