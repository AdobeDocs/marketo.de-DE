---
unique-page-id: 3571800
description: 'Schritt 3 von 3: Verbinden von Marketo und Salesforce (Professional) - Marketo Docs - Produktdokumentation'
title: 'Schritt 3 von 3: Verbinden von Marketo und Salesforce (Professional)'
exl-id: a35e22ef-6378-45e0-be7e-687b0832ecf3
source-git-commit: 8162db802cae125b406c463fde50d4ffdf0eb621
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# Schritt 3 von 3: Verbinden von Marketo und Salesforce (Professional) {#step-of-connect-marketo-and-salesforce-professional}

In diesem Artikel konfigurieren Sie Marketo für die Synchronisierung mit Ihrer konfigurierten Salesforce-Instanz.

>[!PREREQUISITES]
>
>* [Schritt 1 von 3: Marketo-Felder zu Salesforce (Professional) hinzufügen](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md)
>* [Schritt 2 von 3: Salesforce-Benutzer für Marketo (Professional) erstellen](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md)


## Sync User Security Token abrufen {#retrieve-sync-user-security-token}

>[!TIP]
>
>Wenn Sie bereits über das Sicherheits-Token verfügen, fahren Sie zur Vorbereitung direkt mit Festlegen von Sync User Credentials and kudos fort!

1. Melden Sie sich mit dem Marketo Sync User bei Salesforce an, klicken Sie auf den Namen des Synchronisierungsbenutzers und dann auf **Meine Einstellungen**.

   ![](assets/image2015-5-21-14-3a11-3a17.png)

1. Geben Sie in der Navigationssuchleiste &quot;reset&quot;ein und klicken Sie auf **Mein Sicherheitstoken zurücksetzen**.

   ![](assets/image2014-12-9-9-3a52-3a42.png)

1. Klicken **Sicherheitstoken zurücksetzen**.

   ![](assets/image2015-5-21-14-3a13-3a5.png)

   Das Sicherheits-Token wird Ihnen per E-Mail zugestellt.

## Festlegen von Sync User Credentials {#set-sync-user-credentials}

1. Navigieren Sie in Marketo zu **Admin** auswählen **CRM** und klicken Sie auf **Synchronisieren mit [Salesforce.com](https://Salesforce.com)**.

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >Stellen Sie sicher, dass [Alle nicht benötigten Felder ausblenden](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md) in Marketo vom Synchronisierungsbenutzer aus, bevor auf **Synchronisierungsfelder**. Wenn Sie auf Felder synchronisieren klicken, werden alle Felder, die dem Benutzer angezeigt werden, dauerhaft in Marketo erstellt und können nicht gelöscht werden.

1. Geben Sie die Salesforce Sync User-Anmeldeinformationen ein, die in Teil 2 der Salesforce-Konfiguration erstellt wurden ([Professional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md), [Unternehmen](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) und klicken Sie auf **Synchronisierungsfelder**.

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!NOTE]
   >
   >Überprüfen **Sandbox** wenn Sie eine Marketo-Sandbox mit einer Salesforce-Sandbox synchronisieren.

1. Lesen Sie die Warnung und klicken Sie auf **Anmeldeinformationen bestätigen**.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Wenn Sie die [Zuordnungen erstellen und anpassen](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md), dies ist Ihre einzige Chance, dies zu tun! Nachdem Sie auf Salesforce Sync starten geklickt haben, ist es fertig.

## Salesforce-Synchronisierung starten {#start-salesforce-sync}

1. Klicken **Salesforce Sync starten** , um die permanente Marketo-Salesforce-Synchronisation zu starten.

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo deaktiviert das Duplizieren nicht automatisch für eine Salesforce-Synchronisation oder wenn Sie Leads manuell eingeben.

1. Klicken **Synchronisierung starten**.

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >Die Dauer der Erstsynchronisierung hängt von der Größe und Komplexität Ihrer Datenbank ab.

## Synchronisierung überprüfen {#verify-sync}

Marketo stellt Statusmeldungen für die Salesforce-Synchronisation im Admin-Bereich bereit. Sie können überprüfen, ob die Synchronisierung ordnungsgemäß funktioniert, indem Sie die folgenden Schritte ausführen.

1. Klicken Sie in Marketo auf **Admin**, dann **Salesforce**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. Der Synchronisierungsstatus wird oben rechts angezeigt. Es wird eine von drei Nachrichten angezeigt: **Zuletzt synchronisiert**, **Synchronisierung läuft** oder **Fehlgeschlagen**.

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Wow, Sie haben gerade mit der Konfiguration einer der leistungsstärksten Funktionen von Marketo fertig, gehen Sie!

>[!MORELIKETHIS]
>
>* [Installieren des Marketo Sales Insight-Pakets in Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Konfigurieren von Marketo Sales Insight in Salesforce Professional Edition](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)

