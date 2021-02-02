---
unique-page-id: 3571800
description: Schritt 3 von 3 - Connect Marketing and Salesforce (Professional) - Marketing Docs - Produktdokumentation
title: Schritt 3 von 3 - Connect Marketing and Salesforce (Professional)
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---


# Schritt 3 von 3: Connect Marketo und Salesforce (Professional) {#step-of-connect-marketo-and-salesforce-professional}

In diesem Artikel konfigurieren Sie Marketo für die Synchronisierung mit Ihrer konfigurierten Salesforce-Instanz.

>[!PREREQUISITES]
>
>* [Schritt 1 von 3: hinzufügen Marketo Fields to Salesforce (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md)
>* [Schritt 2 von 3: Erstellen eines Salesforce-Benutzers für Marketing (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md)


## Synchronisierungs-Benutzersicherheitstoken abrufen {#retrieve-sync-user-security-token}

>[!TIP]
>
>Wenn Sie bereits über das Sicherheits-Token verfügen, fahren Sie direkt mit &quot;Synchronisieren Sie Benutzeranmeldeinformationen und -kudos für die Vorbereitung!&quot;fort.

1. Melden Sie sich bei Salesforce mit dem Benutzer Marketo Sync an, klicken Sie auf den Namen des Synchronisierungsbenutzers und dann **Meine Einstellungen**.

   ![](assets/image2015-5-21-14-3a11-3a17.png)

1. Geben Sie in der Navigationsleiste &quot;reset&quot;ein und klicken Sie auf **Reset My Security Token**.

   ![](assets/image2014-12-9-9-3a52-3a42.png)

1. Klicken Sie auf **Sicherheitstoken zurücksetzen**.

   ![](assets/image2015-5-21-14-3a13-3a5.png)

   Das Sicherheitstoken wird Ihnen per E-Mail zugesendet.

## Festlegen der Synchronisierungsbenutzeranmeldeinformationen {#set-sync-user-credentials}

1. Gehen Sie in Marketo zu **Admin**, wählen Sie **CRM** und klicken Sie auf **Synchronisieren mit [Salesforce.com](https://Salesforce.com)**.

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >Vergewissern Sie sich, dass Sie [alle Felder, die Sie nicht benötigen, in Marketo vor dem Synchronisierungsbenutzer ausblenden, bevor Sie auf **Felder synchronisieren** klicken. ](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync/hide-a-salesforce-field-from-the-marketo-sync.md) Nachdem Sie auf &quot;Felder synchronisieren&quot;geklickt haben, werden alle Felder, die der Benutzer sehen kann, dauerhaft in Marketo erstellt und können nicht gelöscht werden.

1. Geben Sie die in Teil 2 der Salesforce-Konfiguration ([Professional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md), [Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)) erstellten Salesforce-Synchronisierungsbenutzer-Anmeldedaten ein und klicken Sie auf **Synchronisierungsfelder**.

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!NOTE]
   >
   >Markieren Sie **Sandbox**, wenn Sie eine Marketo Sandbox mit einer Salesforce Sandbox synchronisieren.

1. Lesen Sie die Warnung und klicken Sie dann auf **Anmeldeinformationen** bestätigen.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Wenn Sie über die [Zuordnungen schauen und sie anpassen wollen](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md), dies ist Ihre einzige Chance! Nachdem Sie auf Beginn Salesforce Sync geklickt haben, ist es fertig.

## Beginn Salesforce Sync {#start-salesforce-sync}

1. Klicken Sie auf **Beginn Salesforce Sync**, um die permanente Synchronisierung von Marketing-Salesforce zu starten.

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo wird die Duplizierung nicht automatisch bei einer Salesforce-Synchronisierung oder bei manueller Eingabe von Leads aufheben.

1. Klicken Sie auf **Beginn-Synchronisierung**.

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >Die Dauer zum Abschluss der ersten Synchronisierung hängt von der Größe und Komplexität der Datenbank ab.

## Synchronisierung überprüfen {#verify-sync}

Marketo stellt Statusmeldungen für die Salesforce-Synchronisierung im Admin-Bereich bereit. Sie können überprüfen, ob die Synchronisierung ordnungsgemäß funktioniert, indem Sie die folgenden Schritte ausführen.

1. Klicken Sie in Marketo auf **Admin** und dann auf **Salesforce**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. Der Synchronisierungsstatus ist in der oberen rechten Ecke sichtbar. Es wird eine von drei Nachrichten angezeigt: **Zuletzt synchronisiert**, **Synchronisierung läuft** oder **Fehlgeschlagen**.

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Wow, du hast gerade eine der mächtigsten Funktionen von Marketo konfiguriert, los!

>[!MORELIKETHIS]
>
>* [Installieren des Marketo Sales Insight-Pakets in Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Konfigurieren von Marketo Sales Insight in Salesforce Professional Edition](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)

