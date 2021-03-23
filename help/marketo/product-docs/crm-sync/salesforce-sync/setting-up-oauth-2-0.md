---
description: Einrichten von OAuth 2.0 - Marketing Docs - Produktdokumentation
title: Einrichten von OAuth 2.0
translation-type: tm+mt
source-git-commit: 2d03d93e120c8b3ce359c6aca44730cfa7c16bf9
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---


# Einrichten von OAuth 2.0 {#setting-up-oauth-2-0}

Salesforce verwendet das OAuth-Protokoll, um Benutzern von Anwendungen den sicheren Zugriff (Authentifizierung der Anwendung mit OAuth 2.0) auf Daten über REST-API-Aufrufe zu ermöglichen, ohne Anmeldeinformationen anzuzeigen. Im Folgenden werden die Schritte beschrieben, die ausgeführt werden müssen, um Marketo sicher mit Salesforce zu verbinden und zu synchronisieren.

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
>* Marketo Sync Benutzer muss in Salesforce erstellt werden.
>* Für bestehende Kunden ist die Funktion &quot;OAuth für SFDC-Synchronisierung aktivieren&quot;auf dem Abonnement des Kunden aktiviert.
>* Popup-Blocker sind deaktiviert.
>* Es wird eine verbundene App erstellt und die Consumer key und Consumer secret stehen zur Verwendung bereit.


1. Klicken Sie im Abschnitt Marketing-Admin auf **CRM** und dann **Mit Salesforce** synchronisieren.

   ![](assets/setting-up-oauth-2-7.png)

1. hinzufügen Sie die zuvor aufgezeichneten Consumer key- und Consumer secret-Informationen und klicken Sie auf und **Speichern**.

   ![](assets/setting-up-oauth-2-8.png)

1. Klicken Sie auf der Synchronisierungsseite von Marketo Salesforce auf die Schaltfläche **Mit Salesforce** anmelden.

   ![](assets/setting-up-oauth-2-9.png)

1. Ein Popup mit der Anmeldeseite salesforce wird angezeigt. Geben Sie die Anmeldedaten für &quot;Benutzer synchronisieren&quot; ein und melden Sie sich an.

   ![](assets/setting-up-oauth-2-10.png)

1. Geben Sie den Bestätigungscode ein, den Sie per E-Mail erhalten haben (gesendet von Salesforce), und klicken Sie auf **Verify**.

   ![](assets/setting-up-oauth-2-11.png)

1. Nach erfolgreicher Überprüfung wird die Zugriffsseite angezeigt, auf der der Zugriff angefordert wird. Klicken Sie auf **Allow**.

   ![](assets/setting-up-oauth-2-12.png)

1. In wenigen Minuten erscheint ein Popup in Marketo. Klicken Sie auf **Anmeldeinformationen** bestätigen.

   ![](assets/setting-up-oauth-2-13.png)

1. Klicken Sie nach Abschluss der Feldsynchronisierung auf **Beginn Salesforce Sync**.

   ![](assets/setting-up-oauth-2-14.png)

1. Klicken Sie auf **Beginn-Synchronisierung**.

   ![](assets/setting-up-oauth-2-15.png)

Ihre Synchronisierung zwischen Marketo und Salesforce läuft.

![](assets/setting-up-oauth-2-16.png)
