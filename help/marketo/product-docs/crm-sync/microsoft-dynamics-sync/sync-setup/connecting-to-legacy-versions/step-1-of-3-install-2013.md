---
unique-page-id: 3571813
description: 'Schritt 1 von 3: Installieren der Marketo-Lösung in Dynamics (2013 On-Premise) - Marketo-Dokumente - Produktdokumentation'
title: 'Schritt 1 von 3: Installieren der Marketo-Lösung in Dynamics (2013 On-Premise)'
exl-id: 89f90bca-b459-447f-bbdd-363f232a1059
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# Schritt 1 von 3: Installieren der Marketo-Lösung in [!DNL Dynamics] (2013 On-Premise) {#step-of-install-the-marketo-solution-in-dynamics-on-premises}

Bevor Sie [!DNL Microsoft Dynamics] On-Premise und Marketo synchronisieren können, müssen Sie zunächst die Marketo-Lösung in [!DNL Dynamics] installieren.

>[!NOTE]
>
>Nach dem Synchronisieren von Marketo mit einem CRM können Sie keine neue Synchronisierung durchführen, ohne die Instanz zu ersetzen.

>[!PREREQUISITES]
>
>Sie müssen [Internet Facing Deployment](https://learn.microsoft.com/en-us/dynamics365/customerengagement/on-premises/deploy/configure-an-internet-facing-deployment){target="_blank"} (IFD) mit [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} 2.0, 2.1 oder 3.0 (ADFS) konfiguriert haben. Hinweis: Das IFD-Dokument wird beim Klicken auf den Link automatisch heruntergeladen.
>
>[Laden Sie die Marketo-Lösung herunter](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} bevor Sie beginnen.

>[!NOTE]
>
>**[!DNL Dynamics]Administratorberechtigungen erforderlich.**
>
>Sie benötigen CRM-Administratorrechte, um diese Synchronisierung durchzuführen.

1. Anmelden bei **[!DNL Dynamics]**. Klicken Sie auf das Dropdown-**&#x200B;** Microsoft Dynamics CRM und wählen Sie **[!UICONTROL Einstellungen]**.

   ![](assets/image2014-12-11-10-3a39-3a41.png)

1. Wählen **[!UICONTROL unter]** die Option **[!UICONTROL Lösungen]** aus.

   ![](assets/image2014-12-11-10-3a39-3a51.png)

1. Klicken Sie **[!UICONTROL Importieren]**.

   ![](assets/image2015-3-26-9-3a52-3a10.png)

1. Klicken Sie **[!UICONTROL Durchsuchen]** und wählen Sie die [heruntergeladene Lösung](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) aus. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/image2015-3-26-9-3a54-3a1.png)

1. Zeigen Sie die [!UICONTROL Lösungsinformationen] an und klicken Sie auf **[!UICONTROL Details zum Lösungspaket anzeigen]**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Wenn Sie alle Details überprüft haben, klicken Sie auf **[!UICONTROL Schließen]**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Klicken Sie auf der Seite [!UICONTROL Lösungsinformationen] auf **[!UICONTROL Weiter]**.

   ![](assets/image2015-3-26-9-3a55-3a17.png)

1. Stellen Sie sicher, dass die Option SDK aktiviert ist. Klicken Sie **[!UICONTROL Importieren]**.

   ![](assets/image2015-3-26-10-3a3-3a11.png)

1. Warten Sie, bis der Import abgeschlossen ist.

   >[!TIP]
   >
   >Sie müssen Popups in Ihrem Browser aktivieren, um den Installationsprozess abzuschließen.

   ![](assets/image2014-12-11-10-3a41-3a5.png)

1. Laden Sie eine Protokolldatei herunter (falls gewünscht) und klicken Sie auf **[!UICONTROL Schließen]**.

   >[!NOTE]
   >
   >Möglicherweise wird die Meldung &quot;Marketo-Lead-Verwaltung abgeschlossen mit Warnung“ angezeigt. Dies ist voll und ganz zu erwarten.

   ![](assets/image2014-12-11-10-3a41-3a14.png)

1. Marketo Lead Management wird jetzt auf der Seite **[!UICONTROL Alle Lösungen]** angezeigt.

   ![](assets/image2015-3-26-10-3a1-3a21.png)

1. Wählen Sie die Marketo-Lösung aus und klicken Sie auf **[!UICONTROL Alle Anpassungen veröffentlichen]**.

   ![](assets/image2014-12-11-10-3a41-3a32.png)

>[!CAUTION]
>
>Die Deaktivierung eines der Marketo SDK Messaging-Prozesse führt zu einer fehlerhaften Installation!

>[!MORELIKETHIS]
>
>[Schritt 2 von 3: Konfigurieren von Synchronisierungsbenutzenden für Marketo (2013 On-Premise)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-configure-2013.md){target="_blank"}
