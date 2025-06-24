---
description: Einrichten der ON24-Integration mit Marketo - Dokumentation zu Marketo
title: Einrichten der ON24-Integration mit Marketo
exl-id: 395ffa37-b87d-4eb4-bf9f-72aa96dc819c
feature: Events
source-git-commit: e3f61755dccd9bea1378a429fc428b440fc3ecb4
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 3%

---

# Einrichten der ON24-Integration mit Marketo{#set-up-the-on24-integration-with-marketo}

So richten Sie Ihre ON24-Ereignisintegration ein.

## Nur API-Rolle erstellen {#create-an-api-only-role}

1. Klicken Sie in My Marketo auf **Admin**.

   ![](assets/set-up-the-on24-integration-with-marketo-1.png)

1. Klicken Sie unter Sicherheit auf **Benutzer und Rollen**.

   ![](assets/set-up-the-on24-integration-with-marketo-2.png)

1. Klicken Sie auf **Rollen** und dann auf **Neue Rolle**.

   ![](assets/set-up-the-on24-integration-with-marketo-3.png)

1. Geben Sie einen Rollennamen ein. Öffnen Sie das **Zugriff-API** Menü und wählen Sie „Benutzerdefiniertes Objekt mit Lese-/Schreibzugriff“ und „Person mit Lese-/Schreibzugriff“ aus. Klicken Sie auf **Erstellen**.

   ![](assets/set-up-the-on24-integration-with-marketo-4.png)

## Neuen Benutzer erstellen {#create-a-new-user}

1. Klicken Sie noch in „Benutzer und Rollen“ auf die Registerkarte **Benutzer** und klicken Sie auf **Neuen Benutzer einladen**.

   ![](assets/set-up-the-on24-integration-with-marketo-5.png)

1. Geben Sie die Informationen des neuen Benutzers ein und klicken Sie auf **Weiter**.

   ![](assets/set-up-the-on24-integration-with-marketo-6.png)

1. Wählen Sie die Rolle Nur ON24-API aus, die Sie soeben erstellt haben. Aktivieren Sie das **Nur API**-Kontrollkästchen. Klicken Sie auf **Weiter**.

   ![](assets/set-up-the-on24-integration-with-marketo-7.png)

1. Klicken Sie auf **Senden**.

   ![](assets/set-up-the-on24-integration-with-marketo-8.png)

>[!NOTE]
>
>Eine Einladung ist nicht erforderlich für Benutzende, die nur über eine API verfügen.

## Einrichten der ON24-Verbindung {#set-up-on24-connection}

1. Klicken Sie noch im Admin-Bereich auf **LaunchPoint**.

   ![](assets/set-up-the-on24-integration-with-marketo-9.png)

1. Klicken Sie **Neu** und dann **Neuer Service**.

   ![](assets/set-up-the-on24-integration-with-marketo-10.png)

1. Wählen Sie einen Anzeigenamen aus. Klicken Sie auf die **Dienst** und wählen Sie **Benutzerdefiniert**. Beschreibung eingeben. Klicken Sie auf die Dropdown-Liste Nur API-Benutzer und wählen Sie den von Ihnen erstellten Benutzer [in den oben genannten Schritten](#create-a-new-user). Klicken Sie auf **Erstellen**.

   ![](assets/set-up-the-on24-integration-with-marketo-11.png)

1. Suchen Sie den soeben erstellten benutzerdefinierten LaunchPoint-Service und klicken Sie auf Details anzeigen .

   ![](assets/set-up-the-on24-integration-with-marketo-12.png)

1. Markieren Sie die Client-ID, klicken Sie mit der rechten Maustaste darauf, kopieren Sie sie und speichern Sie sie (Sie benötigen sie später). Wiederholung für Client-Geheimnis.

   ![](assets/set-up-the-on24-integration-with-marketo-13.png)

1. Klicken Sie in der Struktur auf der linken Seite auf Web-Services .

   ![](assets/set-up-the-on24-integration-with-marketo-14.png)

1. Markieren Sie unter „REST API“ den ersten Teil der Identität (bis zum „m“ in .com), klicken Sie mit der rechten Maustaste darauf, kopieren Sie ihn und speichern Sie ihn.

   ![](assets/set-up-the-on24-integration-with-marketo-15.png)

1. Navigieren Sie mit Ihrer gespeicherten Client-ID, Ihrem Client-Geheimnis und Ihrer Identität zu Ihrem ON24-Konto. Die restlichen Schritte werden dort ausgeführt und finden Sie in der [ON24-Dokumentation](https://support.on24.com/hc/en-us/articles/21420762650523-Data-Integration-Setup-Instructions-When-Using-Marketo-Registration-Option-1){target="_blank"}.
