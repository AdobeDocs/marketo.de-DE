---
unique-page-id: 3571800
description: Schritt 3 von 3 - Marketo und Salesforce verbinden (Professional) - Marketo-Dokumente - Produktdokumentation
title: 'Schritt 3 von 3: Marketo und Salesforce verbinden (Professional)'
exl-id: a35e22ef-6378-45e0-be7e-687b0832ecf3
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Schritt 3 von 3: Marketo und Salesforce verbinden (Professional) {#step-of-connect-marketo-and-salesforce-professional}

In diesem Artikel konfigurieren Sie den Marketo Engage für die Synchronisierung mit Ihrer konfigurierten Salesforce-Instanz.

>[!PREREQUISITES]
>
>* [Schritt 1 von 3: Marketo-Felder zu Salesforce (Professional) hinzufügen](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md){target="_blank"}
>* [Schritt 2 von 3: Erstellen eines Salesforce-Benutzers für Marketo (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md){target="_blank"}

## Abrufen des Synchronisierungs-Benutzer-Sicherheits-Tokens {#retrieve-sync-user-security-token}

>[!TIP]
>
>Wenn Sie bereits über das Sicherheits-Token verfügen, fahren Sie direkt mit dem Schritt Benutzeranmeldeinformationen und Lob für die Vorbereitung festlegen fort!

1. Melden Sie sich bei Salesforce mit dem Marketo-Synchronisierungsbenutzer an und klicken Sie auf den Namen des Synchronisierungsbenutzers und dann auf **[!UICONTROL Meine Einstellungen]**.

   ![](assets/image2015-5-21-14-3a11-3a17.png)

1. Geben Sie in der Navigationssuchleiste „Zurücksetzen“ ein und klicken Sie auf **[!UICONTROL Mein Sicherheits-Token zurücksetzen]**.

   ![](assets/image2014-12-9-9-3a52-3a42.png)

1. Klicken Sie **[!UICONTROL Sicherheitstoken zurücksetzen]**.

   ![](assets/image2015-5-21-14-3a13-3a5.png)

   Das Sicherheits-Token wird Ihnen per E-Mail gesendet.

## Festlegen von Benutzeranmeldeinformationen für die Synchronisierung {#set-sync-user-credentials}

1. Wechseln Sie in Marketo zu **[!UICONTROL Admin]**, wählen Sie **[!UICONTROL CRM]** aus und klicken Sie auf **[!UICONTROL Mit Salesforce.com synchronisieren]**.

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >Stellen Sie sicher[ dass Sie in Marketo alle nicht ](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target="_blank"} Felder vor dem Synchronisierungsbenutzer ausblenden, bevor Sie auf **[!UICONTROL Felder synchronisieren]** klicken. Nachdem Sie auf Felder synchronisieren geklickt haben, werden alle Felder, die der Benutzer sehen kann, dauerhaft in Marketo erstellt und können nicht gelöscht werden.

1. Geben Sie die in Teil 2 der Salesforce-Konfiguration ([Professional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md), [Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)) erstellten Anmeldeinformationen für den Salesforce-Benutzer ein und klicken Sie auf **[!UICONTROL Felder synchronisieren]**.

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!NOTE]
   >
   >Aktivieren Sie **[!UICONTROL Sandbox]**, wenn Sie eine Marketo-Sandbox mit einer Salesforce-Sandbox synchronisieren.

1. Lesen Sie die Warnung und klicken Sie dann auf **[!UICONTROL Anmeldedaten bestätigen]**.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Wenn Sie die Zuordnungen ([) überprüfen und anpassen möchten](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md){target="_blank"} ist dies die einzige Möglichkeit, dies zu tun! Nachdem Sie auf Salesforce-Synchronisierung starten geklickt haben, ist der Vorgang abgeschlossen.

## Salesforce-Synchronisierung starten {#start-salesforce-sync}

1. Klicken Sie **[!UICONTROL Salesforce-Synchronisierung starten]**, um die persistente Marketo-Salesforce-Synchronisierung zu starten.

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo wird nicht automatisch für eine Salesforce-Synchronisierung dedupliziert oder wenn Sie Leads manuell eingeben.

1. Klicken Sie **[!UICONTROL Synchronisierung starten]**.

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >Die Zeit bis zum Abschluss der ersten Synchronisierung hängt von der Größe und Komplexität Ihrer Datenbank ab.

## Synchronisierung überprüfen {#verify-sync}

Marketo stellt Statusmeldungen für die Salesforce-Synchronisierung im Admin-Bereich bereit. Gehen Sie wie folgt vor, um zu überprüfen, ob die Synchronisierung ordnungsgemäß funktioniert.

1. Klicken Sie in Marketo auf **[!UICONTROL Admin]** und dann auf **Salesforce**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. Der Synchronisierungsstatus wird in der oberen rechten Ecke angezeigt. Eine der drei Meldungen wird angezeigt: **[!UICONTROL Zuletzt synchronisiert]**, **[!UICONTROL Synchronisierung läuft]** oder **[!UICONTROL Fehlgeschlagen]**.

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Sie haben gerade die Konfiguration einer der leistungsfähigsten Funktionen von Marketo abgeschlossen, los geht&#39;s!

>[!MORELIKETHIS]
>
>* [Installieren des Marketo Sales Insight-Pakets auf der Salesforce-AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}
>* [Konfigurieren von Marketo Sales Insight in Salesforce Professional Edition](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md){target="_blank"}
