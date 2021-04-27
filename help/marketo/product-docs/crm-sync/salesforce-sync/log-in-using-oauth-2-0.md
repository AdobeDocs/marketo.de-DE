---
description: Melden Sie sich mit OAuth 2.0 - Marketo Docs - Produktdokumentation an
title: Anmelden mit OAuth 2.0
exl-id: 0a70505d-d2b8-4dc9-ad11-decc86588f7f
translation-type: tm+mt
source-git-commit: d81a4a3caa12c5ec642afadf9328b3825bde6fed
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# Anmelden mit OAuth 2.0 {#log-in-using-oauth-2-0}

Salesforce verwendet das OAuth-Protokoll, um Benutzern von Anwendungen den sicheren Zugriff auf die Daten zu ermöglichen (die Anwendung mit OAuth 2.0 authentifizieren), ohne die Anmeldedaten offen legen zu müssen. Im Folgenden werden die Schritte beschrieben, die ausgeführt werden müssen, um Marketo sicher mit Salesforce zu verbinden und zu synchronisieren.

## Einrichten einer verbundenen App {#set-up-connected-app}

1. Navigieren Sie in Salesforce unter &quot;Einrichten&quot;in den Plattformwerkzeugen zu Apps, App Manager, und klicken Sie auf **Neue verbundene App**.

   ![](assets/setting-up-oauth-2-1.png)

1. Füllen Sie die Details aus und klicken Sie auf **Speichern**.

   ![](assets/setting-up-oauth-2-2.png)

1. Klicken Sie auf das Kontrollkästchen **OAuth-Einstellungen aktivieren**. Geben Sie für Callback-URL `https://app.marketo.com/salesforce/getSfdcOAuthTokensRedirect` ein. Wählen Sie alle verfügbaren OAuth-Bereiche aus und klicken Sie auf **Hinzufügen**.

   ![](assets/setting-up-oauth-2-3.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/setting-up-oauth-2-4.png)

1. Klicken Sie auf **Weiter**.

   ![](assets/setting-up-oauth-2-5.png)

1. Kopieren Sie Consumer key und Consumer secret.

   ![](assets/setting-up-oauth-2-6.png)

>[!NOTE]
>
>Speichern Sie die Consumer key- und Consumer secret-Informationen zur späteren Verwendung in Marketo.

## Einrichten von Marketo {#set-up-marketo}

>[!PREREQUISITES]
>
>* Der API-Zugriff muss für den Salesforce-Synchronisierungsbenutzer aktiviert sein (wenn Sie Salesforce Professional Edition-Benutzer sind, ist dieser Zugriff standardmäßig nicht verfügbar. Wenden Sie sich an Ihren Salesforce-Kundenbetreuer).
>* Marketo Sync user muss in Salesforce erstellt werden.
>* Für bestehende Kunden ist die Funktion &quot;OAuth für SFDC-Synchronisierung aktivieren&quot;auf dem Abonnement des Kunden aktiviert.
>* Popup-Blocker sind deaktiviert.
>* Es wird eine verbundene App erstellt und die Consumer key und Consumer secret stehen zur Verwendung bereit.


>[!CAUTION]
>
>Vergewissern Sie sich, dass alle nicht benötigten Felder in Marketo vor dem Synchronisierungsbenutzer ausgeblendet werden, bevor Sie auf **Felder synchronisieren** klicken. Nachdem Sie auf &quot;Felder synchronisieren&quot;geklickt haben, werden alle Felder, die der Benutzer im SFDC sehen kann, dauerhaft in Marketo erstellt und können nicht gelöscht werden.

1. Klicken Sie im Abschnitt Marketo Admin auf **CRM** und dann **Synchronisieren mit Salesforce**.

   ![](assets/setting-up-oauth-2-7.png)

1. hinzufügen Sie die zuvor aufgezeichneten Consumer key- und Consumer secret-Informationen und klicken Sie auf und **Speichern**.

   ![](assets/setting-up-oauth-2-8.png)

1. Klicken Sie auf der Synchronisierungsseite von Marketo Salesforce auf die Schaltfläche **Mit Salesforce** anmelden.

   ![](assets/setting-up-oauth-2-9.png)

   >[!CAUTION]
   >
   >Wenn die Felder Benutzername/Kennwort/Token und nicht die Schaltfläche &quot;Mit Salesforce anmelden&quot;angezeigt werden, ist Ihr Marketo-Abonnement für die einfache Authentifizierung aktiviert. Siehe [Einrichten von Marketo mit einfacher Authentifizierung](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md). Sobald die Synchronisierung mit einem Satz von Anmeldeinformationen beginnt, wird kein Wechsel von Salesforce-Anmeldeinformationen oder -Abonnement durchgeführt. Wenn Sie Oauth 2.0 verwenden möchten, wenden Sie sich an Ihren Kundenbetreuer.

1. Ein Popup mit der Anmeldeseite salesforce wird angezeigt. Geben Sie die Anmeldedaten für Marketo Sync User ein und melden Sie sich an.

   ![](assets/setting-up-oauth-2-10.png)

1. Geben Sie den Bestätigungscode ein, den Sie per E-Mail erhalten haben (gesendet von Salesforce), und klicken Sie auf **Verify**.

   ![](assets/setting-up-oauth-2-11.png)

1. Nach erfolgreicher Überprüfung wird die Zugriffsseite angezeigt, auf der der Zugriff angefordert wird. Klicken Sie auf **Allow**.

   ![](assets/setting-up-oauth-2-12.png)

1. In wenigen Minuten wird in Marketo ein Popup angezeigt. Klicken Sie auf **Anmeldeinformationen** bestätigen.

   ![](assets/setting-up-oauth-2-13.png)

1. Klicken Sie nach Abschluss der Feldsynchronisierung auf **Beginn Salesforce Sync**.

   ![](assets/setting-up-oauth-2-14.png)

1. Klicken Sie auf **Beginn-Synchronisierung**.

   ![](assets/setting-up-oauth-2-15.png)

Ihre Synchronisierung zwischen Marketo und Salesforce läuft jetzt.

![](assets/setting-up-oauth-2-16.png)

>[!MORELIKETHIS]
>
>* [Schritt 1 von 3: hinzufügen Marketo-Felder für Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Schritt 2 von 3: Salesforce-Benutzer für Marketo erstellen (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Installieren des Marketo Sales Insight-Pakets in Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Marketo Sales Insight in Salesforce Enterprise/Unlimited konfigurieren](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

