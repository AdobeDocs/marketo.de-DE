---
unique-page-id: 10095429
description: Beheben von Synchronisierungsproblemen mit der Dynamics-Validierung - Marketo-Dokumente - Produktdokumentation
title: Beheben von Synchronisierungsproblemen mit der Dynamics-Validierung
exl-id: 1a300249-65b7-49b1-bf50-82236916298f
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 6%

---

# Beheben von Synchronisierungsproblemen mit der Dynamics-Validierung {#fix-dynamics-validation-sync-issues}

## Ergebnisse des Synchronisierungs-Tools validieren {#validate-sync-tool-results}

Wenn Sie die Dynamics-Validierungs-Synchronisierung ausführen, wird ein Bericht generiert. Wenn neben einem Schritt ein ![x](assets/delete.png) angezeigt wird, sehen Sie sich die folgenden Optionen an, um das Problem zu identifizieren und zu beheben. Führen Sie dann die Synchronisierungsvalidierungsschritte erneut aus, bis das Ergebnis nur noch grüne Häkchen anzeigt.

![](assets/image2015-9-22-15-3a58-3a12.png)

## URL ist gültig {#url-is-valid}

Wenn Sie hier ein ![x](assets/delete.png) haben, überprüfen Sie, ob die URL gültig ist. Finden Sie sie hier in Entwicklerressourcen und sehen Sie sich den Organisations-Service an. Die URL könnte aus verschiedenen Gründen ungültig sein.

1. Melden Sie sich bei Dynamics an. Klicken Sie auf das Symbol Einstellungen und wählen Sie **Erweiterte Einstellungen** aus.

   ![](assets/one.png)

1. Klicken Sie auf Einstellungen und wählen Sie **Anpassungen** aus.

   ![](assets/two.png)

1. Klicken Sie auf **Entwicklungsressourcen**.

   ![](assets/three.png)

1. Die Organisations-Service-URL finden Sie unter Service-Endpunkte .

   ![](assets/four.png)

## Benutzername und Passwort sind gültig {#username-and-password-are-valid}

Wenn Sie hier ein ![x](assets/delete.png) haben, überprüfen Sie, ob Ihre Microsoft Dynamics-Anmeldeinformationen gültig sind. Für die S2S-Authentifizierung der Web-API muss der Benutzername in Marketo mit der [E-Mail](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user)Adresse) des Anwendungsbenutzers im CRM übereinstimmen. Bei anderen Typen sollte er mit dem Benutzernamen für die Benutzersynchronisierung übereinstimmen.

## Synchronisierungsbenutzer ist der Rolle Marketo-Synchronisierungsbenutzer zugewiesen {#sync-user-is-assigned-to-the-marketo-sync-user-role}

Wenn Sie hier ein ![x](assets/delete.png) haben, könnte dies eines der drei folgenden Probleme sein.

**Option 1: Überprüfen Sie, ob die Marketo-Benutzerrolle „Synchronisieren“ in Microsoft Dynamics aktiviert ist**:

1. Klicken Sie in Dynamics auf das Symbol Einstellungen und wählen Sie **Erweiterte Einstellungen** aus.

   ![](assets/one.png)

1. Klicken Sie **Einstellungen** und wählen Sie **Sicherheit** aus.

   ![](assets/six.png)

1. Klicken Sie auf **Benutzer.**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. Klicken Sie auf den Link für den Synchronisierungsbenutzer.

   ![](assets/seven.png)

1. Klicken Sie **Rollen verwalten**.

   ![](assets/eight.png)

1. Überprüfen Sie, ob die Rolle Marketo-Synchronisierungsbenutzer aktiviert ist. Falls nicht, überprüfen Sie sie und klicken Sie auf **OK.**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

**Option 2: Bestätigen der**:

1. Überprüfen Sie die [Einverständnis für Client-ID und App-Registrierung erteilen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md) um zu bestätigen, dass die App über das Einverständnis des Administrators zum Aufrufen von APIs verfügt.

**Option 3: Benutzer synchronisieren**:

1. Stellen Sie sicher, dass „Benutzer synchronisieren“ zur Marketo-Konfiguration hinzugefügt wird.

## Lösung von Marketo ist ordnungsgemäß installiert {#marketo-solution-is-properly-installed}

Wenn Sie hier ein ![x](assets/delete.png) haben, gehen Sie zu Microsoft Dynamics, um zu überprüfen, ob die Marketo-Installation vorhanden ist. Siehe Schritt 1 der Microsoft Dynamics-Einrichtungsdokumentation.

1. Klicken Sie in Dynamics auf das Symbol Einstellungen und wählen Sie **Erweiterte Einstellungen** aus.

   ![](assets/one.png)

1. Klicken Sie auf **Einstellungen** und wählen Sie **Lösungen.**

   ![](assets/eleven.png)

1. Überprüfen Sie, ob die Lösung aufgeführt ist.

   ![](assets/twelve.png)

## Alle Schritte in der Lösung sind aktiviert {#all-steps-in-the-solution-are-enabled}

Wenn Sie hier ein ![x](assets/delete.png) haben, stellen Sie sicher, dass keiner der Standardschritte deaktiviert wurde. Alle Schritte werden bei der Installation automatisch aktiviert, können jedoch bei einer Anpassung deaktiviert werden.

## Synchronisierter Benutzer ist der Lösung von Marketo zugeordnet {#sync-user-is-assigned-to-the-marketo-solution}

Wenn Sie hier ein ![x](assets/delete.png) haben, stellen Sie sicher, dass der Benutzer „Synchronisieren“ auf der Marketo-Standardseite in Microsoft Dynamics zugewiesen ist.

1. Klicken Sie in Dynamics auf das Symbol Einstellungen und wählen Sie **Erweiterte Einstellungen** aus.

   ![](assets/one.png)

1. Klicken Sie **Einstellungen** und wählen Sie **Marketo Config** aus.

   ![](assets/thirteen.png)

1. Stellen Sie sicher, dass der Synchronisierungsbenutzer als Standard zugewiesen ist.

   ![](assets/fourteen.png)

## Synchronisierter Benutzer stimmt mit Benutzernamen und Passwort überein {#sync-user-matches-username-and-password}

Wenn Sie hier ein ![x](assets/delete.png) haben, stellen Sie sicher, dass Sie den richtigen Synchronisierungsbenutzer im Feld Marketo-Benutzer im Schritt Standardeinrichtung der Marketo-Konfiguration in Microsoft Dynamics zuweisen.

>[!MORELIKETHIS]
>
>[Validieren der Microsoft Dynamics-Synchronisierung](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)
