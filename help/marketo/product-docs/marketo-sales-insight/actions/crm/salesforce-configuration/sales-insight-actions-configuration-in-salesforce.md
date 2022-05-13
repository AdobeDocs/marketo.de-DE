---
description: Konfiguration von Sales Insight-Aktionen in Salesforce - Marketo Docs - Produktdokumentation
title: Konfiguration von Sales Insight-Aktionen in Salesforce
exl-id: 2d842886-3501-4aca-96fb-0d6763ab2b01
source-git-commit: 222b0692998be1fd15dc6465af1da627e1c32683
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Konfiguration von Sales Insight-Aktionen in Salesforce {#sales-insight-actions-configuration-in-salesforce}

>[!PREREQUISITES]
>
>* [Installieren](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) oder [Upgrade](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) Sales Insight-Paket in Ihrer Salesforce-Instanz
>* [Konfigurieren von Marketo Sales Insight in Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)


## Neue Remote-Site in Salesforce hinzufügen {#add-new-remote-site-in-salesforce}

1. Klicken Sie in Salesforce auf **Einrichtung**.

   ![](assets/msi-actions-configuration-in-salesforce-1.png)

1. Suchen Sie nach &quot;Remote-Site&quot;und wählen Sie **Remote Site Settings**.
   ![](assets/msi-actions-configuration-in-salesforce-2.png)

1. Klicken **Neue Remote-Site**.

   ![](assets/msi-actions-configuration-in-salesforce-3.png)

1. Geben Sie den Remote-Site-Namen ein (z. B. &quot;MarketoSalesInsight&quot;). Geben Sie die Remote-Site-URL ein (https://ims-na1-stg1.adobelogin.com) und klicken Sie auf **Speichern**.

   ![](assets/msi-actions-configuration-in-salesforce-4.png)

## Aktivierung von Sales Insight-Aktionen im gesamten CRM {#enabling-sales-insight-actions-across-the-crm}

1. Klicken Sie in Salesforce auf die **Marketo Sales Insight-Konfiguration** Registerkarte.

   ![](assets/msi-actions-configuration-in-salesforce-5.png)

   >[!NOTE]
   >
   >Wenn Sie &quot;Marketo Sales Insight-Konfiguration&quot;nicht in Ihrer oberen Leiste sehen, klicken Sie auf die Schaltfläche **+** signieren und finden Sie es unter Alle Registerkarten .

1. Wählen Sie die **MSI-Aktionen aktivieren** aktivieren.

   ![](assets/msi-actions-configuration-in-salesforce-6.png)

1. Geben Sie den geheimen API-Schlüssel ein.

   ![](assets/msi-actions-configuration-in-salesforce-7.png)

   >[!NOTE]
   >
   >Wenn Sie Ihren API-Sicherheitsschlüssel nicht zur Hand haben, führen Sie die Schritte unter [diesem Artikel](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md).

1. Klicken **Speichern** wann geschehen.

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
