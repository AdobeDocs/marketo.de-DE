---
description: Installieren von Marketo for [!DNL Microsoft Dynamics] 2016/Dynamics 365 On-Premise 1 von 3 - Marketo-Dokumente - Produktdokumentation
title: Installieren Sie Marketo for [!DNL Microsoft Dynamics] 2016/Dynamics 365 On-Premise Schritt 1 von 3
exl-id: 0a494ae7-87da-4ff9-bb47-990b957533e1
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Schritt 1 von 3: Synchronisierungsbenutzer für Marketo konfigurieren (2016 On-Premise /Dynamics 365 On-Premise) {#step-of-configure-sync-user-for-marketo-on-premises-2016}

Bevor Sie [!DNL Microsoft Dynamics] 2016 On-Premise/Dynamics 365 mit Marketo synchronisieren können, müssen Sie zunächst die Marketo-Lösung in Dynamics installieren.

>[!NOTE]
>
>Nachdem Sie Marketo mit einem CRM synchronisiert haben, können Sie kein neues CRM mit der bestehenden Marketo-Instanz synchronisieren.

>[!PREREQUISITES]
>
>Wenn Sie [!DNL Microsoft Dynamics] On-Premise verwenden, müssen Sie [Internet Facing Deployment](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) mit [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0+ (ADFS) konfiguriert haben. Hinweis: Das IFD-Dokument wird beim Klicken auf den Link automatisch heruntergeladen.
>
>[Laden Sie die Marketo-Lead-Management](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}Lösung herunter, bevor Sie beginnen.

>[!NOTE]
>
>**[!DNL Dynamics]Administratorberechtigungen erforderlich.**
>
>Sie benötigen CRM-Administratorrechte, um diese Synchronisierung durchzuführen.

1. Melden Sie sich bei **[!DNL Dynamics]an.** Klicken Sie auf das Dropdown **[!DNL Microsoft Dynamics]Menü** CRM und wählen Sie **[!UICONTROL Einstellungen]**.

   ![](assets/image2015-3-19-8-33-29.png)

1. Wählen **[!UICONTROL unter]** die Option **[!UICONTROL Lösungen]** aus.

   ![](assets/image2015-3-19-8-33-3.png)

1. Klicken Sie **[!UICONTROL Importieren]**.

   ![](assets/image2015-3-19-8-34-8.png)

1. Klicken Sie **[!UICONTROL Durchsuchen]** und wählen Sie die Lösung aus, die Sie [heruntergeladen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/image2015-3-19-9-20-56.png)

1. Zeigen Sie die Lösungsinformationen an und klicken Sie auf **[!UICONTROL Details zum Lösungspaket anzeigen]**.

   ![](assets/image2015-11-18-11-12-8.png)

1. Wenn Sie alle Details überprüft haben, klicken Sie auf **[!UICONTROL Schließen]**.

   ![](assets/step6.png)

1. Klicken Sie auf der Seite „Lösungsinformationen“ auf **[!UICONTROL Weiter]**.

   ![](assets/image2015-3-19-9-21-50.png)

1. Stellen Sie sicher, dass das Kontrollkästchen SDK-Option aktiviert ist. Klicken Sie **[!UICONTROL Importieren]**.

   ![](assets/image2015-3-19-9-19-12.png)

1. Warten Sie, bis der Import abgeschlossen ist.

   >[!TIP]
   >
   >Sie müssen Popups in Ihrem Browser aktivieren, um den Installationsprozess abzuschließen.

   ![](assets/image2015-3-11-11-34-9.png)

1. Laden Sie eine Protokolldatei herunter (falls gewünscht) und klicken Sie auf **[!UICONTROL Schließen]**.

   >[!NOTE]
   >
   >Möglicherweise wird die Meldung &quot;Marketo-Lead-Verwaltung abgeschlossen mit Warnung“ angezeigt. Dies ist voll und ganz zu erwarten.

   ![](assets/image2015-3-13-9-54-39.png)

1. Marketo Lead Management wird jetzt auf der Seite **[!UICONTROL Alle Lösungen]** angezeigt.

   ![](assets/image2015-3-19-8-40-38.png)

1. Wählen Sie die Marketo-Lösung aus und klicken Sie auf **[!UICONTROL Alle Anpassungen veröffentlichen]**.

   ![](assets/image2015-3-19-8-41-21.png)

   High Five! Die Installation ist abgeschlossen.

   >[!CAUTION]
   >
   >Die Deaktivierung eines der Marketo SDK Messaging-Prozesse führt zu einer fehlerhaften Installation!

   >[!MORELIKETHIS]
   >
   >[Installieren von Marketo for [!DNL Dynamics] 2015 On-Premise und 2016 365 On-Premise Schritt 2 von 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)
