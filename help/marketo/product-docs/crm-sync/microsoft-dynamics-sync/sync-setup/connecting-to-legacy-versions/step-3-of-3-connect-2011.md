---
unique-page-id: 3571809
description: 'Schritt 3 von 3: Verbinden von Microsoft Dynamics mit Marketo (On-Premises 2011) - Marketo Docs - Produktdokumentation'
title: 'Schritt 3 von 3: Verbinden von Microsoft Dynamics mit Marketo (On-Premises 2011)'
exl-id: e6a5d49d-025a-4899-9e92-7a4c32086c67
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 1%

---

# Schritt 3: Verbinden von Microsoft Dynamics mit Marketo (On-Premises 2011) {#step-of-connect-microsoft-dynamics-with-marketo-on-premises}

Gut! Wir haben die Lösung installiert und den Synchronisierungsbenutzer konfiguriert. Als Nächstes müssen wir Marketo und Dynamics verbinden.

>[!PREREQUISITES]
>
>* [Schritt 1 von 3: Installieren der Marketo-Lösung (On-Premises 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2011.md)
>* [Schritt 2 von 3: Einrichten des Marketo Sync User in Dynamics (On-Premises 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2011.md)

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

## Benutzerinformationen zur Dynamics Sync eingeben {#enter-dynamics-sync-user-information}

1. Melden Sie sich bei Marketo an und klicken Sie auf **Admin**.

   ![](assets/login-admin.png)

1. Klicken Sie auf **CRM**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Klicks **Microsoft**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Klicks **Bearbeiten** in **Schritt 1: Anmeldedaten eingeben.**

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Stellen Sie sicher, dass Ihre Anmeldedaten korrekt sind, da wir die nachfolgenden Schemaänderungen nach der Übermittlung nicht rückgängig machen können. Wenn falsche Anmeldeinformationen gespeichert werden, müssen Sie ein neues Marketo-Abonnement erhalten.

1. Geben Sie die **Benutzername**, **Passwort** und CRM **URL** Klicken Sie dann auf **Speichern**.

   ![](assets/image2015-4-2-14-3a50-3a7.png)

   >[!NOTE]
   >
   >* Der Benutzername in Marketo muss mit dem Benutzernamen für den Synchronisierungsbenutzer im CRM übereinstimmen. Das Format kann `user@domain.com` oder DOMAIN\user.
   >* Wenn Sie die URL nicht kennen, [Hier erfahren Sie, wie Sie ihn finden](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).

## Felder für Synchronisierung auswählen {#select-fields-to-sync}

Jetzt müssen wir die Felder auswählen, über die wir die Synchronisation durchführen möchten.

1. Klicks **Bearbeiten** in **Schritt 2: Wählen Sie Zu synchronisierende Felder aus.**

   ![](assets/image2015-3-16-9-51-28a.png)

1. Es gibt vorab ausgewählte Felder, die synchronisiert werden. Fügen Sie bei Bedarf weitere hinzu und klicken Sie auf **Speichern**.

   ![](assets/image2016-8-25-13-3a26-3a14.png)

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

   ![](assets/image2016-8-25-14-3a14-3a57.png)

## Synchronisierung aktivieren {#enable-sync}

1. Klicks **Bearbeiten** in **Schritt 3: Synchronisierung aktivieren**.

   ![](assets/image2015-3-16-9-52-2b.png)

   >[!CAUTION]
   >
   >Marketo deaktiviert die Duplizierung nicht automatisch für eine Microsoft Dynamics-Synchronisation oder wenn Sie Personen oder Leads manuell eingeben.

1. Alles im Popup lesen, Ihre E-Mail eingeben und auf klicken **Synchronisierung starten**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. Die erste Synchronisation kann einige Stunden dauern. Nach Abschluss des Vorgangs erhalten Sie eine E-Mail-Benachrichtigung.

   ![](assets/image2014-12-11-11-3a55-3a15.png)

   Exzellente Arbeit!
