---
unique-page-id: 7513771
description: Anmeldung und Benutzerverwaltung - Marketo-Dokumente - Produktdokumentation
title: Anmelden und Benutzerverwaltung
exl-id: 3cf5a50a-1926-4fb6-a1fe-39ba5eb2560f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# Anmelden und Benutzerverwaltung {#login-and-user-management}

## Erstellen einer Web-Personalisierung-Benutzerrolle {#create-a-web-personalization-user-role}

1. Navigieren Sie zu **Admin** und klicken Sie auf **Benutzer und Rollen**.

   ![](assets/image2015-4-28-19-3a50-3a49.png)

1. Klicken **Rollen**.

   ![](assets/image2015-4-28-19-3a57-3a58.png)

   >[!NOTE]
   >
   >Wenn die Web Personalization (WP)-Benutzerrolle bereits vorhanden ist, stellen Sie sicher, dass sie wie in Schritt 4 gezeigt konfiguriert ist.

1. Klicken **Neue Rolle**.

   ![](assets/three-1.png)

1. Geben Sie einen Rollennamen ein und wählen Sie Berechtigungen aus. Klicken **Erstellen** (Diese Rolle muss [auf alle Arbeitsbereiche anwenden](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md)).

   ![](assets/four.png)

   >[!TIP]
   >
   >Um Benutzern Zugriff auf alles in Targeting und Personalisierung zu gewähren, wählen Sie _all_ die Kontrollkästchen.

## Web-Personalisierung und Benutzerberechtigungen für prädiktive Inhalte {#web-personalization-and-predictive-content-user-permissions}

**Targeting und Personalisierung**: Benutzer hat nur Anzeigeberechtigungen, wenn diese Berechtigung nur ausgewählt ist.

**Admin Web Personalization + Predictive**: Der Benutzer hat nur Zugriff auf die Kontoeinstellungen und Inhaltseinstellungen für die Web-Personalisierung und die Predictive Content-App. Benutzer können Seiten in der App anzeigen, haben jedoch keine Berechtigungen zum Erstellen, Bearbeiten, Löschen und Starten.

**Predictive Content Editor**: Der Benutzer hat Editor-Zugriff auf die App &quot;Predictive Content&quot;. Die Berechtigung ermöglicht das Erstellen, Bearbeiten und Löschen von Inhaltselementen. Inhalte können nicht für die prädiktive Verwendung im Web oder in E-Mails aktiviert werden.

**Predictive Content Launcher**: Der Benutzer hat Zugriff auf alle Funktionen für prädiktive Inhalte mit Ausnahme der Konto- und Inhaltseinstellungen. Mit dieser Berechtigung können Sie Inhaltselemente erstellen, bearbeiten, löschen und aktivieren.

**Web-Campaign-Editor**: Der Benutzer hat Editor Zugriff auf alle Funktionen zur Web-Personalisierung, um Webkampagnen zu erstellen, zu bearbeiten und zu löschen, aber nicht zu starten.

**Web Campaign Launcher**: Der Benutzer hat Zugriff auf alle Funktionen der Web Personalization-App, mit Ausnahme der Konto- und Inhaltseinstellungen. Mit dieser Berechtigung können Sie Webkampagnen erstellen, bearbeiten, löschen und starten.

## WP-Rolle Benutzern zuweisen {#assign-wp-role-to-user}

1. Navigieren Sie zu **Benutzer**.

   ![](assets/image2015-4-29-11-3a31-3a3.png)

1. Wählen Sie den Benutzer aus, dem WP-Zugriff gewährt werden soll, und klicken Sie auf **Benutzer bearbeiten**.

   ![](assets/image2015-4-29-11-3a38-3a46.png)

1. Wählen Sie die WP-Benutzerrolle für alle Arbeitsbereiche aus.

   ![](assets/seven.png)

1. Neu aktivierte Benutzer sehen die **Web-Personalisierung** in My Marketo beim nächsten Anmelden.

   ![](assets/eight.png)
