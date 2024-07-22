---
description: Einrichten der ON24-Integration mit Marketo - Marketo Docs - Produktdokumentation
title: ON24-Integration mit Marketo einrichten
exl-id: 395ffa37-b87d-4eb4-bf9f-72aa96dc819c
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 1%

---

# ON24-Integration mit Marketo einrichten{#set-up-the-on24-integration-with-marketo}

Hier erfahren Sie, wie Sie Ihre ON24-Ereignisintegration einrichten.

## Erstellen einer Nur-API-Rolle {#create-an-api-only-role}

1. Klicken Sie in My Marketo auf **Admin**.

   ![](assets/set-up-the-on24-integration-with-marketo-1.png)

1. Klicken Sie unter &quot;Security&quot;auf **Users &amp; Roles**.

   ![](assets/set-up-the-on24-integration-with-marketo-2.png)

1. Klicken Sie auf die Registerkarte **Rollen** und dann auf **Neue Rolle**.

   ![](assets/set-up-the-on24-integration-with-marketo-3.png)

1. Geben Sie einen Rollennamen ein. Öffnen Sie das Menü **Access API** und wählen Sie &quot;Read-Write Custom Object&quot;und &quot;Read-Write Person&quot;. Klicken Sie auf **Erstellen**.

   ![](assets/set-up-the-on24-integration-with-marketo-4.png)

## Neuen Benutzer erstellen {#create-a-new-user}

1. Klicken Sie in &quot;Benutzer und Rollen&quot;auf die Registerkarte **Benutzer** und klicken Sie auf **Neuen Benutzer einladen**.

   ![](assets/set-up-the-on24-integration-with-marketo-5.png)

1. Geben Sie die Informationen des neuen Benutzers ein und klicken Sie auf **Weiter**.

   ![](assets/set-up-the-on24-integration-with-marketo-6.png)

1. Wählen Sie die soeben erstellte Rolle Nur ON24-API aus. Aktivieren Sie das Kontrollkästchen **Nur API** . Klicken Sie auf **Weiter**.

   ![](assets/set-up-the-on24-integration-with-marketo-7.png)

1. Klicken Sie auf **Senden**.

   ![](assets/set-up-the-on24-integration-with-marketo-8.png)

>[!NOTE]
>
>Eine Einladung ist nicht für Benutzer erforderlich, die nur über die API verfügen.

## ON24-Verbindung einrichten {#set-up-on24-connection}

1. Klicken Sie im Abschnitt &quot;Admin&quot;auf **LaunchPoint**.

   ![](assets/set-up-the-on24-integration-with-marketo-9.png)

1. Klicken Sie auf **Neu** und dann auf **Neuer Dienst**.

   ![](assets/set-up-the-on24-integration-with-marketo-10.png)

1. Wählen Sie einen Anzeigenamen aus. Klicken Sie auf das Dropdown-Menü **Dienst** und wählen Sie **Benutzerdefiniert** aus. Geben Sie eine Beschreibung ein. Klicken Sie auf das Dropdown-Menü &quot;Nur API-Benutzer&quot;und wählen Sie den Benutzer aus, den Sie in den Schritten oben ](#create-a-new-user) [erstellt haben. Klicken Sie auf **Erstellen**.

   ![](assets/set-up-the-on24-integration-with-marketo-11.png)

1. Suchen Sie den soeben erstellten benutzerdefinierten LaunchPoint-Dienst und klicken Sie auf Details anzeigen .

   ![](assets/set-up-the-on24-integration-with-marketo-12.png)

1. Markieren Sie die Client-ID, klicken Sie mit der rechten Maustaste darauf, kopieren Sie sie und speichern Sie sie (Sie benötigen sie später). Wiederholen Sie dies für Client Secret .

   ![](assets/set-up-the-on24-integration-with-marketo-13.png)

1. Klicken Sie links in der Baumstruktur auf Web Services.

   ![](assets/set-up-the-on24-integration-with-marketo-14.png)

1. Markieren Sie unter &quot;REST API&quot;den ersten Teil der Identität (bis &quot;m&quot;in .com), klicken Sie mit der rechten Maustaste darauf, kopieren Sie ihn und speichern Sie ihn.

   ![](assets/set-up-the-on24-integration-with-marketo-15.png)

1. Navigieren Sie mit Ihrer gespeicherten Client-ID, Ihrem Client-Geheimnis und Ihrer Identität zu Ihrem ON24-Konto. Die restlichen Schritte werden dort ausgeführt und sind hier ](https://on24support.force.com/Support/s/article/Connect-Marketo-ON24-Connect-Data-Integration#Step6){target="_blank"} beschrieben.[
