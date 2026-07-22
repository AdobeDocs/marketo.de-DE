---
description: Erfahren Sie, wie Sie Marketo-KI-Berechtigungen aktivieren, Organisationsregeln konfigurieren und Einstellungen wie Integrationen und Benachrichtigungen verwalten.
title: Einstellungen und Setup
badge: Beta
exl-id: faf642a1-25f0-4566-b35d-074b003835ed
source-git-commit: f5228b97caf8301ca2a4360c02803d5749854b56
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 4%

---

# Einstellungen und Setup {#settings-setup}

Erfahren Sie, wie Sie Berechtigungen aktivieren und den Bereich Einstellungen verwenden, um Verbindungsdetails anzuzeigen, Organisationsregeln zu definieren und Integrationen und Benachrichtigungen einzurichten.

>[!AVAILABILITY]
>
>Diese Funktion befindet sich derzeit in der offenen Beta-Phase. Wenden Sie sich an Ihren Account Manager, um Zugriff anzufordern. Sie müssen auch den [Core Gen-AI Bedingungen und den Zusatzbedingungen](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"} zustimmen.

## Berechtigungen und Rollen {#permission-and-role}

Es gibt eine Berechtigung _Zugriff auf Marketo AI_ und eine _Marketo AI-_, die Admins eine größere Kontrolle darüber gibt, welche Benutzenden auf die **Marketo AI**-Funktion zugreifen können. Die Berechtigung wird auf Rollenebene zugewiesen. Für die Rolle _Marketo AI-_ ist die _Zugriff auf Marketo AI_ standardmäßig aktiviert.

>[!IMPORTANT]
>
>Die _Zugriff auf Marketo AI_-Berechtigung ist nicht standardmäßig für alle Rollen aktiviert. Weitere Informationen finden Sie in der folgenden Tabelle.

| Rolle | Standardstatus |
| --- | --- |
| Admin | Aktiviert |
| Adobe-Produktadministrator | Aktiviert |
| Marketingbenutzer | Deaktiviert |
| Standardbenutzer | Nicht verfügbar |
| Marketo AI-Benutzer | Aktiviert |
| Benutzerdefinierte Rollen | Deaktiviert |

### Zugriff auf Marketo AI {#access-marketo-ai-permission}

Gehen Sie wie folgt vor, um _Zugriff auf Marketo AI_ für qualifizierte Rollen zu aktivieren, für die er noch nicht aktiviert ist.

1. Klicken Sie in „Meine Marketo **auf &quot;**&quot; und dann **Benutzer und Rollen**.

   ![](assets/settings-setup-1.png)

1. Wählen Sie auf der Registerkarte _Rollen_ die gewünschte Rolle aus und klicken Sie auf **Rolle bearbeiten**.

   ![](assets/settings-setup-2.png)

1. Scrollen Sie nach unten, aktivieren Sie das Kontrollkästchen _Zugriff auf Marketo AI_ und klicken Sie auf **Speichern**.

   ![](assets/settings-setup-3.png)

   >[!NOTE]
   >
   >Sie können die gleichen Schritte zum Entfernen der Berechtigung ausführen, indem Sie **Kontrollkästchen** Zugriff auf _Marketo AI_ deaktivieren.

### Marketo AI-Benutzerrolle {#marketo-ai-user-role}

Führen Sie diese Schritte aus, um der Rolle _Marketo AI User_ einen bestimmten Benutzer zuzuweisen.

>[!NOTE]
>
>Diese Rolle **nur** enthält die Berechtigung _Zugriff auf Marketo AI_.

1. Klicken Sie in „Meine Marketo **auf &quot;**&quot; und dann **Benutzer und Rollen**.

   ![](assets/settings-setup-4.png)

1. Wählen Sie den gewünschten Benutzer aus und klicken Sie auf **Benutzer bearbeiten**.

   ![](assets/settings-setup-5.png)

1. Aktivieren _unter „Rollen und_&quot; das Kontrollkästchen _Marketo AI-_. Wenn Sie über mehr als einen Arbeitsbereich verfügen, können Sie in der Dropdown-Liste **+** festlegen, welche Arbeitsbereiche Zugriff erhalten sollen. Klicken Sie auf **Speichern**, wenn Sie fertig sind.

   ![](assets/settings-setup-6.png)

### Benutzerdefinierte Rolle {#custom-role}

Sie haben auch die Möglichkeit, [eine neue Rolle zu erstellen](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role#create-a-role){target="_blank"} ihre Berechtigungen anzupassen, indem Sie _Zugriff auf Marketo AI_ und alles andere hinzufügen, was Sie möchten, und [diese Rolle ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user){target="_blank"} bestimmten Benutzern zuweisen.

## Einstellungen {#settings}

1. Klicken Sie in „Meine Marketo&quot; auf die Kachel **[!UICONTROL Marketo AI]** .

   ![](assets/settings-setup-7.png)

1. Klicken Sie auf das Zahnradsymbol.

   ![](assets/settings-setup-8.png)

### Verbindung {#connection}

Diese Registerkarte enthält keine bearbeitbaren Felder. Es werden Kontoinformationen wie Ihre Munchkin ID und Ihre IMS-Organisation angezeigt.

![](assets/settings-setup-9.png)

### Organisationsregeln {#organizational-rules}

Definieren Sie organisatorische Richtlinien und Einschränkungen, denen die Marketo-KI beim Erstellen oder Ändern von Marketo Engage-Assets folgt.

![](assets/settings-setup-10.png){width="800" zoomable="yes"}

>[!NOTE]
>
>Regeln verwenden das Markdown-Format mit YAML-Schriftart. Globale Regeln gelten für alle Arbeitsbereiche. Workspace-Regeln überschreiben globale Einstellungen.

### Integrationen (in Kürze verfügbar) {#integrations}

Konfigurieren Sie Verbindungen zu externen Services und APIs.

_Diese Registerkarte wird möglicherweise in der Benutzeroberfläche angezeigt, ist jedoch noch nicht verfügbar. Suchen Sie nach Updates_.

### Benachrichtigungen (in Kürze verfügbar) {#notifications}

Verwalten von Warnhinweis-Voreinstellungen und Benachrichtigungskanälen.

_Diese Registerkarte wird möglicherweise in der Benutzeroberfläche angezeigt, ist jedoch noch nicht verfügbar. Bitte lesen Sie diesen Artikel für Updates_.
