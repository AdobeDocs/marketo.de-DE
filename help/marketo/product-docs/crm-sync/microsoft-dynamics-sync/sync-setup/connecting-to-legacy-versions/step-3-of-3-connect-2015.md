---
unique-page-id: 7504744
description: Installieren von Marketo für Microsoft Dynamics 2015 On-Premises Schritt 3 von 3 - Marketo Docs - Produktdokumentation
title: Installieren von Marketo für Microsoft Dynamics 2015 On-Premises Schritt 3 von 3
exl-id: 054bf725-7a80-4114-8360-2d86e2e33dd7
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 1%

---

# 3. Schritt: Marketo Dynamics verbinden (On-Premise 2015) {#step-of-connect-marketo-dynamics-on-premises-2015}

>[!PREREQUISITES]
>
>* [Installieren von Marketo für Microsoft Dynamics 2015 On-Premises Schritt 1 von 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md)
>* [Installieren von Marketo für Microsoft Dynamics 2015 On-Premises Schritt 2 von 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2015.md)

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

## Benutzerinformationen zur Dynamics Sync eingeben {#enter-dynamics-sync-user-information}

1. Melden Sie sich bei Marketo an und klicken Sie auf **Admin**.

   ![](assets/login-admin.png)

1. Klicks **CRM**.

   ![](assets/image2015-3-16-9-47-34.png)

1. Auswählen **Microsoft**.

   ![](assets/image2015-3-16-9-50-6.png)

1. Klicks **Bearbeiten** in **Schritt 1: Anmeldedaten eingeben**.

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >Stellen Sie sicher, dass Ihre Anmeldedaten korrekt sind, da wir die nachfolgenden Schemaänderungen nach der Übermittlung nicht rückgängig machen können. Wenn falsche Anmeldeinformationen gespeichert werden, müssen Sie ein neues Marketo-Abonnement erhalten.

1. Geben Sie die **Benutzername**, **Passwort** Microsoft Dynamics **URL** und ein **Client-ID/Geheimnis**. Klicks **Speichern** wann geschehen.

   ![](assets/step-3-of-3-5.png)

   >[!NOTE]
   >
   >* Wenn Ihre Marketo vor Oktober 2020 bereitgestellt wurde, sind Client-ID und Geheimnis optionale Felder. Andernfalls sind sie obligatorisch. Das Abrufen dieser Informationen hängt von der verwendeten MSD-Version ab.
   >* Der Benutzername in Marketo muss mit dem Benutzernamen für den Synchronisierungsbenutzer im CRM übereinstimmen. Das Format kann `user@domain.com` oder DOMAIN\user.
   >* Wenn Sie die URL nicht kennen, [Hier erfahren Sie, wie Sie ihn finden](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).

   >[!TIP]
   >
   >Kennt die URL nicht? Wir zeigen Ihnen, wie Sie Ihre [URL des Dynamics-Organisationsdienstes](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) hier.

## Felder für Synchronisierung auswählen {#select-fields-to-sync}

1. Klicks **Bearbeiten** in **Schritt 2: Zu synchronisierende Felder auswählen**.

   ![](assets/image2015-3-16-9-51-28.png)

1. Wählen Sie die Felder aus, die Sie mit Marketo synchronisieren möchten, damit sie vorausgewählt werden. Klicks **Speichern**.

   ![](assets/image2016-8-25-15-3a14-3a28.png)

>[!NOTE]
>
>Marketo speichert einen Verweis auf die zu synchronisierenden Felder. Wenn Sie ein Feld in Dynamics löschen, wird empfohlen, dies mit der [Synchronisieren deaktiviert](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Aktualisieren Sie dann das Schema in Marketo, indem Sie die [Zu synchronisierende Felder auswählen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## Synchronisieren von Feldern für einen benutzerdefinierten Filter {#sync-fields-for-a-custom-filter}

Wenn Sie einen benutzerdefinierten Filter erstellt haben, gehen Sie in und wählen Sie die neuen Felder aus, die mit Marketo synchronisiert werden sollen.

1. Navigieren Sie zu Admin und wählen Sie **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicks **Bearbeiten** in den Details zur Feldsynchronisierung.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Scrollen Sie nach unten zum Feld und überprüfen Sie es. Der tatsächliche Name muss &quot;new_synctomkto&quot;lauten, der Anzeigename kann jedoch beliebig sein. Klicks **Speichern**.

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## Synchronisierung aktivieren {#enable-sync}

1. Klicks **Bearbeiten** in **Schritt 3: Synchronisierung aktivieren**.

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >Marketo deaktiviert die Duplizierung nicht automatisch für eine Microsoft Dynamics-Synchronisation oder wenn Sie Personen manuell eingeben.

1. Alles im Popup lesen, Ihre E-Mail eingeben und auf klicken **Synchronisierung starten**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. Die erste Synchronisation kann einige Stunden dauern. Nach Abschluss des Vorgangs erhalten Sie eine E-Mail-Benachrichtigung.

   ![](assets/image2015-3-16-9-59-51.png)

Exzellente Arbeit!
