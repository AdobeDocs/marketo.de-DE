---
description: Konfiguration von Sales Insight-Aktionen in Salesforce - Marketo Docs - Produktdokumentation
title: Konfiguration von Sales Insight-Aktionen in Salesforce
exl-id: 2d842886-3501-4aca-96fb-0d6763ab2b01
source-git-commit: 544dfc0892016223c1e5976bd8c9d108ade7c984
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 1%

---

# Konfiguration von Sales Insight-Aktionen in Salesforce {#sales-insight-actions-configuration-in-salesforce}

>[!PREREQUISITES]
>
>* [Installieren Sie](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) oder [Upgrade](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) Sales Insight-Paket in Ihrer Salesforce-Instanz
>* [Konfigurieren von Marketo Sales Insight in Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

## Neue Remote-Site in Salesforce hinzufügen {#add-new-remote-site-in-salesforce}

1. Klicken Sie in Salesforce auf **Einrichtung**.

   ![](assets/msi-actions-configuration-in-salesforce-1.png)

1. Suchen Sie nach &quot;Remote-Site&quot;und wählen Sie **Remote-Site-Einstellungen**.
   ![](assets/msi-actions-configuration-in-salesforce-2.png)

1. Klicken Sie auf **Neue Remote-Site**.

   ![](assets/msi-actions-configuration-in-salesforce-3.png)

1. Geben Sie den Remote-Site-Namen ein (z. B. &quot;MarketoSalesInsight1&quot;). Geben Sie die Remote-Site-URL `https://ims-na1.adobelogin.com` ein und klicken Sie auf **Speichern**.

   ![](assets/msi-actions-configuration-in-salesforce-4.png)

1. Klicken Sie erneut auf **Neue Remote-Site** .

   ![](assets/msi-actions-configuration-in-salesforce-4a.png)

1. Geben Sie den Remote-Site-Namen ein (z. B. &quot;MarketoSalesInsight2&quot;). Geben Sie die Remote-Site-URL `https://mkto-sales-connect.adobe.io` ein und klicken Sie auf **Speichern**.

## Aktivierung von Sales Insight-Aktionen im gesamten CRM {#enabling-sales-insight-actions-across-the-crm}

1. Klicken Sie in Salesforce auf die Registerkarte **Marketo Sales Insight Config** .

   ![](assets/msi-actions-configuration-in-salesforce-5.png)

   >[!NOTE]
   >
   >Wenn Sie &quot;Marketo Sales Insight-Konfiguration&quot;nicht in Ihrer oberen Leiste sehen, klicken Sie auf das Zeichen **+** und suchen Sie es unter &quot;Alle Registerkarten&quot;.

1. Aktivieren Sie das Kontrollkästchen **MSI-Aktionen aktivieren** .

   ![](assets/msi-actions-configuration-in-salesforce-6.png)

1. Geben Sie den geheimen API-Schlüssel ein.

   ![](assets/msi-actions-configuration-in-salesforce-7.png)

   >[!NOTE]
   >
   >Wenn Sie Ihren API-Sicherheitsschlüssel nicht zur Hand haben, können Sie ihn anhand der Schritte in [diesem Artikel](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md) finden.

1. Klicken Sie auf **Speichern**, wenn Sie fertig sind.

Dadurch werden automatisch alle im Artikel Funktionsübersicht beschriebenen MSI-Aktionen aktiviert.

>[!NOTE]
>
>Sie können alle MSI-Aktionen-Funktionen deaktivieren, indem Sie einfach das Kontrollkästchen &quot;MSI-Aktionen aktivieren&quot;deaktivieren.

## MSI-Actions Governance {#msi-actions-governance}

1. Sie können im nächsten Abschnitt Verkaufskampagnen und/oder die Registerkarte Aufgabe deaktivieren. Dies gilt für Lead-, Kontakt-, Konto- und Opportunity-Bereiche.

   ![](assets/msi-actions-configuration-in-salesforce-8.png)

1. Sie können MSI-Aktionen deaktivieren, indem Sie die entsprechenden Funktionen unter Aktionseinstellungen deaktivieren.

   ![](assets/msi-actions-configuration-in-salesforce-9.png)

>[!NOTE]
>
>Governance-Einstellungen gelten für alle MSI-Benutzer.
