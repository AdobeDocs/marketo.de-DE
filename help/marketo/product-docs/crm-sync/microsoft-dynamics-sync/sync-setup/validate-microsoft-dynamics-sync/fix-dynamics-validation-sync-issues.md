---
unique-page-id: 10095429
description: Probleme bei der Synchronisierung der Dynamikvalidierung - Marketing-Dokumente - Produktdokumentation
title: Probleme mit der Synchronisierung der Dynamikvalidierung beheben
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

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

## Benutzername und Kennwort sind gültig {#username-and-password-are-valid}

Wenn Sie hier ein ![—](assets/delete.png) haben, überprüfen Sie, ob Ihr Microsoft Dynamics-Benutzername und -Kennwort gültig sind.

## Synchronisierungsbenutzer werden der Rolle &quot;Marketo-Synchronisierungsbenutzer&quot; {#sync-user-is-assigned-to-the-marketo-sync-user-role} zugewiesen

Wenn Sie hier ein ![—](assets/delete.png) haben, müssen Sie überprüfen, ob die Rolle &quot;Marketo-Synchronisierungsbenutzer&quot;in Microsoft Dynamics aktiviert ist. Siehe Schritt 2 der Installationsdokumentation von MIcrosoft Dynamics.

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

1. Überprüfen Sie, ob die Rolle &quot;Benutzer synchronisieren&quot;aktiviert ist. Wenn nicht, markieren Sie es und klicken Sie auf **OK.**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

## Die Marketo-Lösung ist korrekt installiert.{#marketo-solution-is-properly-installed}

Wenn Sie ![—](assets/delete.png) hier haben, gehen Sie zu Microsoft Dynamics, um zu überprüfen, ob die Installation von Marketo vorhanden ist. Siehe Schritt 1 der Setup-Dokumentation zu MIcrosoft Dynamics.

1. Klicken Sie unter &quot;Dynamik&quot;auf das Symbol &quot;Einstellungen&quot;und wählen Sie **Erweiterte Einstellungen**.

   ![](assets/one.png)

1. Klicken Sie auf **Einstellungen **und wählen Sie **Lösungen.**

   ![](assets/eleven.png)

1. Überprüfen Sie, ob die Lösung aufgelistet ist.

   ![](assets/twelve.png)

## Alle Schritte in der Lösung sind aktiviert {#all-steps-in-the-solution-are-enabled}

Wenn Sie hier ein ![—](assets/delete.png) haben, stellen Sie sicher, dass keiner der Standardschritte deaktiviert wurde. Alle Schritte werden bei der Installation automatisch aktiviert, können jedoch während der Anpassung deaktiviert werden.

## Synchronisierungsbenutzer werden der Marketing-Lösung {#sync-user-is-assigned-to-the-marketo-solution} zugewiesen

Wenn Sie hier ein ![—](assets/delete.png) haben, vergewissern Sie sich, dass der Synchronisierungsbenutzer auf der Seite &quot;Standard marketo&quot;in Microsoft Dynamics zugewiesen ist.

1. Klicken Sie unter &quot;Dynamik&quot;auf das Symbol &quot;Einstellungen&quot;und wählen Sie **Erweiterte Einstellungen**.

   ![](assets/one.png)

1. Klicken Sie auf **Einstellungen **und wählen Sie **Marketing-Konfiguration**.

   ![](assets/thirteen.png)

1. Vergewissern Sie sich, dass der Synchronisierungsbenutzer als Standard zugewiesen ist.

   ![](assets/fourteen.png)

## Synchronisierungsbenutzer mit Benutzername und Kennwort {#sync-user-matches-username-and-password}

Wenn Sie hier ein ![—](assets/delete.png) haben, stellen Sie sicher, dass Sie den richtigen Synchronisierungsbenutzer im Feld &quot;Marketo-Benutzer&quot;im Setup-Schritt &quot;Standard für Marketo-Konfiguration&quot;in Microsoft Dynamics zuweisen.

>[!MORELIKETHIS]
>
>[Microsoft Dynamics Sync überprüfen](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)

