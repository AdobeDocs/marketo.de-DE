---
unique-page-id: 3571819
description: 'Schritt 3 von 3: Verbinden von Marketo und Dynamics (On-Premises 2013) - Marketo Docs - Produktdokumentation'
title: 'Schritt 3 von 3: Verbinden von Marketo und Dynamics (On-Premises 2013)'
exl-id: e28f1cc3-ee15-4981-a537-6c4a1682c4c1
source-git-commit: f130fa1187ccead6573f76ff947e55d42f6962e4
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 1%

---

# Schritt 3 von 3: Marketo und Dynamics verbinden (On-Premises 2013) {#step-of-connect-marketo-and-dynamics-on-premises}

Gut! Wir haben die Lösung installiert und den Synchronisierungsbenutzer konfiguriert. Als Nächstes müssen wir Marketo und Dynamics verbinden.

>[!PREREQUISITES]
>
>* [Schritt 1 von 3: Installieren der Marketo-Lösung in Dynamics (On-Premises 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2013.md)
>* [Schritt 2 von 3: Konfigurieren der Synchronisierungsbenutzer für Marketo (On-Premises 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-configure-2013.md)


>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

## Benutzerinformationen zur Dynamics Sync eingeben {#enter-dynamics-sync-user-information}

1. Melden Sie sich bei Marketo an und klicken Sie auf **Admin**.

   ![](assets/login-admin.png)

1. Klicken Sie auf **CRM**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Auswählen **Microsoft**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Klicken **Bearbeiten** in **Schritt 1: Anmeldedaten eingeben**.

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Stellen Sie sicher, dass Ihre Anmeldedaten korrekt sind, da wir die nachfolgenden Schemaänderungen nach der Übermittlung nicht rückgängig machen können. Wenn falsche Anmeldeinformationen gespeichert werden, müssen Sie ein neues Marketo-Abonnement erhalten.

1. Geben Sie die **Benutzername**, **Passwort** und Microsoft Dynamics **URL** Klicken Sie dann auf **Speichern**.

   ![](assets/image2015-3-26-11-3a47-3a59.png)

   >[!NOTE]
   >
   >* Der Benutzername in Marketo muss mit dem Benutzernamen für den Synchronisierungsbenutzer im CRM übereinstimmen. Das Format kann user@domain.com oder DOMAIN\user lauten.
   >* Wenn Sie die URL nicht kennen, [Hier erfahren Sie, wie Sie ihn finden](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).


## Felder für Synchronisierung auswählen {#select-fields-to-sync}

Jetzt müssen wir die Felder auswählen, über die wir synchronisieren möchten.

1. Klicken **Bearbeiten** in **Schritt 2: Zu synchronisierende Felder auswählen**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Wählen Sie die Felder aus, die Sie mit Marketo synchronisieren möchten, damit sie vorausgewählt werden. Klicken **Speichern**.

   ![](assets/image2016-8-25-15-3a10-3a17.png)

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

   ![](assets/image2016-8-25-15-3a11-3a4.png)

## Synchronisierung aktivieren {#enable-sync}

1. Klicken **Bearbeiten** in **Schritt 3: Synchronisierung aktivieren**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo deaktiviert die Duplizierung nicht automatisch für eine Microsoft Dynamics-Synchronisation oder wenn Sie Personen oder Leads manuell eingeben.

1. Lesen Sie alles im Popup-Fenster, geben Sie Ihre E-Mail ein und klicken Sie auf **Synchronisierung starten**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. Die erste Synchronisation kann einige Stunden dauern. Nach Abschluss des Vorgangs erhalten Sie eine E-Mail-Benachrichtigung.

   ![](assets/image2014-12-11-11-3a55-3a15.png)

Exzellente Arbeit! Sie haben soeben die Leistung der bidirektionalen Synchronisation zwischen Marketo und Microsoft Dynamics freigesetzt. Wenn Sie Marketo Sales Insight erworben haben, bietet es mehr Spaß:

>[!MORELIKETHIS]
>
>[Installieren und Konfigurieren von Marketo Sales Insight in Microsoft Dynamics 2013](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2013.md)