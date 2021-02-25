---
unique-page-id: 7513771
description: Anmeldung und Benutzerverwaltung - Marketing Docs - Produktdokumentation
title: Anmelden und Benutzerverwaltung
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---


# Anmelden und Benutzerverwaltung {#login-and-user-management}

## Eine Web-Personalisierung-Benutzerrolle {#create-a-web-personalization-user-role} erstellen

1. Wechseln Sie zum Abschnitt **Admin** und klicken Sie dann auf **Benutzer und Rollen**.

   ![](assets/image2015-4-28-19-3a50-3a49.png)

1. Klicken Sie auf **Rollen**.

   ![](assets/image2015-4-28-19-3a57-3a58.png)

   >[!NOTE]
   >
   >Wenn die Benutzerrolle &quot;Web Personalization (WP)&quot;bereits vorhanden ist, stellen Sie sicher, dass sie wie in Schritt 4 gezeigt konfiguriert ist.

1. Klicken Sie auf **Neue Rolle**.

   ![](assets/three-1.png)

1. Geben Sie einen Rollennamen ein und wählen Sie &quot;Berechtigungen&quot;. Klicken Sie auf **Create** (Diese Rolle muss [auf alle Arbeitsbereiche](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md) angewendet werden.)

   ![](assets/four.png)

   >[!TIP]
   >
   >Um Benutzern Zugriff auf alle Elemente in Targeting und Personalisierung zu gewähren, müssen Sie die Kontrollkästchen _alle_ aktivieren.

## Web-Personalisierung und Predictive Content Benutzerberechtigungen {#web-personalization-and-predictive-content-user-permissions}

**Targeting und Personalisierung**: Der Benutzer hat nur Berechtigungen für Ansichten, wenn diese Berechtigung nur aktiviert ist.

**Admin Web Personalization + Predictive**: Benutzer hat nur Zugriff auf die Kontoeinstellungen und Inhaltseinstellungen für die App &quot;Web-Personalisierung&quot;und &quot;Predictive Content&quot;. Die Benutzer können Ansichten in der App erstellen, bearbeiten, löschen oder starten.

**Predictive Content Editor**: Benutzer hat Zugriff auf die Predictive Content-App. Die Berechtigung ermöglicht das Erstellen, Bearbeiten und Löschen von Inhaltselementen. Es ist nicht möglich, Inhalte für eine prädiktive Verwendung im Web oder in E-Mail zu aktivieren.

**Predictive Content Launcher**: Der Benutzer hat Zugriff auf alle Funktionen von Predictive Content, mit Ausnahme der Konto- und Inhaltseinstellungen. Mit dieser Berechtigung können Sie Inhaltselemente erstellen, bearbeiten, löschen und aktivieren.

**Web-Kampagne-Editor**: Der Benutzer hat Editor Zugriff auf alle Web-Personalisierungsfunktionen, um Web-Kampagnen zu erstellen, zu bearbeiten und zu löschen, jedoch nicht zu starten.

**Web Kampagne Launcher**: Benutzer hat Zugriff auf alle Funktionen der Web-Personalisierung-App, mit Ausnahme der Konto- und Inhaltseinstellungen. Mit dieser Berechtigung können Sie Web-Kampagnen erstellen, bearbeiten, löschen und starten.

## WP-Rolle Benutzer {#assign-wp-role-to-user} zuweisen

1. Gehen Sie zu **Benutzer**.

   ![](assets/image2015-4-29-11-3a31-3a3.png)

1. Wählen Sie den Benutzer aus, dem WP Zugriff gewährt werden soll, und klicken Sie auf **Benutzer bearbeiten**.

   ![](assets/image2015-4-29-11-3a38-3a46.png)

1. Wählen Sie die WP-Benutzerrolle für alle Arbeitsbereiche aus.

   ![](assets/seven.png)

1. Bei der nächsten Anmeldung sehen Benutzer, die neu aktiviert sind, die Kachel **Webpersonalisierung** in &quot;Mein Markt&quot;.

   ![](assets/eight.png)
