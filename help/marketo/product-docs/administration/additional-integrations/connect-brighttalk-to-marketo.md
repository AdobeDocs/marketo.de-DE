---
unique-page-id: 15695874
description: "Verbinden [!DNL BrightTALK] mit Marketo - Marketo Docs - Produktdokumentation"
title: "Connect [!DNL BrightTALK] to Marketo"
exl-id: 5c6a12ec-301b-4dec-975c-24ec759ebb37
feature: Administration, Integrations
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 1%

---

# [!DNL BrightTALK] mit Marketo verbinden {#connect-brighttalk-to-marketo}

Erfahren Sie, wie Sie Ihren [!DNL BrightTALK]-Kanal mit Ihrer Marketo-Instanz verbinden. Dazu müssen Sie für beide Benutzer Administrator sein.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

## Schritte in [!DNL BrightTALK] {#steps-in-brighttalk}

1. Melden Sie sich bei [business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login){target="_blank"} an und klicken Sie auf **[!UICONTROL Jetzt verbinden]**.
1. Klicken Sie unter [!UICONTROL Erweiterter Marketo-Connector] auf **[!UICONTROL Verbinden]**.
1. Sie gelangen zum Bildschirm mit den Anmeldedaten und fragen nach: Client-ID, Client-Geheimnis, Identity Service-URL und REST-Dienst-URL. Um diese Informationen zu erhalten, melden Sie sich bei Marketo an.

## Schritte in Marketo {#steps-in-marketo}

>[!NOTE]
>
>An dieser Stelle müssen Sie eine [!DNL API Only User Role] und eine [!DNL API User] einrichten, um zu beschränken, welche Berechtigungen [!DNL BrightTALK] in Ihrer Marketo-Instanz haben. Da wir bereits Artikel für diese Schritte haben, verknüpfen wir Sie mit ihnen.

1. Erstellen Sie eine [Nur API-Benutzerrolle](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target="_blank"}.

1. [Erstellen Sie einen API-Benutzer ](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md){target="_blank"} mit der [!DNL BrightTALK] API-Rolle, die Sie in Schritt 4 erstellt haben.

1. Gehen Sie zurück zum Bereich **[!UICONTROL Admin]** .

   ![](assets/connect-brighttalk-to-marketo-1.png)

1. Klicken Sie unter **[!UICONTROL Integration]** auf **[!UICONTROL LaunchPoint]**.

   ![](assets/connect-brighttalk-to-marketo-2.png)

1. Klicken Sie auf die Dropdownliste **[!UICONTROL Neu]** und wählen Sie **[!UICONTROL Neuer Dienst]** aus.

   ![](assets/connect-brighttalk-to-marketo-3.png)

1. Geben Sie einen **[!UICONTROL Anzeigenamen]** Ihrer Wahl ein. Klicken Sie auf das Dropdown-Menü **[!UICONTROL Dienst]** und wählen Sie **[!UICONTROL Benutzerdefiniert]** aus (wählen Sie _nicht_ [!DNL BrightTALK] aus).

   ![](assets/connect-brighttalk-to-marketo-4.png)

   >[!CAUTION]
   >
   >Denken Sie daran, in der Dropdown-Liste nicht &quot;[!DNL BrightTALK]&quot;auszuwählen. Es handelt sich um ein Feld, das wir derzeit entfernen. Wenn Sie es auswählen, kann dies zu erheblichen Problemen mit Ihrer [!DNL Marketo/BrightTALK] -Integration führen.

1. Geben Sie eine [!UICONTROL Beschreibung] Ihrer Wahl ein. Klicken Sie auf das Dropdown-Menü **[!UICONTROL Nur API-Benutzer]** und wählen Sie die [!DNL BrightTALK API User] aus, die Sie in Schritt 5 erstellt haben. Klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/connect-brighttalk-to-marketo-5.png)

1. Klicken Sie für den soeben erstellten benutzerdefinierten Dienst auf **[!UICONTROL Details anzeigen]** .

   ![](assets/connect-brighttalk-to-marketo-6.png)

1. Kopieren (und speichern) Sie die **[!UICONTROL Client-ID]** und den **[!UICONTROL Client-Geheimnis]**. Klicken Sie auf **[!UICONTROL Schließen]**.

   ![](assets/connect-brighttalk-to-marketo-7.png)

1. Wählen Sie unter **[!UICONTROL Integration]** die Option **[!UICONTROL Webdienste]** aus.

   ![](assets/connect-brighttalk-to-marketo-8.png)

1. Kopieren Sie unter **[!UICONTROL Rest-API]** die **[!UICONTROL Endpunkt]** und die **[!UICONTROL Identität]** und speichern Sie sie.

   ![](assets/connect-brighttalk-to-marketo-9.png)

## Zusätzliche Schritte in [!DNL BrightTALK] {#additional-steps-in-brighttalk}

1. Kehren Sie aus Schritt 3 zum Bildschirm zur Einrichtung des [!DNL BrightTALK] -Connectors zurück und geben Sie die Anmeldeinformationen ein, die Sie in den Schritten 12 und 14 gespeichert haben.

Nachdem die Anmeldeinformationen authentifiziert wurden, haben Sie offiziell [!DNL BrightTALK] mit Marketo verbunden. Der nächste Schritt besteht darin, [zu bestimmen, welche Datenfelder Sie synchronisieren möchten](https://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync){target="_blank"}.
