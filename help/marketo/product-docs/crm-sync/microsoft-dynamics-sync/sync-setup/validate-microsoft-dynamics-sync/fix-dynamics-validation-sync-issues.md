---
unique-page-id: 10095429
description: Beheben von Synchronisierungsproblemen bei der Dynamics-Überprüfung - Marketo-Dokumente - Produktdokumentation
title: Synchronisierungsprobleme bei der Dynamics-Überprüfung beheben
exl-id: 1a300249-65b7-49b1-bf50-82236916298f
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 6%

---

# Synchronisierungsprobleme bei der Dynamics-Überprüfung beheben {#fix-dynamics-validation-sync-issues}

## Überprüfen der Ergebnisse des Synchronisierungswerkzeugs {#validate-sync-tool-results}

Wenn Sie die Synchronisierung der Dynamics-Validierung ausführen, wird ein Bericht generiert. Wenn neben einem Schritt ein ![x](assets/delete.png) vorhanden ist, sehen Sie sich die folgenden Optionen an, um das Problem zu identifizieren und zu beheben. Führen Sie dann die Synchronisierungsvalidierungsschritte erneut aus, bis das Ergebnis nur grüne Häkchen anzeigt.

![](assets/image2015-9-22-15-3a58-3a12.png)

## URL ist gültig {#url-is-valid}

Wenn Sie hier ein ![x](assets/delete.png) haben, überprüfen Sie, ob die URL gültig ist. Finden Sie es hier in den Entwicklungsressourcen und sehen Sie sich den Organisationsdienst an. Die URL kann aus verschiedenen Gründen ungültig sein.

1. Melden Sie sich bei Dynamics an. Klicken Sie auf das Symbol Einstellungen und wählen Sie **Erweiterte Einstellungen** aus.

   ![](assets/one.png)

1. Klicken Sie auf Einstellungen und wählen Sie **Anpassungen** aus.

   ![](assets/two.png)

1. Klicken Sie auf **Entwicklungsressourcen**.

   ![](assets/three.png)

1. Die Organisationsdienst-URL finden Sie unter Dienstendpunkte .

   ![](assets/four.png)

## Benutzername und Passwort sind gültig {#username-and-password-are-valid}

Wenn Sie hier über eine ![x](assets/delete.png) verfügen, überprüfen Sie, ob Ihre Microsoft Dynamics-Anmeldeinformationen gültig sind. Für die Web API S2S-Authentifizierung muss der Benutzername in Marketo mit der [E-Mail-Adresse](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user) des Anwendungsbenutzers im CRM übereinstimmen. Bei anderen Typen sollte sie mit dem Benutzernamen für den Synchronisierungsbenutzer übereinstimmen.

## Der Synchronisierungsbenutzer wird der Benutzerrolle &quot;Marketo Sync User&quot;zugewiesen. {#sync-user-is-assigned-to-the-marketo-sync-user-role}

Wenn Sie hier ein ![x](assets/delete.png) haben, könnte es eines der drei folgenden Probleme sein.

**Option 1 - Überprüfen Sie, ob die Benutzerrolle &quot;Marketo Sync User&quot;in Microsoft Dynamics** aktiviert ist:

1. Klicken Sie in Dynamics auf das Symbol Einstellungen und wählen Sie **Erweiterte Einstellungen** aus.

   ![](assets/one.png)

1. Klicken Sie auf **Einstellungen** und wählen Sie **Sicherheit** aus.

   ![](assets/six.png)

1. Klicken Sie auf **Benutzer.**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. Klicken Sie auf den Link für den Synchronisierungsbenutzer.

   ![](assets/seven.png)

1. Klicken Sie auf **Rollen verwalten**.

   ![](assets/eight.png)

1. Stellen Sie sicher, dass die Benutzerrolle &quot;Marketo Sync User&quot;aktiviert ist. Wenn nicht, überprüfen Sie es und klicken Sie auf **OK**.

   ![](assets/image2015-9-24-9-3a59-3a21.png)

**Option 2 - Confirm Grant Consent**:

1. Überprüfen Sie die Option [Zustimmung für Client-ID und App-Registrierung erteilen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md) , um sicherzustellen, dass die App über die Administratorzustimmung zum Aufrufen von APIs verfügt.

**Option Drei - Benutzer synchronisieren**:

1. Stellen Sie sicher, dass der Synchronisierungsbenutzer zur Marketo-Konfiguration hinzugefügt wird.

## Lösung von Marketo ist ordnungsgemäß installiert {#marketo-solution-is-properly-installed}

Wenn Sie hier über eine &quot;![x](assets/delete.png)&quot;verfügen, gehen Sie zu Microsoft Dynamics , um zu überprüfen, ob die Marketo-Installation vorhanden ist. Siehe Schritt 1 der Microsoft Dynamics-Setup-Dokumentation.

1. Klicken Sie in Dynamics auf das Symbol Einstellungen und wählen Sie **Erweiterte Einstellungen** aus.

   ![](assets/one.png)

1. Klicken Sie auf **Einstellungen** und wählen Sie **Lösungen.**

   ![](assets/eleven.png)

1. Überprüfen Sie, ob die Lösung aufgelistet ist.

   ![](assets/twelve.png)

## Alle Schritte in der Lösung sind aktiviert {#all-steps-in-the-solution-are-enabled}

Wenn Sie hier ein ![x](assets/delete.png) haben, überprüfen Sie, ob keiner der Standardschritte deaktiviert wurde. Alle Schritte werden bei der Installation automatisch aktiviert, können aber bei der Anpassung deaktiviert werden.

## Synchronisierter Benutzer ist der Lösung von Marketo zugeordnet {#sync-user-is-assigned-to-the-marketo-solution}

Wenn Sie hier einen ![x](assets/delete.png) haben, stellen Sie sicher, dass der Synchronisierungsbenutzer auf der Marketo-Standardseite in Microsoft Dynamics zugewiesen ist.

1. Klicken Sie in Dynamics auf das Symbol Einstellungen und wählen Sie **Erweiterte Einstellungen** aus.

   ![](assets/one.png)

1. Klicken Sie auf **Einstellungen** und wählen Sie **Marketo-Konfiguration** aus.

   ![](assets/thirteen.png)

1. Vergewissern Sie sich, dass der Synchronisierungsbenutzer als Standard zugewiesen ist.

   ![](assets/fourteen.png)

## Synchronisierter Benutzer stimmt mit Benutzernamen und Passwort überein {#sync-user-matches-username-and-password}

Wenn Sie hier über &quot;![x](assets/delete.png)&quot;verfügen, weisen Sie im Setup-Schritt Marketo-Konfiguration in Microsoft Dynamics im Feld &quot;Marketo-Benutzer&quot;den richtigen Synchronisierungsbenutzer zu.

>[!MORELIKETHIS]
>
>[Überprüfen der Synchronisierung von Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)
