---
description: Erfahren Sie, wie Sie Berechtigungen für Coworker for Marketo Engage aktivieren, Organisationsregeln konfigurieren und Einstellungen wie Integrationen und Benachrichtigungen verwalten.
title: Einstellungen und Setup
source-git-commit: 01cad5c7d14083c0ef7127850f2488dbfd71f57b
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 3%

---

# Einstellungen und Setup {#settings-setup}

Erfahren Sie, wie Sie Berechtigungen aktivieren und den Bereich Einstellungen verwenden, um Verbindungsdetails anzuzeigen, Organisationsregeln zu definieren und Integrationen und Benachrichtigungen einzurichten.

>[!AVAILABILITY]
>
>Diese Funktion steht allen Abonnements zur Verfügung. Wenn die Kachel „Mitarbeiter für Marketo Engage&quot; auf Ihrem Bildschirm „Mein Marketo&quot; nicht angezeigt wird, wenden Sie sich an Ihren Kundenbetreuer. Sie müssen auch den [Core Gen-AI Bedingungen und den Zusatzbedingungen](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"} zustimmen.

## Berechtigungen und Rollen {#permission-and-role}

Es gibt eine Berechtigung _Zugriffskollege für Marketo Engage_ und eine Rolle _Mitarbeiter für Marketo Engage-Benutzer_, die Admins größere Kontrolle darüber gibt, welche Benutzenden auf die Funktion **Mitarbeiter für Marketo Engage** zugreifen können. Die Berechtigung wird auf Rollenebene zugewiesen. Die Rolle _Mitarbeiter für Marketo Engage-Benutzer_ verfügt standardmäßig über die Berechtigung _Zugriff auf Mitarbeiter für Marketo Engage_ .

>[!NOTE]
>
>Die Berechtigung _Zugriff auf Mitarbeiter für Marketo Engage_ ist nicht standardmäßig für alle Rollen aktiviert. Weitere Informationen finden Sie in der folgenden Tabelle.

| Rolle | Standardstatus |
| --- | --- |
| Admin | Aktiviert |
| Adobe-Produktadministrator | Aktiviert |
| Marketingbenutzer | Deaktiviert |
| Standardbenutzer | Nicht verfügbar |
| Mitarbeiter für Marketo Engage-Benutzer | Aktiviert |
| Benutzerdefinierte Rollen | Deaktiviert |

### Berechtigung „Zugriff auf Mitarbeiter für Marketo Engage&quot; {#access-coworker-marketo-permission}

Gehen Sie wie folgt vor, um _Access Coworker for Marketo Engage_ für qualifizierte Rollen zu aktivieren, für die er noch nicht aktiviert ist.

1. Klicken Sie in „Meine Marketo **auf &quot;**&quot; und dann **Benutzer und Rollen**.

   ![](assets/settings-setup-1.png)

1. Wählen Sie auf der Registerkarte _Rollen_ die gewünschte Rolle aus und klicken Sie auf **Rolle bearbeiten**.

   ![](assets/settings-setup-2.png)

1. Scrollen Sie nach unten, aktivieren Sie das Kontrollkästchen _Access Coworker for Marketo Engage_ und klicken Sie auf **Speichern**.

   ![](assets/settings-setup-3.png)

   >[!NOTE]
   >
   >Sie können mit denselben Schritten die Berechtigung entfernen, indem Sie **Kontrollkästchen** Zugriff auf _für Marketo Engage_ deaktivieren.

### Mitarbeiter für Marketo Engage-Benutzerrolle {#coworker-marketo-user-role}

Führen Sie diese Schritte aus, um der Rolle _Mitarbeiter für Marketo Engage-Benutzer“ einen bestimmten_ zuzuweisen.

>[!NOTE]
>
>Diese Rolle **nur** enthält die Berechtigung _Zugriff auf Mitarbeiter für Marketo Engage_.

1. Klicken Sie in „Meine Marketo **auf &quot;**&quot; und dann **Benutzer und Rollen**.

   ![](assets/settings-setup-4.png)

1. Wählen Sie den gewünschten Benutzer aus und klicken Sie auf **Benutzer bearbeiten**.

   ![](assets/settings-setup-5.png)

1. Aktivieren _in „Rollen_ Arbeitsbereiche“ das Kontrollkästchen _Mitarbeiter für Marketo Engage-_&quot;. Wenn Sie über mehr als einen Arbeitsbereich verfügen, können Sie in der Dropdown-Liste **+** festlegen, welche Arbeitsbereiche Zugriff erhalten sollen. Klicken Sie auf **Speichern**, wenn Sie fertig sind.

   ![](assets/settings-setup-6.png)

### Benutzerdefinierte Rolle {#custom-role}

Sie haben auch die Möglichkeit, [eine neue Rolle zu erstellen](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role#create-a-role){target="_blank"} ihre Berechtigungen anzupassen, indem Sie _Access Coworker for Marketo Engage_ und alles andere hinzufügen, was Sie möchten, und [diese Rolle &#x200B;](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user){target="_blank"} bestimmten Benutzern zuweisen.

## Einstellungen {#settings}

1. Klicken Sie in My Marketo auf die Kachel **[!UICONTROL Mitarbeiter für Marketo Engage]**.

   ![](assets/settings-setup-7.png)

1. Klicken Sie auf das Zahnradsymbol.

   ![](assets/settings-setup-8.png)

### Verbindung {#connection}

Diese Registerkarte enthält keine bearbeitbaren Felder. Es werden Kontoinformationen wie Ihre Munchkin ID und IMS-Organisation angezeigt.

![](assets/settings-setup-9.png)

### Organisationsregeln {#organizational-rules}

Definieren Sie organisatorische Richtlinien und Einschränkungen, denen der Mitarbeiter für Marketo Engage beim Erstellen oder Ändern von Marketo Engage-Assets folgt.

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
