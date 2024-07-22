---
description: 'Schritt 2 von 4: Einrichten der Marketo-Lösung mit Resource Owner Password Control Connection - Marketo Docs - Produktdokumentation'
title: 'Schritt 2 von 4: Einrichten der Marketo-Lösung mit Resource Owner Password Control Connection'
exl-id: 41c05910-d8e3-4fb7-8f68-17ee10294e57
feature: Microsoft Dynamics
source-git-commit: 2eb61d43f2f470d42e1b50ab8edc99e4e25c23cf
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---

# Schritt 2 von 4: Einrichten der Marketo-Lösung mit Resource Owner Password Control Connection {#step-2-of-4-set-up-the-marketo-solution-ropc}

Beginnen wir mit der Erstellung eines Benutzerkontos.

>[!PREREQUISITES]
>
>[Schritt 1 von 4: Installieren Sie die Marketo-Lösung mit Resource Owner Password Control Connection](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"}

## Neuen Benutzer erstellen {#create-a-new-user}

1. Melden Sie sich bei Dynamics an. Klicken Sie auf das Symbol Einstellungen und wählen Sie **[!UICONTROL Erweiterte Einstellungen]** aus.

   ![](assets/one.png)

1. Klicken Sie auf **[!UICONTROL Einstellungen]** und wählen Sie **[!UICONTROL Sicherheit]** aus.

   ![](assets/two.png)

1. Klicken Sie auf **[!UICONTROL Benutzer]**.

   ![](assets/three.png)

1. Klicken Sie auf **[!UICONTROL Neu]**.

   ![](assets/four.png)

1. Klicken Sie im neuen Fenster auf **[!UICONTROL Benutzer hinzufügen und lizenzieren]** .

   ![](assets/five.png)

1. Eine neue Registerkarte wird geöffnet. Klicken Sie oben auf der Seite auf **[!UICONTROL Admin]** .

   ![](assets/six.png)

1. Eine weitere neue Registerkarte wird geöffnet. Klicken Sie auf **[!UICONTROL Benutzer hinzufügen]**.

   ![](assets/seven.png)

   >[!IMPORTANT]
   >
   >Der Synchronisierungsbenutzer sollte über Leseberechtigungen für die Marketo-Konfiguration verfügen.

1. Geben Sie alle Ihre Informationen ein. Wenn Sie fertig sind, klicken Sie auf **[!UICONTROL Hinzufügen]**.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Dieser Name muss ein dedizierter Synchronisierungsbenutzer und nicht das Konto eines vorhandenen CRM-Benutzers sein. Es muss sich nicht um eine tatsächliche E-Mail-Adresse handeln.

1. Geben Sie die E-Mail ein, um die neuen Benutzeranmeldeinformationen zu erhalten, und klicken Sie auf **[!UICONTROL E-Mail senden und schließen]**.

   ![](assets/nine.png)

## Benutzerrolle &quot;Synchronisierung zuweisen&quot; {#assign-sync-user-role}

Weisen Sie die Benutzerrolle &quot;Marketo Sync User&quot;nur dem Marketo-Synchronisierungsbenutzer zu. Sie müssen sie keinen anderen Benutzern zuweisen.

>[!NOTE]
>
>Dies gilt für die Marketo-Version 4.0.0.14 und höher. Bei früheren Versionen müssen alle Benutzer über die Benutzerrolle &quot;Synchronisieren&quot;verfügen. Informationen zum Aktualisieren von Marketo finden Sie unter [Aktualisieren der Marketo-Lösung für Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md){target="_blank"}.

>[!IMPORTANT]
>
>Die Spracheinstellung des Synchronisierungsbenutzers [sollte auf Englisch](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us){target="_blank"} festgelegt sein.

1. Kehren Sie zur Registerkarte **[!UICONTROL Aktivierte Benutzer]** zurück und aktualisieren Sie die Benutzerliste.

   ![](assets/ten.png)

1. Bewegen Sie den Mauszeiger neben dem neu erstellten Marketo Sync-Benutzer und ein Kontrollkästchen wird angezeigt. Klicken Sie auf , um es auszuwählen.

   ![](assets/eleven.png)

1. Klicken Sie auf **[!UICONTROL Rollen verwalten]**.

   ![](assets/twelve.png)

1. Markieren Sie **[!UICONTROL Marketo Sync User]** und klicken Sie auf **[!UICONTROL OK]**.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Alle vom Synchronisierungsbenutzer in Ihrem CRM-System vorgenommenen Aktualisierungen werden _nicht_ mit Marketo synchronisiert.

## Konfigurieren der Marketo-Lösung {#configure-marketo-solution}

Fast da! Wir haben nur noch die Möglichkeit, Marketo Solution über den neu erstellten Benutzer zu informieren.

1. Gehen Sie zurück zum Abschnitt &quot;Erweiterte Einstellungen&quot;, klicken Sie auf das Symbol &quot;![](assets/image2015-5-13-15-3a49-3a19.png)&quot;neben &quot;Einstellungen&quot;und wählen Sie &quot;**[!UICONTROL Marketo-Konfiguration]**&quot;.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Wenn Sie im Einstellungsmenü nicht die Option **[!UICONTROL Marketo-Konfiguration]** sehen, aktualisieren Sie die Seite. Wenn dies nicht funktioniert, versuchen Sie, die Marketo-Lösung ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"} erneut zu veröffentlichen oder melden Sie sich ab und wieder an.[

1. Klicken Sie auf **[!UICONTROL Standard]**.

   ![](assets/fifteen.png)

1. Klicken Sie auf die Suchschaltfläche im Feld **[!UICONTROL Marketo-Benutzer]** und wählen Sie den erstellten Synchronisierungsbenutzer aus.

   ![](assets/sixteen.png)

1. Klicken Sie unten rechts auf das Symbol &quot;![](assets/image2015-3-13-15-3a10-3a11.png)&quot;, um die Änderungen zu speichern.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Klicken Sie oben rechts auf den **X** , um den Bildschirm zu schließen.

   ![](assets/seventeen.png)

1. Klicken Sie auf das Symbol &quot;![](assets/image2015-5-13-15-3a49-3a19-1.png)&quot;neben &quot;Einstellungen&quot;und wählen Sie &quot;**[!UICONTROL Lösungen]**&quot;.

   ![](assets/eighteen.png)

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Alle Anpassungen der Publish]** .

   ![](assets/nineteen.png)

>[!MORELIKETHIS]
>
>[Schritt 3 von 4: Verbinden der Marketo-Lösung mit der Kennwortsteuerungsverbindung des Ressourceneigentümers](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md){target="_blank"}
