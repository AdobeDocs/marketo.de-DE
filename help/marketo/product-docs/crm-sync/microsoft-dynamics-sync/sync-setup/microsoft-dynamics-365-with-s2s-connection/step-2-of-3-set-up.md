---
unique-page-id: 3571827
description: 'Schritt 2 von 3: Einrichten der Marketo-Lösung mit S2S-Verbindung - Marketo Docs - Produktdokumentation'
title: 'Schritt 2 von 3: Einrichten der Marketo-Lösung mit S2S-Verbindung'
exl-id: 324e2142-2aa2-4548-9a04-683832e3ba69
source-git-commit: 8b4d86f2dd5f19abb56451403cd2638b1a852d79
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---

# Schritt 2 von 3: Einrichten des Marketo Sync User in Dynamics {#step-of-set-up-marketo-sync-user-in-dynamics}

Beginnen wir mit der Erstellung eines Benutzerkontos.

>[!PREREQUISITES]
>
>[Schritt 1 von 3: Installieren der Marketo-Lösung mit S2S-Verbindung](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md)

## Neuen Benutzer erstellen {#create-a-new-user}

1. Melden Sie sich bei Dynamics an. Klicken Sie auf das Symbol Einstellungen und wählen Sie **Erweiterte Einstellungen**.

   ![](assets/one.png)

1. Klicken **Einstellungen** und wählen Sie **Sicherheit**.

   ![](assets/two.png)

1. Klicken **Benutzer**.

   ![](assets/three.png)

1. Klicken **Neu.**

   ![](assets/four.png)

1. Klicken **Hinzufügen und Lizenzieren von Benutzern** in das neue Fenster ein.

   ![](assets/five.png)

1. Eine neue Registerkarte wird geöffnet. Klicken **Admin** oben auf der Seite.

   ![](assets/six.png)

1. Eine weitere neue Registerkarte wird geöffnet. Klicken **Benutzer hinzufügen**.

   ![](assets/seven.png)

1. Geben Sie alle Ihre Informationen ein. Wenn Sie fertig sind, klicken Sie auf **Hinzufügen**.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Dieser Name muss ein dedizierter Synchronisierungsbenutzer und nicht das Konto eines vorhandenen CRM-Benutzers sein. Es muss sich nicht um eine tatsächliche E-Mail-Adresse handeln.

1. Geben Sie die E-Mail ein, um die neuen Benutzeranmeldeinformationen zu erhalten, und klicken Sie auf **E-Mail senden und schließen**.

   ![](assets/nine.png)

## Benutzerrolle &quot;Synchronisierung zuweisen&quot; {#assign-sync-user-role}

Weisen Sie die Benutzerrolle &quot;Marketo Sync User&quot;nur dem Marketo-Synchronisierungsbenutzer zu. Sie müssen sie keinen anderen Benutzern zuweisen.

>[!NOTE]
>
>Dies gilt für die Marketo-Version 4.0.0.14 und höher. Bei früheren Versionen müssen alle Benutzer über die Benutzerrolle &quot;Synchronisieren&quot;verfügen. Informationen zum Aktualisieren von Marketo finden Sie unter [Upgrade der Marketo-Lösung für Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>Die Spracheinstellung des Synchronisierungsbenutzers [sollte auf Englisch eingestellt sein](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. Gehen Sie zurück zur Registerkarte Aktivierte Benutzer und aktualisieren Sie die Benutzerliste.

   ![](assets/ten.png)

1. Bewegen Sie den Mauszeiger neben dem neu erstellten Marketo Sync-Benutzer und ein Kontrollkästchen wird angezeigt. Klicken Sie auf , um es auszuwählen.

   ![](assets/eleven.png)

1. Klicken **Rollen verwalten**.

   ![](assets/twelve.png)

1. Überprüfen **Marketo Sync User** und klicken Sie auf **OK**.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Alle vom Synchronisierungsbenutzer in Ihrem CRM-System vorgenommenen Aktualisierungen werden **not** wieder mit Marketo synchronisiert werden.

## Konfigurieren der Marketo-Lösung {#configure-marketo-solution}

Fast da! Wir haben nur noch die Möglichkeit, Marketo Solution über den neu erstellten Benutzer zu informieren.

1. Gehen Sie zurück zum Abschnitt Erweiterte Einstellungen und klicken Sie auf die Schaltfläche ![](assets/image2015-5-13-15-3a49-3a19.png) Symbol neben Einstellungen und wählen Sie **Marketo-Konfiguration**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Wenn Sie **Marketo-Konfiguration** Aktualisieren Sie die Seite im Menü Einstellungen . Wenn das nicht funktioniert, versuchen Sie, [Marketo-Lösung veröffentlichen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md) erneut oder melden Sie sich ab und wieder an.

1. Klicken **Standard**.

   ![](assets/fifteen.png)

1. Klicken Sie auf die Suchschaltfläche **Marketo-Benutzer** und wählen Sie den erstellten Synchronisierungsbenutzer aus.

   ![](assets/sixteen.png)

1. Klicken Sie auf ![](assets/image2015-3-13-15-3a10-3a11.png) in der rechten unteren Ecke, um die Änderungen zu speichern.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Klicken Sie auf **X** oben rechts, um den Bildschirm zu schließen.

   ![](assets/seventeen.png)

1. Klicken Sie auf ![](assets/image2015-5-13-15-3a49-3a19-1.png) Symbol neben Einstellungen und wählen Sie **Lösungen**.

   ![](assets/eighteen.png)

1. Klicken Sie auf **Alle Anpassungen veröffentlichen** Schaltfläche.

   ![](assets/nineteen.png)

## Bevor Sie mit Schritt 3 fortfahren {#before-proceeding-to-step}

    * Wenn Sie die Anzahl der synchronisierten Datensätze beschränken möchten, [richten Sie jetzt einen benutzerdefinierten Synchronisierungsfilter ein](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md).
    * Führen Sie den Prozess [Microsoft Dynamics Sync überprüfen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) aus. Es wird überprüft, ob Ihre ersten Setups ordnungsgemäß durchgeführt wurden.
    * Melden Sie sich beim Marketo Sync User in Microsoft Dynamics CRM an.

>[!MORELIKETHIS]
>
>[Schritt 3 von 3: Verbinden der Marketo-Lösung mit der S2S-Verbindung](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-3-of-3-connect.md)