---
description: 'Schritt 1 von 4: Installieren der Marketo-Lösung mit der Kennwortkontrollverbindung für Ressourcenbesitzer - Marketo-Dokumente - Produktdokumentation'
title: 'Schritt 1 von 4: Installieren der Marketo-Lösung mit der Kennwortsteuerungsverbindung des Ressourceneigentümers'
exl-id: aab3bbb8-4e52-4c40-94d1-631af1d63f9f
feature: Microsoft Dynamics
source-git-commit: 2eb61d43f2f470d42e1b50ab8edc99e4e25c23cf
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 1%

---

# Schritt 1 von 4: Installieren der Marketo-Lösung mit der Kennwortsteuerungsverbindung des Ressourceneigentümers {#step-1-of-4-install-the-marketo-solution-ropc}

Bevor Sie Microsoft Dynamics 365 und Marketo Engage synchronisieren können, müssen Sie zunächst die Marketo-Lösung in Dynamics installieren. **Dynamics-Administratorberechtigungen sind erforderlich**.

>[!CAUTION]
>
>* Aktivieren Sie die Synchronisierung benutzerdefinierter Entitäten nicht, bevor die erste Synchronisierung abgeschlossen ist. Sie werden per E-Mail benachrichtigt, sobald die erste Synchronisierung abgeschlossen ist.
>* Wenn Sie für Ihre Dynamics-Synchronisierung die Multi-Factor Authentication (MFA) aktiviert haben, müssen Sie sie deaktivieren, damit Dynamics ordnungsgemäß mit Marketo synchronisiert werden kann. Weitere Informationen erhalten Sie vom [Marketo-Support](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"}.

>[!NOTE]
>
>Nach dem Synchronisieren von Marketo mit einem CRM können Sie keine neue Synchronisierung durchführen, ohne die Instanz zu ersetzen.

>[!PREREQUISITES]
>
>[Marketo Lead Management-Lösung herunterladen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)

1. Melden Sie sich bei **[Microsoft Office 365](https://login.microsoftonline.com/)** an.

   ![](assets/image2015-3-16-15-3a58-3a55.png)

1. Klicken Sie auf ![](assets/image2015-3-16-16-3a1-3a13.png) Menü und wählen Sie **[!UICONTROL CRM]** aus.

   ![](assets/image2015-3-16-16-3a0-3a10.png)

1. Klicken Sie auf ![](assets/image2015-5-13-10-3a5-3a8.png) Menü. Wählen Sie im Dropdown-Menü **[!UICONTROL Einstellungen]** und dann **[!UICONTROL Lösungen]** aus.

   ![](assets/image2015-5-13-10-3a4-3a1.png)

1. Klicken Sie **[!UICONTROL Importieren]**.

   ![](assets/image2015-3-19-8-3a34-3a8.png)

1. Klicken Sie **[!UICONTROL Datei wählen]**. Wählen Sie die Marketo-Lead-Management-Lösung aus[ die Sie heruntergeladen ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/image2015-10-9-14-3a44-3a14.png)

1. Zeigen Sie die Lösungsinformationen an und klicken Sie auf **[!UICONTROL Details zum Lösungspaket anzeigen]**.

   ![](assets/image2015-10-9-15-3a4-3a16.png)

1. Wenn Sie alle Details überprüft haben, klicken Sie auf **[!UICONTROL Schließen]**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Klicken Sie nun auf der Seite „Lösungsinformationen“ auf **[!UICONTROL Weiter]**.

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. Stellen Sie sicher, dass das Kontrollkästchen SDK-Option aktiviert ist. Klicken Sie **[!UICONTROL Importieren]**.

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >Sie müssen Popups in Ihrem Browser aktivieren, um den Installationsprozess abzuschließen.

1. Warten Sie nun, bis der Import abgeschlossen ist. Steh auf und mach Dehnungen.

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. Klicken Sie auf **[!UICONTROL Schließen]**.

   >[!NOTE]
   >
   >Möglicherweise wird die Meldung &quot;Marketo-Lead-Verwaltung abgeschlossen mit Warnung“ angezeigt. Dies ist voll und ganz zu erwarten.

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. &quot;Marketo Lead Management“ wird jetzt in der Liste der Lösungen angezeigt.

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. Wählen Sie **[!UICONTROL Marketo-Lead-]** aus und klicken Sie auf **[!UICONTROL Publish-Anpassungen für alle]**.

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   Gut gemacht! Die Installation ist abgeschlossen.

   >[!MORELIKETHIS]
   >
   >[Schritt 2 von 4: Richten Sie die Marketo-Lösung mit der Kennwortsteuerungsverbindung für Ressourcenbesitzer ein](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md){target="_blank"}
