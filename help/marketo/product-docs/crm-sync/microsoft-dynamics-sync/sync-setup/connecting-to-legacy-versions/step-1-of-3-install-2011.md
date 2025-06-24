---
unique-page-id: 3571805
description: 'Schritt 1 von 3: Installieren der Marketo-Lösung (2011, On-Premise) - Dokumentation zu Marketo - Produktdokumentation'
title: 'Schritt 1 von 3: Installieren der Marketo-Lösung (2011 On-Premise)'
exl-id: 6e559b10-5273-4dc2-b98d-49c509cbeff7
feature: Microsoft Dynamics
source-git-commit: e3f61755dccd9bea1378a429fc428b440fc3ecb4
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 2%

---

# Schritt 1 von 3: Marketo-Lösung installieren (2011 On-Premise) {#step-of-install-the-marketo-solution-on-premises}

Bevor Sie Microsoft Dynamics On-Premise und Marketo Engage synchronisieren können, müssen Sie zunächst die Marketo-Lösung in Dynamics installieren.

>[!NOTE]
>
>Nach dem Synchronisieren von Marketo mit einem CRM können Sie keine neue Synchronisierung durchführen, ohne die Instanz zu ersetzen.

>[!PREREQUISITES]
>
>Sie müssen [Internet Facing Deployment](https://learn.microsoft.com/en-us/dynamics365/customerengagement/on-premises/deploy/configure-an-internet-facing-deployment){target="_blank"} (IFD) mit [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} 2.0, 2.1 oder 3.0 (ADFS) konfiguriert haben. **Hinweis**: Das IFD-Dokument wird beim Klicken auf den Link automatisch heruntergeladen.
>
>[Laden Sie die Marketo-Lead-Management](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}Lösung herunter, bevor Sie beginnen.

>[!NOTE]
>
>**Dynamics-Administratorberechtigungen erforderlich**.
>
>Sie benötigen CRM-Administratorrechte, um diese Synchronisierung durchzuführen.

1. Melden Sie sich bei Dynamics an und **[!UICONTROL Sie]** Menü unten links auf „Einstellungen“.

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. Wählen **[!UICONTROL in]** Struktur „Lösungen“ aus.

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. Klicken Sie **[!UICONTROL Importieren]**.

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. Klicken Sie **[!UICONTROL Durchsuchen]**. Wählen Sie die Marketo-Lead-Management-Lösung aus[ die Sie heruntergeladen ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. Zeigen Sie die Lösungsinformationen an und klicken Sie auf **[!UICONTROL Details zum Lösungspaket anzeigen]**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Wenn Sie alle Details überprüft haben, klicken Sie auf **[!UICONTROL Schließen]**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Klicken Sie auf der Seite „Lösungsinformationen“ auf **[!UICONTROL Weiter]**.

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. Stellen Sie sicher, dass das Kontrollkästchen SDK-Nachrichtenoption aktiviert ist. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/image2015-4-2-11-3a42-3a37.png)

   >[!TIP]
   >
   >Sie müssen Popups in Ihrem Browser aktivieren, um den Installationsprozess abzuschließen.

1. Warten Sie nun, bis der Import abgeschlossen ist. Steh auf und mach Dehnungen.

   ![](assets/image2015-4-2-11-3a43-3a51.png)

1. Klicken Sie auf **[!UICONTROL Schließen]**.

   >[!NOTE]
   >
   >Möglicherweise wird die Meldung &quot;Marketo-Lead-Verwaltung abgeschlossen mit Warnung“ angezeigt. Dies ist voll und ganz zu erwarten.

   ![](assets/image2015-4-2-11-3a44-3a44.png)

1. Marketo Lead Management wird jetzt auf der Seite **Alle Lösungen** angezeigt.

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. Wählen Sie Marketo Lead-Verwaltung aus und klicken Sie auf **[!UICONTROL Alle Anpassungen veröffentlichen]**.

   ![](assets/image2015-4-2-11-3a48-3a21.png)

>[!CAUTION]
>
>Die Deaktivierung eines der Marketo SDK Messaging-Prozesse führt zu einer fehlerhaften Installation!

>[!MORELIKETHIS]
>
>[Schritt 2 von 3: Einrichten des Marketo-Synchronisierungsbenutzers in Dynamics (2011 On-Premise)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2011.md){target="_blank"}
