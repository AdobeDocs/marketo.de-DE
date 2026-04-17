---
description: Erfahren Sie, wie Sie Marketo-KI-Berechtigungen aktivieren, Organisationsregeln konfigurieren und Einstellungen wie Integrationen und Benachrichtigungen verwalten.
title: Einstellungen und Setup
hide: true
hidefromtoc: true
exl-id: d6f37214-65b9-48c1-bf9f-d64b4eda87b9
source-git-commit: f26e46d4e6cb4855e5eb7f4d34a90f801e9654a7
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# Einstellungen und Setup {#settings-setup}

Erfahren Sie, wie Sie Berechtigungen aktivieren und den Bereich Einstellungen verwenden, um Verbindungsdetails anzuzeigen, Organisationsregeln zu definieren und Integrationen und Benachrichtigungen einzurichten.

## Berechtigungen {#permissions}

>[!IMPORTANT]
>
>In der Alpha-Phase der Marketo-KI _Zugriff ist standardmäßig aktiviert_ für die folgenden Rollen: Administrator, Adobe-Produktadministrator, Marketing-Benutzer, Standardbenutzer. Anstatt sie für Rollen zu aktivieren, auf die Sie Zugriff haben möchten, müssen Sie sie für Rollen deaktivieren, auf die Sie keinen Zugriff haben möchten.

### Zugriff für alle {#access-for-all}

Wenn Sie möchten, dass Marketo AI für alle oben aufgeführten Rollen aktiviert ist, müssen Sie nichts tun.

### Zugriff für einige {#access-for-some}

Gehen Sie wie folgt vor, um den Zugriff für alle Rollen zu entfernen.

1. Klicken Sie in „Meine Marketo **auf &quot;**&quot; und dann **Benutzer und Rollen**.

   ![](assets/settings-setup-1.png)

1. Wählen Sie auf der Registerkarte _Rollen_ die gewünschte Rolle aus und klicken Sie auf **Rolle bearbeiten**.

   ![](assets/settings-setup-2.png)

1. Scrollen Sie nach unten und _Sie_ Kontrollkästchen **Zugriff auf Build mit**) und klicken Sie auf **Speichern**.

   ![](assets/settings-setup-3.png)

Wiederholen Sie diese Schritte für alle anderen gewünschten Rollen.

### Benutzerdefinierte Rolle {#custom-role}

Sie haben auch die Möglichkeit, [eine neue Rolle zu erstellen](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role#create-a-role){target="_blank"} ihre Berechtigungen anzupassen, _Zugriff mit KI erstellen_ zusammen mit allem anderen, was Sie möchten, und [diese Rolle &#x200B;](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user){target="_blank"} bestimmten Benutzern zuweisen.

<!-- ## Permissions {#permissions}

In order to access Marketo AI, Admins must first enable role permissions. 

1. In your My Marketo, click **Admin**, then **Users & Roles**.

   ![](assets/settings-setup-1.png)

1. In the _Roles_ tab, select the desired role and click **Edit Role**.

   ![](assets/settings-setup-2.png)

1. Scroll down and select the **Access Build with AI** checkbox and click **Save**.

   ![](assets/settings-setup-3.png)

-->

## Einstellungen {#settings}

1. Klicken Sie in Ihrem Mein Marketo auf die Kachel **Mit KI erstellen**.

   ![](assets/settings-setup-4.png)

1. Klicken Sie auf das Zahnradsymbol.

   ![](assets/settings-setup-5.png)

### Verbindung {#connection}

Diese Registerkarte enthält keine bearbeitbaren Felder. Es werden Kontoinformationen wie Ihre Munchkin ID und Ihre IMS-Organisation angezeigt.

![](assets/settings-setup-6.png)

### Organisationsregeln {#organizational-rules}

Definieren Sie organisatorische Richtlinien und Einschränkungen, denen die Marketo-KI beim Erstellen oder Ändern von Marketo Engage-Assets folgt.

![](assets/settings-setup-7.png){width="800" zoomable="yes"}

>[!NOTE]
>
>Regeln verwenden das Markdown-Format mit YAML-Schriftart. Globale Regeln gelten für alle Arbeitsbereiche. Workspace-Regeln überschreiben globale Einstellungen.

### Integrationen (in Kürze verfügbar) {#integrations}

Konfigurieren Sie Verbindungen zu externen Services und APIs.

_Diese Registerkarte wird möglicherweise in der Benutzeroberfläche angezeigt, ist jedoch noch nicht verfügbar. Suchen Sie nach Updates_.

### Benachrichtigungen (in Kürze verfügbar) {#notifications}

Verwalten von Warnhinweis-Voreinstellungen und Benachrichtigungskanälen.

_Diese Registerkarte wird möglicherweise in der Benutzeroberfläche angezeigt, ist jedoch noch nicht verfügbar. Suchen Sie nach Updates_.
