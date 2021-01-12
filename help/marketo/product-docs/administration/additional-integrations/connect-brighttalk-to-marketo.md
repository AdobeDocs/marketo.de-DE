---
unique-page-id: 15695874
description: BrightTALK mit Marketo - Marketing Docs - Produktdokumentation verbinden
title: BrightTALK mit Marketo verbinden
translation-type: tm+mt
source-git-commit: 78961a3e163ce903facf955a9dda6909b5e85bad
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---


# BrightTALK mit Marketo verbinden {#connect-brighttalk-to-marketo}

Erfahren Sie, wie Sie Ihren BrightTALK-Kanal mit Ihrer Marketo-Instanz verbinden. Um dies zu tun, müssen Sie Administrator für beide sein.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

## Schritte in BrightTALK {#steps-in-brighttalk}

1. Melden Sie sich bei [business.brighttalk.com/demandcentral](http://business.brighttalk.com/demandcentral/login) an und klicken Sie auf **Jetzt verbinden**.
1. Klicken Sie unter &quot;Erweiterter Marketing-Connector&quot;auf **Connect**.
1. Sie gelangen zum Anmeldebildschirm, in dem Sie nach Folgendem gefragt werden: Client-ID, geheimer Clientschlüssel, Identitätsdienst-URL und REST-Dienst-URL. Um diese Informationen zu erhalten, melden Sie sich bei Marketo an.

## Schritte in Marketo {#steps-in-marketo}

>[!NOTE]
>
>An dieser Stelle müssen Sie eine Nur-Benutzer-API-Rolle und einen API-Benutzer einrichten, um die Berechtigungen von BrightTALK in Ihrer Marketo-Instanz einzuschränken. Da wir bereits Artikel für diese Schritte haben, werden wir Sie mit ihnen verknüpfen.

1. Erstellen Sie eine Benutzerrolle [Nur API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md).
1. [Erstellen Sie einen API-Benutzer](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md) mit der BrightTALK API-Rolle, die Sie in Schritt 4 erstellt haben.
1. Gehen Sie zurück zum Admin-Bereich.

   ![](assets/one.png)

1. Klicken Sie unter Integration auf **LaunchPoint**.

   ![](assets/two.png)

1. Klicken Sie auf die Dropdownliste **Neu** und wählen Sie **Neuer Dienst**.

   ![](assets/three.png)

1. Geben Sie einen Anzeigenamen Ihrer Wahl ein. Klicken Sie auf die Dropdown-Liste Dienst und wählen Sie **Benutzerdefiniert** (do _not_ select BrightTALK).

   ![](assets/four.png)

   >[!CAUTION]
   >
   >Denken Sie daran, BrightTALK nicht in der Dropdown-Liste auszuwählen. Es ist ein Bereich, den wir gerade entfernen, und die Auswahl dieses Bereichs könnte zu erheblichen Problemen mit Ihrer Integration von Marketo/BrightTALK führen.

1. Geben Sie eine Beschreibung Ihrer Wahl ein. Klicken Sie auf die Dropdown-Liste &quot;Nur API-Benutzer&quot;und wählen Sie den BrightTALK-API-Benutzer aus, den Sie in Schritt 5 erstellt haben. Klicken Sie auf **Erstellen**.

   ![](assets/five.png)

1. Klicken Sie für den soeben erstellten benutzerdefinierten Dienst auf **Ansicht Details**.

   ![](assets/six.png)

1. Kopieren (und speichern) Sie die **Client-ID** und **geheimer Clientschlüssel**. Klicken Sie auf **Schließen**.

   ![](assets/eight-1.png)

1. Wählen Sie unter Integration **Web-Services**.

   ![](assets/nine-1.png)

1. Kopieren (und speichern) Sie unter &quot;Rest-API&quot;den **Endpunkt** und **Identität**.

   ![](assets/ten.png)

## Weitere Schritte in BrightTALK {#additional-steps-in-brighttalk}

1. Kehren Sie in Schritt 3 zum Setup-Bildschirm für den BrightTALK Connector zurück und geben Sie die Anmeldeinformationen ein, die Sie in den Schritten 12 und 14 gespeichert haben.

   Nachdem die Anmeldeinformationen authentifiziert wurden, haben Sie BrightTALK offiziell mit Marketo verbunden. Der nächste Schritt besteht darin, [zu bestimmen, welche Datenfelder synchronisiert werden sollen.](http://support.brighttalk.com/hc/en-us/articles/115005131274-BrightTALK-Connector-for-Marketo-Choose-the-Fields-to-Sync)
