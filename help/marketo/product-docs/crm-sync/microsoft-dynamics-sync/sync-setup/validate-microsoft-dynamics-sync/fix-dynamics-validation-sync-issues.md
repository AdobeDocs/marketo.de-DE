---
unique-page-id: 10095429
description: Probleme mit der Synchronisierung der Dynamikvalidierung - Marketo Dokumente - Produktdokumentation
title: Probleme mit der Synchronisierung der Dynamikvalidierung beheben
exl-id: 1a300249-65b7-49b1-bf50-82236916298f
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 8%

---

# Probleme bei der Synchronisierung der Dynamikvalidierung {#fix-dynamics-validation-sync-issues} beheben

## Validieren der Ergebnisse des Synchronisierungstools {#validate-sync-tool-results}

Wenn Sie die Synchronisierung zum Überprüfen der Dynamik ausführen, wird dieser Bericht generiert. Wenn neben einem Schritt ein ![delete](assets/delete.png) vorhanden ist, sehen Sie unten, um das Problem zu identifizieren und zu beheben. Führen Sie dann die Synchronisierungsüberprüfungsschritte erneut aus, bis das Ergebnis nur die Häkchen anzeigt.

![](assets/image2015-9-22-15-3a58-3a12.png)

## URL ist gültig {#url-is-valid}

Wenn Sie ![delete](assets/delete.png) hier verwenden, überprüfen Sie, ob die URL gültig ist. Suchen Sie es hier in Developer Resources und schauen Sie sich den Organisationsdienst an. Die URL kann aus verschiedenen Gründen ungültig sein.

1. Melden Sie sich bei Dynamics an. Klicken Sie auf das Symbol Einstellungen und wählen Sie **Erweiterte Einstellungen**.

   ![](assets/one.png)

1. Klicken Sie auf Einstellungen und wählen Sie **Anpassungen**.

   ![](assets/two.png)

1. Klicken Sie auf **Entwicklerressourcen**.

   ![](assets/three.png)

1. Die Organisationsdienst-URL befindet sich unter Dienstendpunkte.

   ![](assets/four.png)

## Benutzername und Passwort sind gültig {#username-and-password-are-valid}

Wenn Sie hier ein ![—](assets/delete.png) haben, überprüfen Sie, ob Ihr Microsoft Dynamics-Benutzername und -Kennwort gültig sind.

## Synchronisierungsbenutzer werden der Marketo Sync User-Rolle {#sync-user-is-assigned-to-the-marketo-sync-user-role} zugewiesen.

Wenn Sie hier ein ![—](assets/delete.png) haben, müssen Sie überprüfen, ob die Rolle &quot;Marketo Sync User&quot;in Microsoft Dynamics aktiviert ist. Siehe Schritt 2 der Installationsdokumentation von MIcrosoft Dynamics.

1. Klicken Sie unter &quot;Dynamik&quot;auf das Symbol &quot;Einstellungen&quot;und wählen Sie **Erweiterte Einstellungen**.

   ![](assets/one.png)

1. Klicken Sie auf **Einstellungen** und wählen Sie **Sicherheit**.

   ![](assets/six.png)

1. Klicken Sie auf **Benutzer.**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. Klicken Sie auf den Link für den Synchronisierungsbenutzer.

   ![](assets/seven.png)

1. Klicken Sie auf **Rollen verwalten**.

   ![](assets/eight.png)

1. Überprüfen Sie, ob die Rolle &quot;Marketo Sync User&quot;aktiviert ist. Wenn nicht, markieren Sie es und klicken Sie auf **OK.**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

## Lösung von Marketo ist ordnungsgemäß installiert {#marketo-solution-is-properly-installed}

Wenn Sie ![—](assets/delete.png) hier haben, gehen Sie zu Microsoft Dynamics, um zu überprüfen, ob die Marketo-Installation vorhanden ist. Siehe Schritt 1 der Setup-Dokumentation zu MIcrosoft Dynamics.

1. Klicken Sie unter &quot;Dynamik&quot;auf das Symbol &quot;Einstellungen&quot;und wählen Sie **Erweiterte Einstellungen**.

   ![](assets/one.png)

1. Klicken Sie auf **Einstellungen** und wählen Sie **Lösungen.**

   ![](assets/eleven.png)

1. Überprüfen Sie, ob die Lösung aufgelistet ist.

   ![](assets/twelve.png)

## Alle Schritte in der Lösung sind aktiviert {#all-steps-in-the-solution-are-enabled}

Wenn Sie hier ein ![—](assets/delete.png) haben, stellen Sie sicher, dass keiner der Standardschritte deaktiviert wurde. Alle Schritte werden bei der Installation automatisch aktiviert, können jedoch während der Anpassung deaktiviert werden.

## Synchronisierter Benutzer ist der Lösung von Marketo zugeordnet {#sync-user-is-assigned-to-the-marketo-solution}

Wenn Sie hier ein ![—](assets/delete.png) haben, stellen Sie sicher, dass der Synchronisierungsbenutzer auf der Seite &quot;Marketo-Standard&quot;in Microsoft Dynamics zugewiesen ist.

1. Klicken Sie unter &quot;Dynamik&quot;auf das Symbol &quot;Einstellungen&quot;und wählen Sie **Erweiterte Einstellungen**.

   ![](assets/one.png)

1. Klicken Sie auf **Einstellungen** und wählen Sie **Marketo Config**.

   ![](assets/thirteen.png)

1. Vergewissern Sie sich, dass der Synchronisierungsbenutzer als Standard zugewiesen ist.

   ![](assets/fourteen.png)

## Synchronisierter Benutzer stimmt mit Benutzernamen und Passwort überein {#sync-user-matches-username-and-password}

Wenn Sie hier ein ![—](assets/delete.png) haben, stellen Sie sicher, dass Sie den richtigen Synchronisierungsbenutzer im Feld &quot;Marketo-Benutzer&quot;im Schritt Marketo Config Default Setup unter Microsoft Dynamics zuweisen.

>[!MORELIKETHIS]
>
>[Microsoft Dynamics Sync überprüfen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)
