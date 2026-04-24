---
description: Erfahren Sie, wie Sie Marketo-KI-Berechtigungen aktivieren, Organisationsregeln konfigurieren und Einstellungen wie Integrationen und Benachrichtigungen verwalten.
title: Einstellungen und Setup
beta: true
exl-id: faf642a1-25f0-4566-b35d-074b003835ed
source-git-commit: 6a46070308e79bc3799b2da92962b5a3a2f73ce9
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 3%

---

# Einstellungen und Setup {#settings-setup}

Erfahren Sie, wie Sie Berechtigungen aktivieren und den Bereich Einstellungen verwenden, um Verbindungsdetails anzuzeigen, Organisationsregeln zu definieren und Integrationen und Benachrichtigungen einzurichten.

>[!NOTE]
>
>Diese Funktion befindet sich in der offenen Beta-Phase und wird in den nächsten Monaten schrittweise eingeführt. Wenn die Kachel „Mit KI erstellen“ auf dem Bildschirm &quot;_Marketo&quot; angezeigt wird, erfahren Sie, wann_ für Ihr Abonnement aktiviert wurde.

## Berechtigungen und Rollen {#permission-and-role}

Es gibt einen _Build mit KI_-Berechtigung und eine _Build mit KI-Benutzer_-Rolle, die Admins größere Kontrolle darüber gibt, welche Benutzer auf die Funktion **Build mit KI** zugreifen können. Die Berechtigung wird auf Rollenebene zugewiesen. Die Rolle _Build with AI User_ verfügt standardmäßig über die Berechtigung _Zugriff auf Build mit_-Funktion .

>[!IMPORTANT]
>
>Die _Zugriff Build mit KI_-Berechtigung ist nicht standardmäßig für alle Rollen aktiviert. Weitere Informationen finden Sie in der folgenden Tabelle.

| Rolle | Standardstatus |
| --- | --- |
| Admin | Aktiviert |
| Adobe-Produktadministrator | Aktiviert |
| Marketingbenutzer | Deaktiviert |
| Standardbenutzer | Nicht verfügbar |
| Erstellen mit KI-Benutzenden | Aktiviert |
| Benutzerdefinierte Rollen | Deaktiviert |

### Zugriff auf Build mit KI-Berechtigung {#access-build-with-ai-permission}

Gehen Sie wie folgt vor, um _Zugriff erstellen mit KI_ für qualifizierte Rollen zu aktivieren, für die er noch nicht aktiviert ist.

1. Klicken Sie in „Meine Marketo **auf &quot;**&quot; und dann **Benutzer und Rollen**.

   ![](assets/settings-setup-1.png)

1. Wählen Sie auf der Registerkarte _Rollen_ die gewünschte Rolle aus und klicken Sie auf **Rolle bearbeiten**.

   ![](assets/settings-setup-2.png)

1. Scrollen Sie nach unten, aktivieren Sie das Kontrollkästchen _Zugriff auf Build mit_) und klicken Sie auf **Speichern**.

   ![](assets/settings-setup-3.png)

   >[!NOTE]
   >
   >Sie können die gleichen Schritte zum Entfernen der Berechtigung ausführen, indem Sie **Kontrollkästchen** Zugriff _KI_ deaktivieren.

### Mit KI-Benutzerrolle erstellen {#build-with-ai-user-role}

Führen Sie diese Schritte aus, um der Rolle _Erstellen mit KI-Benutzer_ einen bestimmten Benutzer zuzuweisen.

>[!NOTE]
>
>Diese Rolle **nur** enthält die Berechtigung _Zugriff auf Build mit KI_.

1. Klicken Sie in „Meine Marketo **auf &quot;**&quot; und dann **Benutzer und Rollen**.

   ![](assets/settings-setup-1.png)

1. Wählen Sie den gewünschten Benutzer aus und klicken Sie auf **Benutzer bearbeiten**.

   ![](assets/settings-setup-5b.png)

1. Aktivieren _in „Rollen_ Arbeitsbereiche“ das Kontrollkästchen _Mit KI-Benutzer erstellen_. Wenn Sie über mehr als einen Arbeitsbereich verfügen, können Sie in der Dropdown-Liste **+** festlegen, welche Arbeitsbereiche Zugriff erhalten sollen. Klicken Sie auf **Speichern**, wenn Sie fertig sind.

   ![](assets/settings-setup-6b.png)

### Benutzerdefinierte Rolle {#custom-role}

Sie haben auch die Möglichkeit, [eine neue Rolle zu erstellen](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role#create-a-role){target="_blank"} ihre Berechtigungen anzupassen, _Zugriff mit KI erstellen_ zusammen mit allem anderen, was Sie möchten, und [diese Rolle ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user){target="_blank"} bestimmten Benutzern zuweisen.

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
