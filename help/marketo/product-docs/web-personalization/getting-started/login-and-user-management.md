---
unique-page-id: 7513771
description: Anmeldung und Benutzerverwaltung - Marketo-Dokumente - Produktdokumentation
title: Anmeldung und Benutzerverwaltung
exl-id: 3cf5a50a-1926-4fb6-a1fe-39ba5eb2560f
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 2%

---

# Anmeldung und Benutzerverwaltung {#login-and-user-management}

## Erstellen einer [!UICONTROL Web Personalization]-Benutzerrolle {#create-a-web-personalization-user-role}

1. Gehen Sie zum Abschnitt **[!UICONTROL Admin]** und klicken Sie dann auf **[!UICONTROL Benutzer und Rollen]**.

   ![](assets/image2015-4-28-19-3a50-3a49.png)

1. Klicken Sie auf **[!UICONTROL Rollen]**.

   ![](assets/image2015-4-28-19-3a57-3a58.png)

   >[!NOTE]
   >
   >Wenn die Benutzerrolle Web Personalization (WP) bereits vorhanden ist, stellen Sie sicher, dass sie wie in Schritt 4 konfiguriert ist.

1. Klicken Sie auf **[!UICONTROL Neue Rolle]**.

   ![](assets/three-1.png)

1. Geben Sie einen [!UICONTROL Rollennamen] ein und wählen Sie [!UICONTROL Berechtigungen] aus. Klicken Sie **[!UICONTROL Erstellen]** (diese Rolle muss [für alle Arbeitsbereiche gelten](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md)).

   ![](assets/four.png)

   >[!TIP]
   >
   >Um Benutzerinnen und Benutzern die Berechtigung zum Zugriff auf alle Elemente in Targeting und Personalization zu erteilen, aktivieren Sie _alle_ Kontrollkästchen.

## [!UICONTROL Web-Personalization] und Benutzerberechtigungen für prädiktive Inhalte {#web-personalization-and-predictive-content-user-permissions}

**[!UICONTROL Targeting und Personalization]**: Der Benutzer hat nur Leseberechtigungen, wenn diese Berechtigung nur ausgewählt ist.

**[!UICONTROL Admin Web Personalization + Predictive]**: Der Benutzer hat nur Zugriff auf die Kontoeinstellungen und Inhaltseinstellungen für die Web Personalization und die Predictive Content-App. Benutzer können Seiten in der App anzeigen, haben jedoch keine Berechtigungen zum Erstellen, Bearbeiten, Löschen oder Starten.

**[!UICONTROL Predictive Content Editor]**: Der Benutzer hat Editor-Zugriff auf die Predictive Content-App. Mit der Berechtigung können Sie Inhaltselemente erstellen, bearbeiten und löschen. Es ist nicht zulässig, Inhalte für die prädiktive Verwendung im Web oder in E-Mails zu aktivieren.

**[!UICONTROL Predictive Content Launcher]**: Der Benutzer hat Zugriff auf alle Funktionen für prädiktive Inhalte mit Ausnahme der Konto- und Inhaltseinstellungen. Mit der Berechtigung können Sie Inhaltselemente erstellen, bearbeiten und löschen sowie aktivieren.

**[!UICONTROL Web-Kampagnen-]**: Der Benutzer hat Editor-Zugriff auf alle Web-Personalization-Funktionen zum Erstellen, Bearbeiten und Löschen, aber nicht zum Starten von Web-Kampagnen.

**[!UICONTROL Web-Kampagnen-Starter]**: Der Benutzer hat Zugriff auf alle Funktionen der Web-Personalization-App, mit Ausnahme der Konto- und Inhaltseinstellungen. Mit der Berechtigung können Sie Web-Kampagnen erstellen, bearbeiten, löschen und starten.

## WP-Rolle dem Benutzer zuweisen {#assign-wp-role-to-user}

1. Navigieren Sie zu **[!UICONTROL Benutzer]**.

   ![](assets/image2015-4-29-11-3a31-3a3.png)

1. Wählen Sie den Benutzer aus, dem WP Zugriff gewähren soll, und klicken Sie auf **[!UICONTROL Benutzer bearbeiten]**.

   ![](assets/image2015-4-29-11-3a38-3a46.png)

1. Wählen Sie die Rolle WP-Benutzer für alle Arbeitsbereiche aus.

   ![](assets/seven.png)

1. Neu aktivierte Benutzer sehen die Kachel **[!UICONTROL Web-Personalization]** in Mein Marketo, wenn sie sich das nächste Mal anmelden.

   ![](assets/eight.png)
