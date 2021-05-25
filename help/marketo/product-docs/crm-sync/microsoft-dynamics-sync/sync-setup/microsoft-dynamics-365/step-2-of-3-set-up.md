---
unique-page-id: 3571827
description: 'Schritt 2 von 3: Einrichten eines Marketo Sync User in Dynamics - Marketo Docs - Produktdokumentation'
title: 'Schritt 2 von 3: Einrichten des Marketo Sync User in Dynamics'
exl-id: 324e2142-2aa2-4548-9a04-683832e3ba69
source-git-commit: 5473e1a78769ba23e9c3a5926407cf42ef9685a0
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Schritt 2 von 3: Marketo Sync User in Dynamics {#step-of-set-up-marketo-sync-user-in-dynamics} einrichten

Beginnen wir mit der Erstellung eines Benutzerkontos.

>[!PREREQUISITES]
[Schritt 1 von 3: Installieren der Marketo-Lösung (Online)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md)>
>

## Neuen Benutzer {#create-a-new-user} erstellen

1. Melden Sie sich bei Dynamics an. Klicken Sie auf das Symbol Einstellungen und wählen Sie **Erweiterte Einstellungen** aus.

   ![](assets/one.png)

1. Klicken Sie auf **Einstellungen** und wählen Sie **Sicherheit** aus.

   ![](assets/two.png)

1. Klicken Sie auf **Benutzer**.

   ![](assets/three.png)

1. Klicken Sie auf **Neu.**

   ![](assets/four.png)

1. Klicken Sie im neuen Fenster auf **Benutzer hinzufügen und lizenzieren** .

   ![](assets/five.png)

1. Eine neue Registerkarte wird geöffnet. Klicken Sie oben auf der Seite auf **Admin** .

   ![](assets/six.png)

1. Eine weitere neue Registerkarte wird geöffnet. Klicken Sie auf **Benutzer hinzufügen**.

   ![](assets/seven.png)

1. Geben Sie alle Ihre Informationen ein. Wenn Sie fertig sind, klicken Sie auf **Hinzufügen**.

   ![](assets/eight.png)

   >[!NOTE]
   Dieser Name muss ein dedizierter Synchronisierungsbenutzer und nicht das Konto eines vorhandenen CRM-Benutzers sein. Es muss sich nicht um eine tatsächliche E-Mail-Adresse handeln.

1. Geben Sie die E-Mail ein, um die neuen Benutzeranmeldeinformationen zu erhalten, und klicken Sie auf **E-Mail senden und schließen**.

   ![](assets/nine.png)

## Benutzerrolle &quot;Sync zuweisen&quot;{#assign-sync-user-role}

Weisen Sie die Benutzerrolle &quot;Marketo Sync User&quot;nur dem Marketo-Synchronisierungsbenutzer zu. Sie müssen sie keinen anderen Benutzern zuweisen.

>[!NOTE]
Dies gilt für die Marketo-Version 4.0.0.14 und höher. Bei früheren Versionen müssen alle Benutzer über die Benutzerrolle &quot;Synchronisieren&quot;verfügen. Informationen zum Aktualisieren von Marketo finden Sie unter [Upgrade der Marketo-Lösung für Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
Die Spracheinstellung des Synchronisierungsbenutzers [sollte auf &quot;English](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us)&quot;gesetzt werden.

1. Gehen Sie zurück zur Registerkarte Aktivierte Benutzer und aktualisieren Sie die Benutzerliste.

   ![](assets/ten.png)

1. Bewegen Sie den Mauszeiger neben dem neu erstellten Marketo Sync-Benutzer und ein Kontrollkästchen wird angezeigt. Klicken Sie auf , um es auszuwählen.

   ![](assets/eleven.png)

1. Klicken Sie auf **Rollen verwalten**.

   ![](assets/twelve.png)

1. Markieren Sie **Marketo Sync User** und klicken Sie auf **OK**.

   ![](assets/thirteen.png)

   >[!NOTE]
   Alle vom Synchronisierungsbenutzer in Ihrem CRM-System vorgenommenen Aktualisierungen werden **nicht** wieder mit Marketo synchronisiert.

## Konfigurieren der Marketo-Lösung {#configure-marketo-solution}

Fast da! Wir haben nur noch die Möglichkeit, Marketo Solution über den neu erstellten Benutzer zu informieren.

1. Gehen Sie zurück zum Abschnitt Erweiterte Einstellungen , klicken Sie auf das Symbol ![](assets/image2015-5-13-15-3a49-3a19.png) neben Einstellungen und wählen Sie **Marketo Config** aus.

   ![](assets/fourteen.png)

   >[!NOTE]
   Wenn **Marketo Config** nicht im Menü &quot;Einstellungen&quot;angezeigt wird, aktualisieren Sie die Seite. Wenn dies nicht funktioniert, versuchen Sie [Marketo Solution](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md) erneut zu veröffentlichen oder melden Sie sich ab und wieder an.

1. Klicken Sie auf **Default**.

   ![](assets/fifteen.png)

1. Klicken Sie auf die Suchschaltfläche im Feld **Marketo User** und wählen Sie den erstellten Synchronisierungsbenutzer aus.

   ![](assets/sixteen.png)

1. Klicken Sie unten rechts auf das Symbol ![](assets/image2015-3-13-15-3a10-3a11.png) , um die Änderungen zu speichern.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Klicken Sie oben rechts auf **X**, um den Bildschirm zu schließen.

   ![](assets/seventeen.png)

1. Klicken Sie auf das Symbol ![](assets/image2015-5-13-15-3a49-3a19-1.png) neben Einstellungen und wählen Sie **Lösungen** aus.

   ![](assets/eighteen.png)

1. Klicken Sie auf die Schaltfläche **Alle Anpassungen veröffentlichen** .

   ![](assets/nineteen.png)

## Bevor Sie mit Schritt 3 fortfahren {#before-proceeding-to-step}

    * Wenn Sie die Anzahl der synchronisierten Datensätze beschränken möchten, [richten Sie jetzt einen benutzerdefinierten Synchronisierungsfilter ein](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md).
    * Führen Sie den Prozess [Microsoft Dynamics Sync überprüfen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) aus. Es wird überprüft, ob Ihre ersten Setups ordnungsgemäß durchgeführt wurden.
    * Melden Sie sich beim Marketo Sync User in Microsoft Dynamics CRM an.

>[!MORELIKETHIS]
[Schritt 3 von 3: Verbinden von Microsoft Dynamics mit Marketo (Online)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md)
