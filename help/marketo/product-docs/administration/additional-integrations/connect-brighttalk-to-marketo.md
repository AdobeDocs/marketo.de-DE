---
unique-page-id: 15695874
description: "Verbinden [!DNL BrightTALK] nach Marketo - Marketo Docs - Produktdokumentation"
title: "Verbinden [!DNL BrightTALK] nach Marketo"
exl-id: 5c6a12ec-301b-4dec-975c-24ec759ebb37
feature: Administration, Integrations
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '312'
ht-degree: 1%

---

# Verbinden [!DNL BrightTALK] zu Marketo {#connect-brighttalk-to-marketo}

Erfahren Sie, wie Sie Ihre [!DNL BrightTALK] zu Ihrer Marketo-Instanz weiterleiten. Dazu müssen Sie für beide Benutzer Administrator sein.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

## Schritte in [!DNL BrightTALK] {#steps-in-brighttalk}

1. Anmelden bei [business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login){target="_blank"} und klicken **[!UICONTROL Jetzt verbinden]**.
1. under [!UICONTROL Erweiterter Marketo Connector]klicken **[!UICONTROL Verbinden]**.
1. Sie gelangen zum Bildschirm mit den Anmeldedaten und fragen nach: Client-ID, Client-Geheimnis, Identity Service-URL und REST-Dienst-URL. Um diese Informationen zu erhalten, melden Sie sich bei Marketo an.

## Schritte in Marketo {#steps-in-marketo}

>[!NOTE]
>
>An dieser Stelle müssen Sie eine [!DNL API Only User Role] und [!DNL API User] um die Berechtigungen zu beschränken [!DNL BrightTALK] wird in Ihrer Marketo-Instanz vorhanden sein. Da wir bereits Artikel für diese Schritte haben, verknüpfen wir Sie mit ihnen.

1. Erstellen Sie eine [Nur API-Benutzerrolle](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target="_blank"}.

1. [Erstellen eines API-Benutzers](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md){target="_blank"}, wobei [!DNL BrightTALK] API-Rolle, die Sie in Schritt 4 erstellt haben.

1. Gehen Sie zurück zu **[!UICONTROL Admin]** Bereich.

   ![](assets/connect-brighttalk-to-marketo-1.png)

1. under **[!UICONTROL Integration]** klicken **[!UICONTROL LaunchPoint]**.

   ![](assets/connect-brighttalk-to-marketo-2.png)

1. Klicken Sie auf **[!UICONTROL Neu]** und wählen Sie **[!UICONTROL Neuer Dienst]**.

   ![](assets/connect-brighttalk-to-marketo-3.png)

1. Geben Sie einen **[!UICONTROL Anzeigename]** Ihrer Wahl. Klicken Sie auf **[!UICONTROL Dienst]** und wählen Sie **[!UICONTROL Benutzerdefiniert]** (do _not_ select [!DNL BrightTALK]).

   ![](assets/connect-brighttalk-to-marketo-4.png)

   >[!CAUTION]
   >
   >Nicht auswählen [!DNL BrightTALK] in der Dropdown-Liste. Es handelt sich um ein Feld, das wir derzeit entfernen, und durch seine Auswahl können bei Ihnen erhebliche Probleme auftreten. [!DNL Marketo/BrightTALK] Integration.

1. Geben Sie einen [!UICONTROL Beschreibung] Ihrer Wahl. Klicken Sie auf **[!UICONTROL Nur API-Benutzer]** und wählen Sie die [!DNL BrightTALK API User] die Sie in Schritt 5 erstellt haben. Klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/connect-brighttalk-to-marketo-5.png)

1. Klicks **[!UICONTROL Details anzeigen]** für den soeben erstellten benutzerdefinierten Dienst.

   ![](assets/connect-brighttalk-to-marketo-6.png)

1. Kopieren (und speichern) Sie die **[!UICONTROL Client-ID]** und **[!UICONTROL Client Secret]**. Klicken Sie auf **[!UICONTROL Schließen]**.

   ![](assets/connect-brighttalk-to-marketo-7.png)

1. under **[!UICONTROL Integration]** auswählen **[!UICONTROL Web-Services]**.

   ![](assets/connect-brighttalk-to-marketo-8.png)

1. under **[!UICONTROL Rest-API]**, kopieren (und speichern) Sie die **[!UICONTROL Endpunkt]** und **[!UICONTROL Identität]**.

   ![](assets/connect-brighttalk-to-marketo-9.png)

## Weitere Schritte in [!DNL BrightTALK] {#additional-steps-in-brighttalk}

1. Kehren Sie zu [!DNL BrightTALK] Bildschirm zur Einrichtung des Connectors in Schritt 3 und geben Sie die Anmeldeinformationen ein, die Sie in den Schritten 12 und 14 gespeichert haben.

Nachdem die Anmeldeinformationen authentifiziert wurden, haben Sie eine offizielle Verbindung [!DNL BrightTALK] nach Marketo. Der nächste Schritt besteht darin, [Welche Datenfelder Sie synchronisieren möchten](https://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync){target="_blank"}.
