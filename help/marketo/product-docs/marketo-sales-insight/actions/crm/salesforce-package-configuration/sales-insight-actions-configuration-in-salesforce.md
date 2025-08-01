---
description: Konfiguration von Sales Insight-Aktionen in Salesforce - Marketo-Dokumente - Produktdokumentation
title: Konfiguration von Sales Insight-Aktionen in Salesforce
exl-id: 2d842886-3501-4aca-96fb-0d6763ab2b01
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 1%

---

# [!DNL Sales Insight Actions] in [!DNL Salesforce] {#sales-insight-actions-configuration-in-salesforce}

>[!PREREQUISITES]
>
>* [Installieren](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) oder [Aktualisieren](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) des Sales Insight-Pakets in Ihrer [!DNL Salesforce]
>* [Konfigurieren von Marketo Sales Insight in [!DNL Salesforce] Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

## Neue Remote-Site in [!DNL Salesforce] hinzufügen {#add-new-remote-site-in-salesforce}

1. Klicken Sie [!DNL Salesforce] auf **[!UICONTROL Setup]**.

   ![](assets/msi-actions-configuration-in-salesforce-1.png)

1. Suchen Sie nach &quot;[!UICONTROL Remote Site] und wählen Sie **[!UICONTROL Remote Site Settings]** aus.
   ![](assets/msi-actions-configuration-in-salesforce-2.png)

1. Klicken Sie auf **[!UICONTROL Neue Remote-Site]**.

   ![](assets/msi-actions-configuration-in-salesforce-3.png)

1. Geben Sie den Namen der Remote-Site ein (es kann sich um „MarketoSalesInsight1“ handeln). Geben Sie den URL-`https://ims-na1.adobelogin.com` der Remote-Site ein und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/msi-actions-configuration-in-salesforce-4.png)

1. Klicken Sie erneut **[!UICONTROL Neue Remote-Site]**.

   ![](assets/msi-actions-configuration-in-salesforce-4a.png)

1. Geben Sie den Namen der Remote-Site ein (es kann sich um „MarketoSalesInsight2“ handeln). Geben Sie die URL-`https://mkto-sales-connect.adobe.io` der Remote-Site ein und klicken Sie auf **[!UICONTROL Speichern]**.

## Aktivieren von [!DNL Sales Insight Actions] im gesamten CRM {#enabling-sales-insight-actions-across-the-crm}

1. Klicken Sie in [!DNL Salesforce] auf die Registerkarte **[!UICONTROL Marketo Sales Insight Config]**.

   ![](assets/msi-actions-configuration-in-salesforce-5.png)

   >[!NOTE]
   >
   >Wenn &quot;[!UICONTROL Marketo Sales Insight Config]&quot; nicht in der oberen Leiste angezeigt wird, klicken Sie auf das **+** und suchen Sie es auf den Registerkarten „Alle“.

1. Aktivieren Sie **[!UICONTROL Kontrollkästchen MSI]** Aktionen aktivieren .

   ![](assets/msi-actions-configuration-in-salesforce-6.png)

1. Geben Sie den [!UICONTROL API-Geheimschlüssel] ein.

   ![](assets/msi-actions-configuration-in-salesforce-7.png)

   >[!NOTE]
   >
   >Wenn Sie Ihren [!UICONTROL API-Geheimschlüssel] nicht zur Hand haben, können Sie ihn finden, indem Sie die Schritte in [diesem Artikel) ](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md).

1. Klicken Sie auf **[!UICONTROL Speichern]**, wenn Sie fertig sind.

Dadurch werden automatisch alle im Artikel Funktionsübersicht beschriebenen Funktionen für MSI-Aktionen aktiviert.

>[!NOTE]
>
>Sie können alle MSI-Aktionsfunktionen deaktivieren, indem Sie einfach das Kontrollkästchen „MSI-Aktionen aktivieren“ deaktivieren.

## MSI-Governance-Aktionen {#msi-actions-governance}

1. Sie können Verkaufskampagnen und/oder die Registerkarte Aufgabe im nächsten Abschnitt deaktivieren. Dies gilt für Lead-, Kontakt-, Konto- und Opportunity-Panels.

   ![](assets/msi-actions-configuration-in-salesforce-8.png)

1. Sie können MSI-Aktionen deaktivieren, indem Sie die entsprechenden Funktionen unter [!UICONTROL Aktionseinstellungen] deaktivieren.

   ![](assets/msi-actions-configuration-in-salesforce-9.png)

>[!NOTE]
>
>Die Governance-Einstellungen gelten für alle MSI-Benutzer.
