---
unique-page-id: 3571805
description: 'Schritt 1 von 3: Installieren der Marketo-Lösung (On-Premises 2011) - Marketo Docs - Produktdokumentation'
title: Schritt 1 von 3 - Installieren der Marketo-Lösung (On-Premises 2011)
exl-id: 6e559b10-5273-4dc2-b98d-49c509cbeff7
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---

# Schritt 1 von 3: Installieren der Marketo-Lösung (On-Premises 2011) {#step-of-install-the-marketo-solution-on-premises}

Bevor Sie Microsoft Dynamics On-Premises und Marketo Engage synchronisieren können, müssen Sie zunächst die Marketo-Lösung in Dynamics installieren.

>[!NOTE]
>
>Nachdem Sie Marketo mit einem CRM synchronisiert haben, können Sie keine neue Synchronisierung durchführen, ohne die Instanz zu ersetzen.

>[!PREREQUISITES]
>
>Sie müssen [Internet Facing Deployment](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701){target="_blank"} (IFD) mit [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} 2.0, 2.1 oder 3.0 (ADFS) konfiguriert haben. **Hinweis**: Das IFD-Dokument wird beim Klicken auf den Link automatisch heruntergeladen.
>
>[Laden Sie die Marketo-Lead-Management-Lösung herunter](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} , bevor Sie beginnen.

>[!NOTE]
>
>**Erforderliche Dynamics-Administratorberechtigungen**.
>
>Sie benötigen CRM-Administratorberechtigungen, um diese Synchronisierung durchzuführen.

1. Melden Sie sich bei Dynamics an und wählen Sie im Menü unten links **[!UICONTROL Einstellungen]** aus.

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. Wählen Sie **[!UICONTROL Lösungen]** im Baum aus.

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. Klicken Sie auf **[!UICONTROL Importieren]**.

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. Klicken Sie auf **[!UICONTROL Durchsuchen]**. Wählen Sie die Marketo Lead Management-Lösung aus, die Sie [heruntergeladen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} haben. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. Zeigen Sie die Lösungsinformationen an und klicken Sie auf **[!UICONTROL Details zum Lösungspaket anzeigen]**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Wenn Sie alle Details überprüft haben, klicken Sie auf **[!UICONTROL Schließen]**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Klicken Sie auf der Seite Lösungsinformationen auf **[!UICONTROL Weiter]**.

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. Stellen Sie sicher, dass das Kontrollkästchen SDK-Nachrichtenoption aktiviert ist. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/image2015-4-2-11-3a42-3a37.png)

   >[!TIP]
   >
   >Sie müssen Popups in Ihrem Browser aktivieren, um den Installationsprozess abzuschließen.

1. Warten Sie nun, bis der Import abgeschlossen ist. Steh auf und mach einige Strecken.

   ![](assets/image2015-4-2-11-3a43-3a51.png)

1. Klicken Sie auf **[!UICONTROL Schließen]**.

   >[!NOTE]
   >
   >Möglicherweise wird eine Meldung mit der Meldung &quot;Marketo Lead Management wurde mit Warnung abgeschlossen&quot;angezeigt. Dies ist völlig zu erwarten.

   ![](assets/image2015-4-2-11-3a44-3a44.png)

1. Die Marketo-Lead-Verwaltung wird jetzt auf der Seite **Alle Lösungen** angezeigt.

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. Wählen Sie Marketo Lead Management und klicken Sie auf **[!UICONTROL Publish All Customizations]**.

   ![](assets/image2015-4-2-11-3a48-3a21.png)

>[!CAUTION]
>
>Die Deaktivierung eines der Marketo SDK Messaging-Prozesse führt zu einer fehlerhaften Installation!

>[!MORELIKETHIS]
>
>[Schritt 2 von 3: Einrichten des Marketo-Synchronisierungsbenutzers in Dynamics (On-Premises 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2011.md){target="_blank"}
