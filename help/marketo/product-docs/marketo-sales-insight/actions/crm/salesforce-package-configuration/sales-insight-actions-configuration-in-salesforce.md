---
description: Konfiguration von Sales Insight-Aktionen in Salesforce - Marketo-Dokumente - Produktdokumentation
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
>* [Installieren](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) oder [Aktualisieren](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) Sales Insight-Paket in Ihrer Salesforce-Instanz
>* [Konfigurieren von Marketo Sales Insight in Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

## Neue Remote-Site in Salesforce hinzufügen {#add-new-remote-site-in-salesforce}

1. Klicken Sie in Salesforce auf **Setup**.

   ![](assets/msi-actions-configuration-in-salesforce-1.png)

1. Suchen Sie nach „Remote Site“ und wählen Sie **Remote Site Settings**.
   ![](assets/msi-actions-configuration-in-salesforce-2.png)

1. Klicken Sie auf **Neue Remote-Site**.

   ![](assets/msi-actions-configuration-in-salesforce-3.png)

1. Geben Sie den Namen der Remote-Site ein (es kann sich um „MarketoSalesInsight1“ handeln). Geben Sie den URL-`https://ims-na1.adobelogin.com` der Remote-Site ein und klicken Sie auf **Speichern**.

   ![](assets/msi-actions-configuration-in-salesforce-4.png)

1. Klicken Sie erneut **Neue Remote-Site**.

   ![](assets/msi-actions-configuration-in-salesforce-4a.png)

1. Geben Sie den Namen der Remote-Site ein (es kann sich um „MarketoSalesInsight2“ handeln). Geben Sie die URL-`https://mkto-sales-connect.adobe.io` der Remote-Site ein und klicken Sie auf **Speichern**.

## Aktivieren von Sales Insight-Aktionen im gesamten CRM {#enabling-sales-insight-actions-across-the-crm}

1. Klicken Sie in Salesforce auf die Registerkarte **Marketo Sales Insight Config** .

   ![](assets/msi-actions-configuration-in-salesforce-5.png)

   >[!NOTE]
   >
   >Wenn &quot;Marketo Sales Insight Config“ nicht in der oberen Leiste angezeigt wird, klicken Sie auf das **+** und suchen Sie es auf allen Registerkarten.

1. Aktivieren Sie **Kontrollkästchen MSI** Aktionen aktivieren .

   ![](assets/msi-actions-configuration-in-salesforce-6.png)

1. Geben Sie den API-Geheimschlüssel ein.

   ![](assets/msi-actions-configuration-in-salesforce-7.png)

   >[!NOTE]
   >
   >Wenn Sie Ihren API-Geheimschlüssel nicht zur Hand haben, können Sie ihn finden, indem Sie die Schritte in [diesem Artikel) ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md).

1. Klicken Sie auf **Speichern**, wenn Sie fertig sind.

Dadurch werden automatisch alle im Artikel Funktionsübersicht beschriebenen Funktionen für MSI-Aktionen aktiviert.

>[!NOTE]
>
>Sie können alle MSI-Aktionsfunktionen deaktivieren, indem Sie einfach das Kontrollkästchen „MSI-Aktionen aktivieren“ deaktivieren.

## MSI-Governance-Aktionen {#msi-actions-governance}

1. Sie können Verkaufskampagnen und/oder die Registerkarte Aufgabe im nächsten Abschnitt deaktivieren. Dies gilt für Lead-, Kontakt-, Konto- und Opportunity-Panels.

   ![](assets/msi-actions-configuration-in-salesforce-8.png)

1. Sie können MSI-Aktionen deaktivieren, indem Sie die entsprechenden Funktionen in den Aktionseinstellungen deaktivieren.

   ![](assets/msi-actions-configuration-in-salesforce-9.png)

>[!NOTE]
>
>Die Governance-Einstellungen gelten für alle MSI-Benutzer.
