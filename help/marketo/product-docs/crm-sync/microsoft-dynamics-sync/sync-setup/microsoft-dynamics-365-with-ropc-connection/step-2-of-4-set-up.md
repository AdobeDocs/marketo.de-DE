---
description: 'Schritt 2 von 4: Einrichten der Marketo-Lösung mit der Kennwortkontrollverbindung für Ressourcenbesitzer - Marketo-Dokumente - Produktdokumentation'
title: 'Schritt 2 von 4: Einrichten der Marketo-Lösung mit der Kennwortsteuerungsverbindung für Ressourcenbesitzer'
exl-id: 41c05910-d8e3-4fb7-8f68-17ee10294e57
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '441'
ht-degree: 0%

---

# Schritt 2 von 4: Einrichten der Marketo-Lösung mit der Kennwortsteuerungsverbindung für Ressourcenbesitzer {#step-2-of-4-set-up-the-marketo-solution-ropc}

Beginnen wir mit der Erstellung eines Benutzerkontos.

>[!PREREQUISITES]
>
>[Schritt 1 von 4: Installieren Sie die Marketo-Lösung mit der Kennwortsteuerungsverbindung des Ressourceneigentümers](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md){target="_blank"}

## Neuen Benutzer erstellen {#create-a-new-user}

1. Melden Sie sich bei [!DNL Dynamics] an. Klicken Sie auf [!UICONTROL Einstellungen] und wählen Sie **[!UICONTROL Erweiterte Einstellungen]** aus.

   ![](assets/one.png)

1. Klicken Sie **[!UICONTROL Einstellungen]** und wählen Sie **[!UICONTROL Sicherheit]** aus.

   ![](assets/two.png)

1. Klicken Sie auf **[!UICONTROL Benutzer]**.

   ![](assets/three.png)

1. Klicken Sie auf **[!UICONTROL Neu]**.

   ![](assets/four.png)

1. Klicken Sie **[!UICONTROL neuen Fenster auf]** Benutzer hinzufügen und lizenzieren“.

   ![](assets/five.png)

1. Eine neue Registerkarte wird geöffnet. Klicken **[!UICONTROL oben]** der Seite auf „Admin“.

   ![](assets/six.png)

1. Eine weitere neue Registerkarte wird geöffnet. Klicken Sie **[!UICONTROL Benutzer hinzufügen]**.

   ![](assets/seven.png)

   >[!IMPORTANT]
   >
   >Der Synchronisierungsbenutzer sollte über Leseberechtigungen für die Marketo-Konfiguration verfügen.

1. Geben Sie alle Ihre Informationen ein. Wenn Sie fertig sind, klicken Sie auf **[!UICONTROL Hinzufügen]**.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Dieser Name muss ein dedizierter Synchronisierungsbenutzer sein und nicht das Konto eines vorhandenen CRM-Benutzers. Es muss keine tatsächliche E-Mail-Adresse sein.

1. Geben Sie die E-Mail-Adresse ein, um die Anmeldeinformationen für den neuen Benutzer zu erhalten, und klicken Sie auf **[!UICONTROL E-Mail senden und schließen]**.

   ![](assets/nine.png)

## Assign Sync User Role {#assign-sync-user-role}

Weisen Sie die Rolle Marketo-Synchronisierungsbenutzer nur dem Marketo-Synchronisierungsbenutzer zu. Sie müssen sie keinem anderen Benutzer zuweisen.

>[!NOTE]
>
>Dies gilt für die Marketo-Version 4.0.0.14 und höher. Bei früheren Versionen müssen alle Benutzer über die Rolle „Benutzer synchronisieren“ verfügen. Informationen zum Upgrade von Marketo finden Sie unter [Upgrade der Marketo-Lösung für [!DNL Microsoft Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>Die Spracheinstellung des Synchronisierungsbenutzers [sollte auf Englisch festgelegt werden](https://learn.microsoft.com/en-us/power-platform/admin/enable-languages){target="_blank"}.

1. Gehen Sie zurück zur Registerkarte [!UICONTROL Aktivierte Benutzer] und aktualisieren Sie die Benutzerliste.

   ![](assets/ten.png)

1. Bewegen Sie den Mauszeiger neben dem neu erstellten Marketo-Synchronisierungsbenutzer, und ein Kontrollkästchen wird angezeigt. Zur Auswahl klicken.

   ![](assets/eleven.png)

1. Klicken Sie **[!UICONTROL Rollen verwalten]**.

   ![](assets/twelve.png)

1. Markieren Sie **[!UICONTROL Marketo-Synchronisierungsbenutzer]** und klicken Sie auf **[!UICONTROL OK]**.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Alle Aktualisierungen, die der Synchronisierungsbenutzer in Ihrem CRM vorgenommen hat, _nicht_ wieder mit Marketo synchronisiert.

## Marketo-Lösung konfigurieren {#configure-marketo-solution}

Fast da! Uns bleibt nur noch, die Marketo-Lösung über den neu erstellten Benutzer zu informieren.

1. Gehen Sie zurück zum Abschnitt [!UICONTROL Erweiterte Einstellungen] und klicken Sie auf das ![](assets/image2015-5-13-15-3a49-3a19.png) neben [!UICONTROL Einstellungen] und wählen Sie **[!UICONTROL Marketo Config]**.

   ![](assets/fourteen.png)

   >[!NOTE]
   >
   >Wenn **[!UICONTROL Marketo Config]** im Menü [!UICONTROL Einstellungen] nicht angezeigt wird, aktualisieren Sie die Seite. Wenn dies nicht funktioniert, versuchen Sie erneut, [die Marketo-Lösung zu veröffentlichen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md) oder melden Sie sich ab und wieder an.

1. Klicken Sie auf **[!UICONTROL Standard]**.

   ![](assets/fifteen.png)

1. Klicken Sie im Feld **[!UICONTROL Marketo-Benutzer]** auf die Schaltfläche „Suchen“ und wählen Sie den erstellten Synchronisierungsbenutzer aus.

   ![](assets/sixteen.png)

1. Klicken Sie auf das ![](assets/image2015-3-13-15-3a10-3a11.png) in der rechten unteren Ecke, um die Änderungen zu speichern.

   ![](assets/image2015-3-13-15-3a3-3a3.png)

1. Klicken Sie auf **X** oben rechts, um den Bildschirm zu schließen.

   ![](assets/seventeen.png)

1. Klicken Sie auf das ![](assets/image2015-5-13-15-3a49-3a19-1.png) neben [!UICONTROL Einstellungen] und wählen Sie **[!UICONTROL Lösungen]** aus.

   ![](assets/eighteen.png)

1. Klicken Sie auf **[!UICONTROL Schaltfläche Alle Anpassungen]**.

   ![](assets/nineteen.png)

>[!MORELIKETHIS]
>
>[Schritt 3 von 4: Verbinden der Marketo-Lösung mit der Kennwortsteuerungsverbindung des Ressourceneigentümers](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md){target="_blank"}
