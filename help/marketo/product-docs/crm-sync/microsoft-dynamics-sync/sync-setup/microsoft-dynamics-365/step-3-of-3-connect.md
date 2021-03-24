---
unique-page-id: 3571830
description: Schritt 3 von 3 - Verbinden von Microsoft Dynamics mit Marketo (Online) - Marketing Docs - Produktdokumentation
title: Schritt 3 von 3 - Verbinden von Microsoft Dynamics mit Marketo (Online)
translation-type: tm+mt
source-git-commit: ed9399396c82a3b2fb93c83ffdaa1dc7b0827306
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---


# Schritt 3 von 3: Verbinden von Microsoft Dynamics mit Marketo (Online) {#step-of-connect-microsoft-dynamics-with-marketo-online}

Dies ist der letzte Schritt der Synchronisierung. Wir sind fast da!

>[!PREREQUISITES]
>
>* [Schritt 1 von 3: Installieren der Marketing Solution (Online)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md)
>* [Schritt 2 von 3: Marketo Sync User in Dynamics einrichten](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md)


>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

## Dynamics Sync-Benutzerinformationen eingeben {#enter-dynamics-sync-user-information}

1. Melden Sie sich bei Marketing an und klicken Sie auf **Admin**.

   ![](assets/login-admin.png)

1. Klicken Sie auf **CRM**.

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. Wählen Sie **Microsoft**.

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. Klicken Sie in **Schritt 1 auf** Bearbeiten **: Geben Sie Anmeldeinformationen** ein.

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >Vergewissern Sie sich bitte, dass Ihre Anmeldeinformationen korrekt sind, da wir die nachfolgenden Änderungen des Schemas nach der Übermittlung nicht wiederherstellen können. Wenn falsche Anmeldeinformationen gespeichert werden, müssen Sie ein neues Marketing-Abonnement erhalten.

1. Geben Sie **Benutzername**, **Kennwort** und Microsoft Dynamics **URL** ein. Klicken Sie abschließend auf **Speichern**.

   ![](assets/five-1.png)

   >[!NOTE]
   >
   >* Wenn Ihr Marketo vor Oktober 2020 bereitgestellt wurde, sind die optionalen Felder Client-ID und Geheimer Schlüssel optional. Andernfalls sind sie obligatorisch. Das Abrufen dieser Informationen hängt von der verwendeten MSD-Version ab.
   >* Der Benutzername in Marketing muss mit dem Benutzernamen für den Synchronisierungsbenutzer in CRM übereinstimmen. Das Format kann &quot;`user@domain.com`&quot;oder &quot;DOMAIN\user&quot;lauten.
   >* Wenn Sie die URL nicht kennen, [erfahren Sie, wie Sie sie hier finden.](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md)


## Zu synchronisierende Felder auswählen{#select-fields-to-sync}

1. Klicken Sie in **Schritt 2 auf** Bearbeiten **: Wählen Sie die zu synchronisierenden Felder aus.**

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Wählen Sie die Felder aus, die Sie mit Marketo synchronisieren möchten, damit sie vorausgewählt werden. Klicken Sie auf **Speichern**.

   ![](assets/image2016-8-25-15-3a6-3a11.png)

>[!NOTE]
>
>Marketo speichert einen Verweis auf die zu synchronisierenden Felder. Wenn Sie ein Feld in Dynamics löschen, wird empfohlen, dies mit [sync deaktiviert](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md) zu tun. Aktualisieren Sie anschließend das Schema in Marketo, indem Sie die Felder [Zu synchronisierende Felder auswählen ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md) bearbeiten und speichern.

## Synchronisieren von Feldern für einen benutzerspezifischen Filter {#sync-fields-for-a-custom-filter}

Wenn Sie einen benutzerspezifischen Filter erstellt haben, sollten Sie unbedingt einsteigen und die neuen Felder auswählen, die mit Marketo synchronisiert werden sollen.

1. Gehen Sie zu Admin und wählen Sie **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicken Sie unter &quot;Details zur Feldsynchronisierung&quot;auf **Bearbeiten**.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Blättern Sie nach unten zum Feld und überprüfen Sie es. Der tatsächliche Name muss new_synctomkto sein, der Anzeigename kann jedoch beliebig sein. Klicken Sie auf **Speichern**.

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## Synchronisierung aktivieren {#enable-sync}

1. Klicken Sie in **Schritt 3 auf** Bearbeiten **: Aktivieren Sie die Synchronisierung**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo wird nicht automatisch deduplizieren gegen eine Microsoft Dynamics-Synchronisierung, oder wenn Sie manuell eingeben Personen oder Interessenten.

1. Lesen Sie alles im Popup-Fenster, geben Sie Ihre E-Mail-Adresse ein und klicken Sie auf **Beginn-Synchronisierung**.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. Die erste Synchronisierung kann einige Stunden dauern. Nach Abschluss des Vorgangs erhalten Sie eine E-Mail-Benachrichtigung.

   ![](assets/image2015-3-16-9-3a59-3a51.png)

Exzellente Arbeit!
