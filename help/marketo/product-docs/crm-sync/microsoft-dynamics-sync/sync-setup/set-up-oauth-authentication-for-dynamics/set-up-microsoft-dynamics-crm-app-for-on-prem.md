---
description: Einrichten der Microsoft Dynamics CRM-App für On-Prem - Marketing Docs - Produktdokumentation
title: Einrichten der Microsoft Dynamics CRM-App für On-Prem
translation-type: tm+mt
source-git-commit: 9f88e7cebc5e9d0d4491d65d332ccfdd9a31c395
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---


# Einrichten der Microsoft Dynamics CRM-App für On-prem {#set-up-microsoft-dynamics-crm-app-for-on-prem}

Die Client-ID/geheime Client-Einrichtung in Marketing kann für On-Prem mit AD FS (ver. Mai 2016 oder höher). Bei älteren Versionen von On-prem wenden Sie sich bitte an [Marketing Support](https://nation.marketo.com/t5/Support/ct-p/Support), um die Authentifizierungsmethode zu ändern, sodass sie nur auf Benutzer-ID und Kennwort basiert.

## Microsoft Dynamics CRM-App {#set-up-microsoft-dynamics-crm-app} einrichten

Führen Sie die Schritte in [diesem Microsoft-Artikel](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/development/enabling-oauth-confidential-clients-with-ad-fs#create-an-application-group-in-ad-fs-2016-or-later) aus.

Wenn Sie fertig sind, ist der nächste Schritt **Geben Sie die Dynamics CRM generierte Client-ID und Geheimnis in Marketo** ein.

## Geben Sie die Dynamics CRM-generierte Client-ID und den geheimen Schlüssel in Marketo ein. {#enter-the-dynamics-crm-generated-client-id-and-secret-into-marketo}

Die folgenden Schritte gelten für Online- und On-Prem-Versionen.

1. Klicken Sie in Marketo auf **Admin**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-1.png)

1. Klicken Sie auf **Microsoft Dynamics**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-2.png)

1. Klicken Sie auf **Synchronisierung deaktivieren**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-3.png)

1. Klicken Sie neben Berechtigungen auf **Bearbeiten**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-4.png)

1. Geben Sie die zuvor abgerufenen **Client-ID** und **Client-geheim** ein und drücken Sie die Taste **Speichern**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-5.png)

1. Klicken Sie auf **Synchronisierungseinstellungen überprüfen**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-6.png)

1. Klicken Sie auf **Weiter**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-7.png)

1. Sie sollten alle grünen Häkchen sehen. Klicken Sie auf **Schließen**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-8.png)

   >[!NOTE]
   >
   >Wenn unter den grünen Häkchen ein rotes X angezeigt wird, finden Sie in [diesem Artikel](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) Korrekturoptionen.

1. Klicken Sie auf **Synchronisierung aktivieren**.

   ![](assets/set-up-microsoft-dynamics-crm-app-for-on-prem-9.png)

Und das ist es!
