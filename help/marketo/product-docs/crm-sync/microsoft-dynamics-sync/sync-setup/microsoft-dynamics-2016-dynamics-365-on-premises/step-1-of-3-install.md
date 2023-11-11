---
description: Installieren Sie Marketo für Microsoft Dynamics 2016/Dynamics 365 On-Premises 1 von 3 - Marketo Docs - Produktdokumentation
title: Installieren von Marketo für Microsoft Dynamics 2016/Dynamics 365 On-Premises Schritt 1 von 3
exl-id: 0a494ae7-87da-4ff9-bb47-990b957533e1
feature: Microsoft Dynamics
source-git-commit: 15cb3ddcd82fa1ba60fae3aa1adaac3d5964a0fa
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# Schritt 1 von 3: Konfigurieren der Synchronisierungsbenutzer für Marketo (On-Premise 2016/Dynamics 365 On-Premises) {#step-of-configure-sync-user-for-marketo-on-premises-2016}

Bevor Sie Microsoft Dynamics 2016 On-Prem/Dynamics 365 mit Marketo Engage synchronisieren können, müssen Sie zunächst die Marketo-Lösung in Dynamics installieren.

>[!NOTE]
>
>Nachdem Sie Marketo mit einem CRM synchronisiert haben, können Sie kein neues CRM mit der bestehenden Marketo-Instanz synchronisieren.

>[!PREREQUISITES]
>
>Wenn Sie Microsoft Dynamics On-Premise verwenden, müssen Sie [Bereitstellung im Internet](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701){target="_blank"} (IFD) with [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} 2.0+ (ADFS) konfiguriert. Hinweis: Das IFD-Dokument wird beim Klicken auf den Link automatisch heruntergeladen.
>
>[Marketo-Lead-Management-Lösung herunterladen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} bevor Sie beginnen.

>[!NOTE]
>
>**Dynamics Admin-Berechtigungen erforderlich**.
>
>Sie benötigen CRM-Administratorberechtigungen, um diese Synchronisierung durchzuführen.

1. Melden Sie sich bei Dynamics an. Klicken Sie auf **[!UICONTROL Microsoft Dynamics CRM]** Dropdown-Menü und wählen Sie **[!UICONTROL Einstellungen]**.

   ![](assets/image2015-3-19-8-33-29.png)

1. under **[!UICONTROL Einstellungen]** auswählen **[!UICONTROL Lösungen]**.

   ![](assets/image2015-3-19-8-33-3.png)

1. Klicks **[!UICONTROL Import]**.

   ![](assets/image2015-3-19-8-34-8.png)

1. Klicks **[!UICONTROL Durchsuchen]** und wählen Sie die gewünschte Lösung aus [heruntergeladen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}. Klicken Sie auf **Weiter**.

   ![](assets/image2015-3-19-9-20-56.png)

1. Anzeigen der Lösungsinformationen und klicken Sie auf **[!UICONTROL Lösungspaketdetails anzeigen]**.

   ![](assets/image2015-11-18-11-12-8.png)

1. Wenn Sie alle Details überprüft haben, klicken Sie auf **[!UICONTROL Schließen]**.

   ![](assets/step6.png)

1. Klicken Sie auf der Seite Lösungsinformationen auf **[!UICONTROL Nächste]**.

   ![](assets/image2015-3-19-9-21-50.png)

1. Stellen Sie sicher, dass das Kontrollkästchen SDK-Option aktiviert ist. Klicks **[!UICONTROL Import]**.

   ![](assets/image2015-3-19-9-19-12.png)

1. Warten Sie, bis der Import abgeschlossen ist.

   >[!TIP]
   >
   >Sie müssen Popups in Ihrem Browser aktivieren, um den Installationsprozess abzuschließen.

   ![](assets/image2015-3-11-11-34-9.png)

1. Laden Sie eine Protokolldatei herunter (falls gewünscht) und klicken Sie auf **[!UICONTROL Schließen]**.

   >[!NOTE]
   >
   >Möglicherweise wird eine Meldung mit der Meldung &quot;Marketo Lead Management wurde mit Warnung abgeschlossen&quot;angezeigt. Dies ist völlig zu erwarten.

   ![](assets/image2015-3-13-9-54-39.png)

1. Die Marketo-Lead-Verwaltung wird jetzt im **[!UICONTROL Alle Lösungen]** Seite.

   ![](assets/image2015-3-19-8-40-38.png)

1. Wählen Sie die Marketo-Lösung aus und klicken Sie auf **[!UICONTROL Alle Anpassungen veröffentlichen]**.

   ![](assets/image2015-3-19-8-41-21.png)

   Hoch fünf! Die Installation ist abgeschlossen.

   >[!CAUTION]
   >
   >Die Deaktivierung eines der Marketo SDK Messaging-Prozesse führt zu einer fehlerhaften Installation!

   >[!MORELIKETHIS]
   >
   >[Installieren Sie Marketo für Dynamics 2015 On-Prem und 2016 365 On-Prem Schritt 2 von 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md){target="_blank"}
