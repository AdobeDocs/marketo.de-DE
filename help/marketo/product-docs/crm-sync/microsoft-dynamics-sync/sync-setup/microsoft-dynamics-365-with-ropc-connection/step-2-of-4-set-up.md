---
description: 'Schritt 2 von 4: Einrichten der Marketo-Lösung mit Resource Owner Password Control Connection - Marketo Docs - Produktdokumentation'
title: 'Schritt 2 von 4: Einrichten der Marketo-Lösung mit Resource Owner Password Control Connection'
exl-id: 41c05910-d8e3-4fb7-8f68-17ee10294e57
feature: Microsoft Dynamics
source-git-commit: 2eb61d43f2f470d42e1b50ab8edc99e4e25c23cf
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 0%

---

# Schritt 2 von 4: Einrichten der Marketo-Lösung mit Resource Owner Password Control Connection {#step-2-of-4-set-up-the-marketo-solution-ropc}

Beginnen wir mit der Erstellung eines Benutzerkontos.

>[!PREREQUISITES]
>
>[Schritt 1 von 4: Installieren der Marketo-Lösung mit Resource Owner Password Control Connection](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"}

## Neuen Benutzer erstellen {#create-a-new-user}

1. Melden Sie sich bei Dynamics an. Klicken Sie auf das Symbol Einstellungen und wählen Sie **[!UICONTROL Erweiterte Einstellungen]**.

   ![](assets/one.png)

1. Klicks **[!UICONTROL Einstellungen]** und wählen **[!UICONTROL Sicherheit]**.

   ![](assets/two.png)

1. Klicks **[!UICONTROL Benutzer]**.

   ![](assets/three.png)

1. Klicks **[!UICONTROL Neu]**.

   ![](assets/four.png)

1. Klicks **[!UICONTROL Hinzufügen und Lizenzieren von Benutzern]** im neuen Fenster.

   ![](assets/five.png)

1. Eine neue Registerkarte wird geöffnet. Klicks **[!UICONTROL Admin]** oben auf der Seite.

   ![](assets/six.png)

1. Eine weitere neue Registerkarte wird geöffnet. Klicks **[!UICONTROL Benutzer hinzufügen]**.

   ![](assets/seven.png)

   >[!IMPORTANT]
   >
   >Der Synchronisierungsbenutzer sollte über Leseberechtigungen für die Marketo-Konfiguration verfügen.

1. Geben Sie alle Ihre Informationen ein. Wenn Sie fertig sind, klicken Sie auf **[!UICONTROL Hinzufügen]**.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Dieser Name muss ein dedizierter Synchronisierungsbenutzer und nicht das Konto eines vorhandenen CRM-Benutzers sein. Es muss sich nicht um eine tatsächliche E-Mail-Adresse handeln.

1. Geben Sie die E-Mail zum Empfang der neuen Benutzeranmeldeinformationen ein und klicken Sie auf **[!UICONTROL E-Mail senden und schließen]**.

   ![](assets/nine.png)

## Benutzerrolle &quot;Synchronisierung zuweisen&quot; {#assign-sync-user-role}

Weisen Sie die Benutzerrolle &quot;Marketo Sync User&quot;nur dem Marketo-Synchronisierungsbenutzer zu. Sie müssen sie keinen anderen Benutzern zuweisen.

>[!NOTE]
>
>Dies gilt für die Marketo-Version 4.0.0.14 und höher. Bei früheren Versionen müssen alle Benutzer über die Benutzerrolle &quot;Synchronisieren&quot;verfügen. Informationen zum Aktualisieren von Marketo finden Sie unter [Upgrade der Marketo-Lösung für Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md){target="_blank"}.

>[!IMPORTANT]
>
>Die Spracheinstellung des Synchronisierungsbenutzers [sollte auf Englisch eingestellt sein](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us){target="_blank"}.

1. Gehen Sie zurück zu **[!UICONTROL Aktivierte Benutzer]** und aktualisieren Sie die Benutzerliste.

   ![](assets/ten.png)

1. Bewegen Sie den Mauszeiger neben dem neu erstellten Marketo Sync-Benutzer und ein Kontrollkästchen wird angezeigt. Klicken Sie auf , um es auszuwählen.

   ![](assets/eleven.png)

1. Klicks **[!UICONTROL Rollen verwalten]**.

   ![](assets/twelve.png)

1. Überprüfen **[!UICONTROL Marketo Sync User]** und klicken **[!UICONTROL OK]**.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Alle vom Synchronisierungsbenutzer in Ihrem CRM-System vorgenommenen Aktualisierungen werden _not_ wieder mit Marketo synchronisiert werden.

## Konfigurieren der Marketo-Lösung {#configure-marketo-solution}

Fast da! Wir haben nur noch die Möglichkeit, Marketo Solution über den neu erstellten Benutzer zu informieren.

1. Gehen Sie zurück zum Abschnitt Erweiterte Einstellungen und klicken Sie auf die Schaltfläche ![](assets/image2015-5-13-15-3a49-3a19.png) Symbol neben Einstellungen und wählen Sie **[!UICONTROL Marketo-Konfiguration]**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Wenn Sie nicht sehen **[!UICONTROL Marketo-Konfiguration]** Aktualisieren Sie die Seite im Menü Einstellungen . Wenn das nicht funktioniert, versuchen Sie, [Marketo-Lösung veröffentlichen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"} erneut oder melden Sie sich ab und wieder an.

1. Klicks **[!UICONTROL Standard]**.

   ![](assets/fifteen.png)

1. Klicken Sie auf die Suchschaltfläche **[!UICONTROL Marketo-Benutzer]** und wählen Sie den erstellten Synchronisierungsbenutzer aus.

   ![](assets/sixteen.png)

1. Klicken Sie auf ![](assets/image2015-3-13-15-3a10-3a11.png) in der rechten unteren Ecke, um die Änderungen zu speichern.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Klicken Sie auf **X** oben rechts, um den Bildschirm zu schließen.

   ![](assets/seventeen.png)

1. Klicken Sie auf ![](assets/image2015-5-13-15-3a49-3a19-1.png) Symbol neben Einstellungen und wählen Sie **[!UICONTROL Lösungen]**.

   ![](assets/eighteen.png)

1. Klicken Sie auf **[!UICONTROL Alle Anpassungen veröffentlichen]** Schaltfläche.

   ![](assets/nineteen.png)

>[!MORELIKETHIS]
>
>[Schritt 3 von 4: Verbinden der Marketo-Lösung mit der Resource Owner Password Control Connection](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md){target="_blank"}
