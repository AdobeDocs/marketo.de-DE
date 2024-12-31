---
unique-page-id: 7511512
description: Installieren und Konfigurieren von Marketo Sales Insight in Salesforce1 - Marketo-Dokumentation - Produktdokumentation
title: Installieren und Konfigurieren von Marketo Sales Insight in Salesforce1
exl-id: 9f26e90b-3199-4ef8-92bc-95e8bd81f1c5
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 1%

---

# Installieren und Konfigurieren von Marketo Sales Insight in Salesforce1 {#install-and-configure-marketo-sales-insight-in-salesforce}

>[!NOTE]
>
>Bestehende Kunden: Bitte [Aktualisieren Sie Ihr MSI-Paket](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) bevor Sie fortfahren!

>[!PREREQUISITES]
>
>Wenn Sie über Salesforce Enterprise/Unlimited verfügen:
>
>* [Schritt 1 von 3: Marketo-Felder zu Salesforce hinzufügen (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Schritt 2 von 3: Erstellen eines Salesforce-Benutzers für Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Schritt 3 von 3: Marketo und Salesforce verbinden (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
>* [Konfigurieren von Marketo Sales Insight in Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)
>
>Wenn Sie über Salesforce Professional verfügen:
>
>* [Konfigurieren von Marketo Sales Insight in Salesforce Professional Edition](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)
>

>[!NOTE]
>
>Marketo Sales Insight in Salesforce1 umfasst: Best Bets, Lead-Feed, Interesting Moments und Add to Marketo Campaign.

## Aktivieren der Salesforce1 Mobile App {#enable-the-salesforce1-mobile-app}

1. Klicken Sie **Setup** und dann **Mobile Administration**.

   ![](assets/image2015-4-21-15-3a29-3a22.png)

1. Klicken Sie auf **Salesforce**.

   ![](assets/image2015-4-21-15-3a30-3a51.png)

1. Klicken Sie auf **Salesforce1-**.

   ![](assets/image2015-4-21-15-3a32-3a21.png)

1. Klicken Sie **Salesforce1-Mobile-Browser-App aktivieren**.

   ![](assets/image2015-4-21-15-3a34-3a27.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/image2015-4-21-15-3a42-3a48.png)

1. Wählen Sie **Mobile Administration** aus.

   ![](assets/image2015-4-22-11-3a10-3a14.png)

1. Klicken Sie **Mobiles Navigationsmenü verwalten**.

   ![](assets/image2015-4-22-11-3a13-3a10.png)

1. Wählen Sie **Marketo** und **Hinzufügen** zu den **Ausgewählt** Menüelementen aus.

   ![](assets/image2015-4-22-14-3a55-3a37.png)

1. Wählen Sie **Marketo** aus, verschieben Sie **nach**) in einen gewünschten Bereich und klicken Sie auf **Speichern**.

   ![](assets/image2015-4-22-17-3a20-3a56.png)

## Veraltetes benutzerdefiniertes Marketo-Objekt ausblenden {#hide-outdated-marketo-custom-object}

1. Klicken Sie **Setup**.

   ![](assets/image2015-4-22-15-3a13-3a48.png)

1. Wählen Sie **Benutzer verwalten** aus.

   ![](assets/image2015-5-5-11-3a13-3a45.png)

1. Wählen Sie **Profile** aus.

   ![](assets/image2015-5-5-11-3a15-3a21.png)

1. Klicken Sie auf **, um** gewünschten Profile zu bearbeiten.

   ![](assets/image2015-5-5-13-3a51-3a36.png)

1. Wählen **unter „Registerkarteneinstellungen** die _erste_ **Marketo** aus.

   ![](assets/image2015-5-5-13-3a55-3a36.png)

1. Wählen Sie **Registerkarte ausgeblendet** aus.

   ![](assets/image2015-5-5-14-3a2-3a29.png)

   >[!NOTE]
   >
   >Stellen Sie sicher, dass Sie die Registerkarte Marketo für alle gewünschten Profile ausblenden!

## Registerkarten anpassen {#customize-tabs}

1. Klicken Sie auf **+**.

   ![](assets/image2015-4-22-17-3a14-3a49.png)

1. Klicken Sie **Meine Registerkarten anpassen**.

   ![](assets/image2015-4-22-17-3a16-3a22.png)

1. Wählen Sie **Marketo** aus und **Sie es** den ausgewählten Registerkarten hinzu.

   ![](assets/image2015-4-22-17-3a17-3a15.png)

1. Wählen Sie **Marketo** aus, verschieben Sie **nach**) in einen gewünschten Bereich und klicken Sie auf **Speichern**.

   ![](assets/image2015-4-22-18-3a29-3a47.png)

## Seiten-Layouts anpassen {#customize-page-layouts}

1. Klicken Sie **Setup**.

   ![](assets/image2015-4-22-17-3a26-3a56.png)

1. Klicken Sie **Setup**, geben Sie **Seitenlayouts** ein, und klicken Sie **Seitenlayouts** unter Leads.

   >[!NOTE]
   >
   >Wiederholen Sie die Schritte für jedes Seiten-Layout, das Ihr Unternehmen (Marketing, Vertrieb usw.) für Objekte des Typs Kontakt, Konto und Opportunity verwendet.

   ![](assets/image2015-4-22-17-3a34-3a33.png)

1. Klicken Sie **Bearbeiten**, um Änderungen am Lead-Layout vorzunehmen.

   ![](assets/image2015-4-22-17-3a44-3a0.png)

1. Klicken Sie auf **VisualForce** Seiten und ziehen Sie **Lead Mobile** in den Abschnitt „Mobile Cards“.

   ![](assets/image2015-4-22-17-3a49-3a37.png)

1. Ändern Sie die Höhe in 66 und klicken Sie auf **OK**.

   ![](assets/image2015-4-22-17-3a52-3a15.png)

1. Klicken Sie auf **Felder** und ziehen Sie **Zu Marketo Campaign hinzufügen** in den Abschnitt **Marketo Sales Insight**.

   ![](assets/configure-step-6.png)

   >[!TIP]
   >
   >Geben Sie in die Schnellsuche „Hinzufügen zu“ ein, damit „Hinzufügen zu Marketo Campaign“ leicht zu finden ist.

1. Klicken Sie auf **Speichern**.

   ![](assets/image2015-4-22-18-3a1-3a56.png)

Puh! Sie haben die Installation von Marketo Sales Insight für Salesforce1 abgeschlossen! Jetzt klopfen Sie sich mal auf die Schulter.

>[!MORELIKETHIS]
>
>* [Beste Wetten in Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/best-bets-in-salesforce1.md)
>* [Interessante Momente in Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/interesting-moments-in-salesforce1.md)
>* [Senden von Marketo-E-Mail- und Kampagnen- und Watchlist-Aktionen in Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/send-marketo-email-and-campaign-and-watchlist-actions-in-salesforce1.md)
