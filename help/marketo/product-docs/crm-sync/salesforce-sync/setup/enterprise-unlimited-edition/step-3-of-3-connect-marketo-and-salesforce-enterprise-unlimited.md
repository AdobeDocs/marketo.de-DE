---
unique-page-id: 2360366
description: Schritt 3 von 3 - Verbinden von Marketo und Salesforce (Enterprise/Unlimited) - Marketo Docs - Produktdokumentation
title: Schritt 3 von 3 - Verbinden von Marketo und Salesforce (Enterprise/Unlimited)
exl-id: ef74bc53-9dc9-43c7-a9aa-565463fdd2e5
translation-type: tm+mt
source-git-commit: d81a4a3caa12c5ec642afadf9328b3825bde6fed
workflow-type: tm+mt
source-wordcount: '466'
ht-degree: 0%

---

# Schritt 3 von 3: Verbinden von Marketo und Salesforce (Enterprise/Unlimited) {#step-of-connect-marketo-and-salesforce-enterprise-unlimited}

In diesem Artikel konfigurieren Sie Marketo für die Synchronisierung mit Ihrer konfigurierten Salesforce-Instanz.

>[!PREREQUISITES]
>
>* [Schritt 1 von 3: hinzufügen Marketo-Felder für Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Schritt 2 von 3: Salesforce-Benutzer für Marketo erstellen (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)


## Synchronisierungs-Benutzersicherheitstoken abrufen {#retrieve-sync-user-security-token}

>[!TIP]
>
>Wenn Sie bereits über das Sicherheits-Token verfügen, fahren Sie direkt mit &quot;Synchronisieren Sie Benutzeranmeldeinformationen und -kudos für die Vorbereitung!&quot;fort.

1. Melden Sie sich mit dem Marketo Sync User bei Salesforce an, klicken Sie auf den Namen des Synchronisierungsbenutzers und dann auf **Meine Einstellungen**.

   ![](assets/image2015-6-12-9-3a12-3a47.png)

1. Geben Sie in der Schnellsuche &quot;reset&quot;ein und klicken Sie auf **Reset My Security Token**.

   ![](assets/image2015-6-12-9-3a13-3a39.png)

1. Klicken Sie auf **Sicherheitstoken zurücksetzen**.

   ![](assets/image2014-12-9-9-3a52-3a50.png)

   Das Sicherheitstoken wird Ihnen per E-Mail zugesendet.

## Festlegen der Synchronisierungsbenutzeranmeldeinformationen {#set-sync-user-credentials}

1. Gehen Sie in Marketo zu **Admin**, wählen Sie **CRM** und klicken Sie auf **Synchronisieren mit [Salesforce.com](https://Salesforce.com)**

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >Vergewissern Sie sich, dass Sie alle nicht benötigten Felder in Marketo vor dem Synchronisierungsbenutzer ausblenden, bevor Sie auf **Felder synchronisieren** klicken. [](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync/hide-a-salesforce-field-from-the-marketo-sync.md) Nachdem Sie auf &quot;Felder synchronisieren&quot;geklickt haben, werden alle vom Benutzer angezeigten Felder dauerhaft in Marketo erstellt und können nicht gelöscht werden.

1. Geben Sie die in Teil 2 der Salesforce-Konfiguration ([Professional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md) oder [Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)) erstellten Salesforce-Synchronisierungsbenutzer-Anmeldedaten ein und klicken Sie auf **Synchronisierungsfelder** (nur wenn Sie eine Marketo Sandbox mit einer Salesforce-Sandbox synchronisieren).****

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!CAUTION]
   >
   >Wenn anstelle der Felder Benutzername/Kennwort/Token die Schaltfläche &quot;Bei Salesforce anmelden&quot;angezeigt wird, ist Ihr Marketo-Abonnement für OAuth aktiviert. Bitte [verweisen Sie auf diesen Artikel](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md). Sobald die Synchronisierung mit einem Satz Anmeldeinformationen beginnt, gibt es kein Umschalten zwischen Salesforce-Anmeldeinformationen oder Abonnement **.** Wenn Sie die einfache Authentifizierung verwenden möchten, wenden Sie sich an Ihren Kundenbetreuer.

1. Lesen Sie die Warnung und klicken Sie dann auf **Anmeldeinformationen** bestätigen.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Wenn Sie über die [Zuordnungen schauen und sie anpassen wollen](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md), dies ist Ihre einzige Chance! Nachdem Sie auf Beginn Salesforce Sync geklickt haben, ist es fertig.

## Salesforce-Synchronisierung starten {#start-salesforce-sync}

1. Klicken Sie auf **Beginn Salesforce Sync**, um die permanente Marketo-Salesforce-Synchronisierung zu starten.

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo wird das Duplizieren nicht automatisch bei einer Salesforce-Synchronisierung oder bei manueller Eingabe von Leads aufheben.

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

Wow, Sie haben gerade die Konfiguration eines der leistungsstärksten Features von Marketo beendet, gehen Sie!

>[!MORELIKETHIS]
>
>* [Schritt 1 von 3: hinzufügen Marketo-Felder für Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Schritt 2 von 3: Salesforce-Benutzer für Marketo erstellen (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Installieren des Marketo Sales Insight-Pakets in Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Marketo Sales Insight in Salesforce Enterprise/Unlimited konfigurieren](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

