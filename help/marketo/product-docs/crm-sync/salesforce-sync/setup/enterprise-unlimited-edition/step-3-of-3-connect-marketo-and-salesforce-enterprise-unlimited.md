---
unique-page-id: 2360366
description: 'Schritt 3 von 3: Verbinden von Marketo und Salesforce (Enterprise/Unlimited) - Marketo Docs - Produktdokumentation'
title: 'Schritt 3 von 3: Verbinden von Marketo und Salesforce (Enterprise/Unlimited)'
exl-id: ef74bc53-9dc9-43c7-a9aa-565463fdd2e5
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# Schritt 3 von 3: Verbinden von Marketo und Salesforce (Enterprise/Unlimited) {#step-of-connect-marketo-and-salesforce-enterprise-unlimited}

In diesem Artikel konfigurieren Sie Marketo Engage so, dass es mit Ihrer konfigurierten Salesforce-Instanz synchronisiert wird.

>[!PREREQUISITES]
>
>* [Schritt 1 von 3: Hinzufügen von Marketo-Feldern zu Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}
>* [Schritt 2 von 3: Erstellen eines Salesforce-Benutzers für Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}

## Sync User Security Token abrufen {#retrieve-sync-user-security-token}

>[!TIP]
>
>Wenn Sie bereits über das Sicherheits-Token verfügen, fahren Sie zur Vorbereitung direkt mit Festlegen von Sync User Credentials and kudos fort!

1. Melden Sie sich mit dem Marketo Sync User bei Salesforce an, klicken Sie auf den Namen des Synchronisierungsbenutzers und dann auf **[!UICONTROL Meine Einstellungen]**.

   ![](assets/image2015-6-12-9-3a12-3a47.png)

1. Geben Sie bei der schnellen Suche &quot;reset&quot;ein und klicken Sie auf **[!UICONTROL Mein Sicherheitstoken zurücksetzen]**.

   ![](assets/image2015-6-12-9-3a13-3a39.png)

1. Klicks **[!UICONTROL Sicherheits-Token zurücksetzen]**.

   ![](assets/image2014-12-9-9-3a52-3a50.png)

   Das Sicherheits-Token wird Ihnen per E-Mail zugestellt.

## Festlegen von Sync User Credentials {#set-sync-user-credentials}

1. Navigieren Sie in Marketo zu **[!UICONTROL Admin]** auswählen **[!UICONTROL CRM]** und klicken Sie auf **Synchronisieren mit [Salesforce.com](https://Salesforce.com)**

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >Stellen Sie sicher, [Alle nicht benötigten Felder ausblenden](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target="_blank"} in Marketo vom Synchronisierungsbenutzer aus, bevor auf **[!UICONTROL Synchronisierungsfelder]**. Wenn Sie auf Felder synchronisieren klicken, werden alle Felder, die dem Benutzer angezeigt werden, dauerhaft in Marketo erstellt und können nicht gelöscht werden.

1. Geben Sie die Salesforce Sync User-Anmeldeinformationen ein, die in Teil 2 der Salesforce-Konfiguration erstellt wurden ([Professional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md){target="_blank"} or [Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}) und klicken Sie auf **[!UICONTROL Synchronisierungsfelder]** (check **[!UICONTROL Sandbox]** nur, wenn Sie eine Marketo-Sandbox mit einer Salesforce-Sandbox synchronisieren).

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!CAUTION]
   >
   >Wenn anstelle der Felder &quot;Benutzername/Kennwort/Token&quot;die Schaltfläche &quot;Bei Salesforce anmelden&quot;angezeigt wird, ist Ihr Marketo-Abonnement für OAuth aktiviert. Bitte [in diesem Artikel](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md){target="_blank"}. Sobald die Synchronisierung mit der Verwendung einer Reihe von Anmeldeinformationen beginnt, _Salesforce-Anmeldedaten oder -Abonnements werden nicht geändert_. Wenn Sie die Standardauthentifizierung verwenden möchten, wenden Sie sich an das Adobe Account Team (Ihren Kundenbetreuer).

1. Lesen Sie die Warnung und klicken Sie dann auf **[!UICONTROL Anmeldeinformationen bestätigen]**.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Wenn Sie die [Zuordnungen erstellen und anpassen](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md){target="_blank"}, dies ist Ihre einzige Chance, dies zu tun! Nachdem Sie auf Salesforce Sync starten geklickt haben, ist es fertig.

## Salesforce-Synchronisierung starten {#start-salesforce-sync}

1. Klicks **[!UICONTROL Salesforce Sync starten]** , um die permanente Marketo-Salesforce-Synchronisation zu starten.

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo deaktiviert das Duplizieren nicht automatisch für eine Salesforce-Synchronisation oder wenn Sie Leads manuell eingeben.

1. Klicks **[!UICONTROL Synchronisierung starten]**.

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >Die Dauer der Erstsynchronisierung hängt von der Größe und Komplexität Ihrer Datenbank ab.

## Synchronisierung überprüfen {#verify-sync}

Marketo stellt Statusmeldungen für die Salesforce-Synchronisation im Admin-Bereich bereit. Sie können überprüfen, ob die Synchronisierung ordnungsgemäß funktioniert, indem Sie die folgenden Schritte ausführen.

1. Klicken Sie in Marketo auf **[!UICONTROL Admin]**, dann **Salesforce**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. Der Synchronisierungsstatus wird oben rechts angezeigt. Es wird eine von drei Nachrichten angezeigt: **[!UICONTROL Zuletzt synchronisiert]**, **[!UICONTROL Synchronisierung läuft]** oder **[!UICONTROL Fehlgeschlagen]**.

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Sie sind gerade mit der Konfiguration einer der leistungsstärksten Funktionen von Marketo fertig, gehen Sie!

>[!MORELIKETHIS]
>
>* [Schritt 1 von 3: Hinzufügen von Marketo-Feldern zu Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}
>* [Schritt 2 von 3: Erstellen eines Salesforce-Benutzers für Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}
>* [Installieren des Marketo Sales Insight-Pakets in Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}
>* [Konfigurieren von Marketo Sales Insight in Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md){target="_blank"}
