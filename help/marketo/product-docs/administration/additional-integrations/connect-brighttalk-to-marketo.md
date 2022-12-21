---
unique-page-id: 15695874
description: BrightTALK mit Marketo verbinden - Marketo Docs - Produktdokumentation
title: BrightTALK mit Marketo verbinden
exl-id: 5c6a12ec-301b-4dec-975c-24ec759ebb37
source-git-commit: 5f509a7aa27692e54bf129b94c657aff0f645f2b
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 1%

---

# BrightTALK mit Marketo verbinden {#connect-brighttalk-to-marketo}

Erfahren Sie, wie Sie Ihren BrightTALK-Kanal mit Ihrer Marketo-Instanz verbinden. Dazu müssen Sie für beide Benutzer Administrator sein.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

## Schritte in BrightTALK {#steps-in-brighttalk}

1. Anmelden bei [business.brighttalk.com/demandcentral](https://business.brighttalk.com/demandcentral/login){target=&quot;_blank&quot;} und klicken Sie auf **Jetzt verbinden**.
1. Klicken Sie unter &quot;Advanced Marketo Connector&quot;auf **Verbinden**.
1. Sie gelangen zum Bildschirm mit den Anmeldedaten und fragen nach: Client-ID, Client-Geheimnis, Identity Service-URL und REST-Dienst-URL. Um diese Informationen zu erhalten, melden Sie sich bei Marketo an.

## Schritte in Marketo {#steps-in-marketo}

>[!NOTE]
>
>An dieser Stelle müssen Sie eine Nur-API-Benutzerrolle und einen API-Benutzer einrichten, um zu beschränken, welche Berechtigungen BrightTALK in Ihrer Marketo-Instanz haben wird. Da wir bereits Artikel für diese Schritte haben, verknüpfen wir Sie mit ihnen.

1. Erstellen Sie eine [Nur API-Benutzerrolle](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target=&quot;_blank&quot;}.

1. [Erstellen eines API-Benutzers](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md){target=&quot;_blank&quot;} unter Verwendung der BrightTALK-API-Rolle, die Sie in Schritt 4 erstellt haben.

1. Gehen Sie zurück zum Admin-Bereich.

   ![](assets/connect-brighttalk-to-marketo-1.png)

1. Klicken Sie unter &quot;Integration&quot;auf **LaunchPoint**.

   ![](assets/connect-brighttalk-to-marketo-2.png)

1. Klicken Sie auf **Neu** und wählen Sie **Neuer Dienst**.

   ![](assets/connect-brighttalk-to-marketo-3.png)

1. Geben Sie einen Anzeigenamen Ihrer Wahl ein. Klicken Sie auf das Dropdown-Menü Dienst und wählen Sie **Benutzerdefiniert** (do _not_ Wählen Sie BrightTALK).

   ![](assets/connect-brighttalk-to-marketo-4.png)

   >[!CAUTION]
   >
   >Denken Sie daran, BrightTALK nicht in der Dropdown-Liste auszuwählen. Es ist ein Bereich, den wir derzeit entfernen. Wenn Sie es auswählen, können erhebliche Probleme mit Ihrer Marketo/BrightTALK-Integration auftreten.

1. Geben Sie eine Beschreibung Ihrer Wahl ein. Klicken Sie auf das Dropdown-Menü Nur API-Benutzer und wählen Sie den BrightTALK-API-Benutzer aus, den Sie in Schritt 5 erstellt haben. Klicken Sie auf **Erstellen**.

   ![](assets/connect-brighttalk-to-marketo-5.png)

1. Klicken **Details anzeigen** für den soeben erstellten benutzerdefinierten Dienst.

   ![](assets/connect-brighttalk-to-marketo-6.png)

1. Kopieren (und speichern) Sie die **Client-ID** und **Client Secret**. Klicken Sie auf **Schließen**.

   ![](assets/connect-brighttalk-to-marketo-7.png)

1. Wählen Sie unter Integration die Option **Web-Services**.

   ![](assets/connect-brighttalk-to-marketo-8.png)

1. Kopieren (und speichern) Sie unter der REST-API die **Endpunkt** und **Identität**.

   ![](assets/connect-brighttalk-to-marketo-9.png)

## Zusätzliche Schritte in BrightTALK {#additional-steps-in-brighttalk}

1. Kehren Sie aus Schritt 3 zum Bildschirm zur Einrichtung des BrightTALK-Connectors zurück und geben Sie die Anmeldeinformationen ein, die Sie in den Schritten 12 und 14 gespeichert haben.

   Nachdem die Anmeldeinformationen authentifiziert wurden, haben Sie offiziell BrightTALK mit Marketo verbunden. Der nächste Schritt besteht darin, [Welche Datenfelder Sie synchronisieren möchten](https://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync){target=&quot;_blank&quot;}.
