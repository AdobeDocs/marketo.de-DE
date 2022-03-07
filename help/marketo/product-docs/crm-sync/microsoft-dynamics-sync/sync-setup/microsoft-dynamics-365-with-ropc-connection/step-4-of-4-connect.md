---
description: 'Schritt 4 von 4: Verbinden der Marketo-Lösung mit Resource Owner Password Control Connection - Marketo Docs - Produktdokumentation'
title: 'Schritt 4 von 4: Verbinden der Marketo-Lösung mit der Resource Owner Password Control Connection'
exl-id: 71a52a3e-f31e-45ee-8196-d536528e42ca
source-git-commit: 3a52db828a9bbf01b617d6e417d078d11ea30fb7
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 2%

---

# Schritt 4 von 4: Verbinden der Marketo-Lösung mit der Kennwortsteuerungsverbindung des Ressourceneigentümers {#step-4-of-4-connect-the-marketo-solution-ropc}

Dies ist der letzte Schritt der Synchronisierung. Sie haben es fast geschafft!

>[!PREREQUISITES]
>
>* [Schritt 1 von 4: Installieren Sie die Marketo-Lösung mit Resource Owner Password Control Connection.](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md)
>* [Schritt 2 von 4: Einrichten der Marketo-Lösung mit Resource Owner Password Control Connection](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)
>* [Schritt 3 von 4: Einrichten der Client App auf MS Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md)


>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

>[!NOTE]
>
>Wenn Sie von der einfachen Authentifizierung auf OAuth aktualisieren, können Sie [diesem Artikel](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md) um die Authentifizierung neu zu konfigurieren.

## Benutzerinformationen zur Dynamics Sync eingeben {#enter-dynamics-sync-user-information}

1. Melden Sie sich bei Marketo an und klicken Sie auf **Admin**.

   ![](assets/login-admin.png)

1. Klicken Sie auf **CRM**.

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. Auswählen **Microsoft**.

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. Klicken **Bearbeiten** in **Schritt 1: Anmeldedaten eingeben**.

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >Stellen Sie sicher, dass Ihre Organisations-URL korrekt ist, da wir die nachfolgenden Schemaänderungen nach der Übermittlung nicht rückgängig machen können. Wenn eine falsche Organisations-URL verwendet wird, müssen Sie ein neues Marketo-Abonnement erhalten. Wenn Sie die URL nicht kennen, [Hier erfahren Sie, wie Sie ihn finden](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).

   >[!NOTE]
   >
   >Bevor Sie neue Anmeldedaten eingeben, können Sie [Validieren Sie sie hier .](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md).

1. Geben Sie die **Benutzername**, **Passwort**, Microsoft Dynamics **URL**, **Client-ID** und **Client Secret**. Klicken **Speichern** wann geschehen.

   ![](assets/step-4-of-4-connect-ropc-5.png)

   >[!NOTE]
   >
   >Der Benutzername in Marketo muss mit dem Benutzernamen für den Synchronisierungsbenutzer im CRM übereinstimmen. Das Format kann `user@domain.com` oder DOMAIN\user.

## Felder für Synchronisierung auswählen {#select-fields-to-sync}

1. Klicken **Bearbeiten** in **Schritt 2: Zu synchronisierende Felder auswählen**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Wählen Sie die Felder aus, die Sie mit Marketo synchronisieren möchten, damit sie vorausgewählt werden. Klicken **Speichern**.

   ![](assets/image2016-8-25-15-3a6-3a11.png)

>[!NOTE]
>
>Marketo speichert einen Verweis auf die zu synchronisierenden Felder. Wenn Sie ein Feld in Dynamics löschen, wird empfohlen, dies mit der [Synchronisieren deaktiviert](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Aktualisieren Sie dann das Schema in Marketo, indem Sie die [Zu synchronisierende Felder auswählen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## Synchronisieren von Feldern für einen benutzerdefinierten Filter {#sync-fields-for-a-custom-filter}

Wenn Sie einen benutzerdefinierten Filter erstellt haben, gehen Sie in und wählen Sie die neuen Felder aus, die mit Marketo synchronisiert werden sollen.

1. Navigieren Sie zu Admin und wählen Sie **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicken **Bearbeiten** in den Details zur Feldsynchronisierung.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Scrollen Sie nach unten zum Feld und überprüfen Sie es. Der tatsächliche Name muss &quot;new_synctomkto&quot;lauten, der Anzeigename kann jedoch beliebig sein. Klicken **Speichern**.

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## Synchronisierung aktivieren {#enable-sync}

1. Klicken **Bearbeiten** in **Schritt 3: Synchronisierung aktivieren**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo deaktiviert die Duplizierung nicht automatisch für eine Microsoft Dynamics-Synchronisation oder wenn Sie Personen oder Leads manuell eingeben.

1. Lesen Sie alles im Popup-Fenster, geben Sie Ihre E-Mail-Adresse ein und klicken Sie auf **Synchronisierung starten**.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. Die erste Synchronisation kann einige Stunden dauern. Nach Abschluss des Vorgangs erhalten Sie eine E-Mail-Benachrichtigung.

   ![](assets/image2015-3-16-9-3a59-3a51.png)

Exzellente Arbeit!

>[!MORELIKETHIS]
>
>[Authentifizierungsmethode für Dynamics neu konfigurieren](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md)