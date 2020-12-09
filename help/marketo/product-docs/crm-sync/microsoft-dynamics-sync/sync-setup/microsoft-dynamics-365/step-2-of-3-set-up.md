---
unique-page-id: 3571827
description: Schritt 2 von 3 - Einrichten von Marketo Sync User in Dynamics - Marketing Docs - Produktdokumentation
title: Schritt 2 von 3 - Einrichten von "Marketo Sync User in Dynamics"
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 0%

---


# Schritt 2 von 3: Marketo Sync User in Dynamics einrichten {#step-of-set-up-marketo-sync-user-in-dynamics}

Beginnen wir mit der Erstellung eines Benutzerkontos.

>[!PREREQUISITES]
>
>[Schritt 1 von 3: Installieren der Marketing Solution (Online)](step-1-of-3-install.md)

## Neuen Benutzer erstellen {#create-a-new-user}

1. Melden Sie sich bei Dynamics an. Klicken Sie auf das Symbol Einstellungen und wählen Sie **Erweiterte Einstellungen**.

   ![](assets/one.png)

1. Klicken Sie auf** Einstellungen** und wählen Sie **Sicherheit**.

   ![](assets/two.png)

1. Klicken Sie auf **Benutzer**.

   ![](assets/three.png)

1. Klicken Sie auf **Neu.**

   ![](assets/four.png)

1. Klicken Sie im neuen Fenster auf **Hinzufügen und Lizenzanwender** .

   ![](assets/five.png)

1. Eine neue Registerkarte wird geöffnet. Klicken Sie oben auf der Seite auf **Admin** .

   ![](assets/six.png)

1. Eine weitere neue Registerkarte wird geöffnet. Klicken Sie auf **Hinzufügen Benutzer**.

   ![](assets/seven.png)

1. Geben Sie alle Ihre Informationen ein. Wenn Sie fertig sind, klicken Sie auf **Hinzufügen**.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Dieser Name muss ein dedizierter Synchronisierungsbenutzer sein und nicht ein vorhandenes CRM-Benutzerkonto. Es muss keine tatsächliche E-Mail-Adresse sein.

1. Geben Sie die E-Mail ein, um die Anmeldeinformationen des neuen Benutzers zu erhalten, und klicken Sie auf E-Mail **senden und schließen**.

   ![](assets/nine.png)

## Synchronisierte Benutzerrolle zuweisen {#assign-sync-user-role}

Weisen Sie die Rolle &quot;Benutzer synchronisieren&quot;nur dem Synchronisierungsbenutzer von Marketing zu. Sie müssen sie keinem anderen Benutzer zuweisen.

>[!NOTE]
>
>Dies gilt für Marketo Version 4.0.0.14 und höher. Bei älteren Versionen müssen alle Benutzer die Rolle &quot;Synchronisierungsbenutzer&quot;haben. Informationen zum Aktualisieren von Marketo finden Sie unter [Aktualisieren der Marketing-Lösung für Microsoft Dynamics](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md).

1. Gehen Sie zurück zur Registerkarte &quot;Aktivierte Benutzer&quot;und aktualisieren Sie die Liste &quot;Benutzer&quot;.

   ![](assets/ten.png)

1. Bewegen Sie den Mauszeiger über den neu erstellten Markieren zum Synchronisieren-Benutzer und ein Kontrollkästchen wird angezeigt. Klicken Sie auf , um es auszuwählen.

   ![](assets/eleven.png)

1. Klicken Sie auf Rollen **verwalten**.

   ![](assets/twelve.png)

1. Markieren Sie **zur Synchronisierung des Benutzers** und klicken Sie auf **OK**.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Aktualisierungen, die der Synchronisierungsbenutzer in Ihrem CRM-System vorgenommen hat, werden **nicht** mit Marketo synchronisiert.

## Konfigurieren der Marketing-Lösung {#configure-marketo-solution}

Fast da! Alles, was wir noch haben, ist, Marketo Solution über den neuen Benutzer zu informieren.

1. Gehen Sie zurück zum Abschnitt &quot;Erweiterte Einstellungen&quot;, klicken Sie auf das ![](assets/image2015-5-13-15-3a49-3a19.png)Symbol neben &quot;Einstellungen&quot;und wählen Sie &quot; **Konfiguration** markieren&quot;.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Wenn Sie im Menü &quot;Einstellungen&quot;keine **Marketo-Konfiguration** sehen, aktualisieren Sie die Seite. Wenn dies nicht funktioniert, versuchen Sie, die Marketing Solution [erneut zu](https://docs.marketo.com/pages/viewpage.action?pageId=3571822#publish-customizations) [](https://docs.marketo.com/pages/viewpage.action?pageId=3571822#publish-customizations) veröffentlichen oder melden Sie sich ab und wieder an.

1. Klicken Sie auf **Standard**.

   ![](assets/fifteen.png)

1. Klicken Sie auf die Suchschaltfläche im Feld &quot;Benutzer **markieren** &quot;und wählen Sie den erstellten Synchronisierungsbenutzer aus.

   ![](assets/sixteen.png)

1. Klicken Sie auf das ![](assets/image2015-3-13-15-3a10-3a11.png)Symbol in der unteren rechten Ecke, um die Änderungen zu speichern.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Klicken Sie oben rechts auf das **X** , um den Bildschirm zu schließen.

   ![](assets/seventeen.png)

1. Klicken Sie auf das ![](assets/image2015-5-13-15-3a49-3a19-1.png)Symbol neben Einstellungen und wählen Sie **Lösungen**.

   ![](assets/eighteen.png)

1. Klicken Sie auf die Schaltfläche Alle Anpassungen **veröffentlichen** .

   ![](assets/nineteen.png)

## Bevor Sie zu Schritt 3 fortfahren {#before-proceeding-to-step}

    * Wenn Sie die Anzahl der synchronisierten Datensätze einschränken möchten, [richten Sie jetzt einen benutzerdefinierten Synchronisierungsfilter ein](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md).
    * Führen Sie den Vorgang &quot;[Validate Microsoft Dynamics Sync](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)&quot;aus. Es wird überprüft, ob die ersten Setups ordnungsgemäß durchgeführt wurden.
    * Melden Sie sich beim Marketo Sync User in Microsoft Dynamics CRM an.

>[!NOTE]
>
>**Verwandte Artikel**
>
>
>[Schritt 3 von 3: Verbinden von Microsoft Dynamics mit Marketo (Online)](step-3-of-3-connect.md)
