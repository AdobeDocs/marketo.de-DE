---
description: Anmelden mit OAuth 2.0 - Marketo Docs - Produktdokumentation
title: Anmelden mit OAuth 2.0
exl-id: 0a70505d-d2b8-4dc9-ad11-decc86588f7f
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---

# Anmelden mit OAuth 2.0 {#log-in-using-oauth-2-0}

Salesforce verwendet das OAuth-Protokoll, um Anwendern von Anwendungen den sicheren Zugriff (Authentifizierung der Anwendung mit OAuth 2.0) auf Daten zu ermöglichen, ohne Anmeldeinformationen anzuzeigen. Im Folgenden werden die Schritte beschrieben, die zur sicheren Verbindung und Synchronisation von Marketo Engage mit Salesforce durchgeführt werden müssen.

>[!IMPORTANT]
>
>Um über OAuth eine Verbindung zwischen Marketo und Salesforce herzustellen, melden Sie sich über einen privaten (Inkognito-)Browser bei Marketo an, um zu verhindern, dass eine Verbindung mit Salesforce mit dem falschen Benutzernamen hergestellt wird.

## Einrichten einer verbundenen App {#set-up-connected-app}

1. Navigieren Sie in Salesforce unter &quot;Einrichtung&quot;in den Platform Tools zu Apps, App Manager, und klicken Sie auf **[!UICONTROL Neue verbundene App]**.

   ![](assets/setting-up-oauth-2-1.png)

1. Füllen Sie die Details aus und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/setting-up-oauth-2-2.png)

1. Klicken Sie auf **[!UICONTROL Aktivieren der OAuth-Einstellungen]** aktivieren. Geben Sie als Callback-URL ein. `https://app.marketo.com/salesforce/getSfdcOAuthTokensRedirect`. Wählen Sie alle verfügbaren OAuth-Bereiche aus und klicken Sie auf **[!UICONTROL Hinzufügen]**.

   ![](assets/setting-up-oauth-2-3.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/setting-up-oauth-2-4.png)

1. Klicks **[!UICONTROL Weiter]**.

   ![](assets/setting-up-oauth-2-5.png)

1. Kopieren Sie den Consumer Key und das Consumer Secret (Sie werden sie später zum Marketo Engage benötigen).

   ![](assets/setting-up-oauth-2-6.png)

>[!CAUTION]
>
>Scrollen Sie auf der Seite Neue verbundene App nach unten und stellen Sie sicher, dass das Kontrollkästchen &quot;Anfordern des Testversands für Code Exchange (PKCE)&quot;aktiviert ist. _NOT_ aktiviert, da dies die Einrichtung beeinträchtigen würde.

## Einrichten von Marketo {#set-up-marketo}

>[!PREREQUISITES]
>
>* Der API-Zugriff muss für den Salesforce Sync User aktiviert sein (wenn Sie Salesforce Professional Edition-Benutzer sind, ist dieser Zugriff standardmäßig nicht verfügbar - wenden Sie sich an Ihren Salesforce-Kundenbetreuer).
* Der Marketo Sync-Benutzer muss in Salesforce erstellt werden.
* Für Bestandskunden ist die Funktion &quot;OAuth für SFDC-Synchronisation aktivieren&quot;im Abonnement des Kunden aktiviert.
* Popup-Blocker sind deaktiviert.
* Es wurde eine vernetzte App erstellt, und es stehen der Consumer Key und das Consumer Secret zur Verfügung.

>[!CAUTION]
>
Stellen Sie sicher, dass alle nicht benötigten Felder in Marketo vor dem Synchronisierungsbenutzer ausgeblendet werden, bevor Sie auf **[!UICONTROL Synchronisierungsfelder]**. Nachdem Sie auf &quot;Synchronisierungsfelder&quot;geklickt haben, werden alle Felder, die der Benutzer im SFDC sehen kann, dauerhaft in Marketo erstellt und können nicht gelöscht werden.

1. Klicken Sie im Marketo Admin-Bereich auf **[!UICONTROL CRM]**, dann **[!UICONTROL Mit Salesforce synchronisieren]**.

   ![](assets/setting-up-oauth-2-7.png)

1. Fügen Sie die zuvor aufgezeichneten Informationen zum Consumer Key und Consumer Secret hinzu und klicken Sie auf und **[!UICONTROL Speichern]**.

   ![](assets/setting-up-oauth-2-8.png)

1. Klicken Sie auf der Synchronisierungsseite für Marketo Salesforce auf die **[!UICONTROL Mit Salesforce anmelden]** Schaltfläche.

   ![](assets/setting-up-oauth-2-9.png)

   >[!CAUTION]
   >
   Wenn die Felder &quot;Benutzername/Kennwort/Token&quot;und nicht die Schaltfläche &quot;Mit Salesforce anmelden&quot;angezeigt werden, ist Ihr Marketo-Abonnement für die Standardauthentifizierung aktiviert. Siehe [Einrichten von Marketo mit Standardauthentifizierung](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md){target="_blank"}. Sobald die Synchronisierung mit einer Reihe von Anmeldeinformationen beginnt, erfolgt kein Wechsel von Salesforce-Anmeldeinformationen oder -Abonnements. Wenn Sie Oauth 2.0 verwenden möchten, wenden Sie sich an das Adobe Account Team (Ihren Kundenbetreuer).

1. Ein Popup mit der Salesforce-Anmeldeseite wird angezeigt. Geben Sie die Anmeldedaten für Ihren Marketo Sync User ein und melden Sie sich an.

   ![](assets/setting-up-oauth-2-10.png)

1. Geben Sie den Verifikationscode ein, den Sie per E-Mail erhalten haben (von Salesforce gesendet), und klicken Sie auf **[!UICONTROL Überprüfen]**.

   ![](assets/setting-up-oauth-2-11.png)

1. Nach erfolgreicher Überprüfung wird auf der Zugriffsseite angezeigt, auf der der Zugriff angefordert wird. Klicks **[!UICONTROL Zulassen]**.

   ![](assets/setting-up-oauth-2-12.png)

1. In einigen Minuten wird ein Popup in Marketo angezeigt. Klicks **[!UICONTROL Anmeldeinformationen bestätigen]**.

   ![](assets/setting-up-oauth-2-13.png)

1. Klicken Sie nach Abschluss der Feldsynchronisierung auf **[!UICONTROL Salesforce Sync starten]**.

   ![](assets/setting-up-oauth-2-14.png)

1. Klicks **[!UICONTROL Synchronisierung starten]**.

   ![](assets/setting-up-oauth-2-15.png)

Ihre Synchronisation zwischen Marketo und Salesforce wird jetzt ausgeführt.

![](assets/setting-up-oauth-2-16.png)

>[!MORELIKETHIS]
>
* [Schritt 1 von 3: Hinzufügen von Marketo-Feldern zu Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}
* [Schritt 2 von 3: Erstellen eines Salesforce-Benutzers für Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}
* [Installieren des Marketo Sales Insight-Pakets in Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}
* [Konfigurieren von Marketo Sales Insight in Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md){target="_blank"}
