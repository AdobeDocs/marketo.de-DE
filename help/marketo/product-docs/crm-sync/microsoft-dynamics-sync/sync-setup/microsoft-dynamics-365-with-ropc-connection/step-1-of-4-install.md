---
description: 'Schritt 1 von 4: Installieren der Marketo-Lösung mit Resource Owner Password Control Connection - Marketo Docs - Produktdokumentation'
title: 'Schritt 1 von 4: Installieren der Marketo-Lösung mit Resource Owner Password Control Connection'
exl-id: aab3bbb8-4e52-4c40-94d1-631af1d63f9f
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Schritt 1 von 4: Installieren der Marketo-Lösung mit Resource Owner Password Control Connection {#step-1-of-4-install-the-marketo-solution-ropc}

Bevor Sie Microsoft Dynamics 365 und Marketo synchronisieren können, müssen Sie zunächst die Marketo-Lösung in Dynamics installieren. **Dynamics-Administratorberechtigungen sind erforderlich.**

>[!CAUTION]
>
>* Aktivieren Sie nicht die Synchronisierung benutzerdefinierter Entitäten, bevor die erste Synchronisierung abgeschlossen ist. Sie werden per E-Mail benachrichtigt, sobald die erste Synchronisation abgeschlossen ist.
>* Wenn Sie die Multi-Factor-Authentifizierung (MFA) für Ihre Dynamics Sync aktiviert haben, müssen Sie sie deaktivieren, damit Dynamics ordnungsgemäß mit Marketo synchronisiert werden kann. Für weitere Informationen wenden Sie sich bitte an [Marketo-Support](https://nation.marketo.com/t5/Support/ct-p/Support).

>[!NOTE]
>
>Nachdem Sie Marketo mit einem CRM synchronisiert haben, können Sie keine neue Synchronisierung durchführen, ohne die Instanz zu ersetzen.

>[!PREREQUISITES]
>
>[Marketo-Lead-Management-Lösung herunterladen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)

1. Anmelden bei **[Microsoft Office 365](https://login.microsoftonline.com/)**.

   ![](assets/image2015-3-16-15-3a58-3a55.png)

1. Klicks ![](assets/image2015-3-16-16-3a1-3a13.png) Menü und wählen Sie **CRM**.

   ![](assets/image2015-3-16-16-3a0-3a10.png)

1. Klicks ![](assets/image2015-5-13-10-3a5-3a8.png) Menü. Wählen Sie im Dropdown-Menü **Einstellungen** und wählen Sie **Lösungen**.

   ![](assets/image2015-5-13-10-3a4-3a1.png)

1. Klicks **Importieren.**

   ![](assets/image2015-3-19-8-3a34-3a8.png)

1. Klicks **Wählen Sie Datei aus.** Wählen Sie die Marketo Lead Management-Lösung aus, die Sie verwenden [heruntergeladen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Klicks **Nächste**.

   ![](assets/image2015-10-9-14-3a44-3a14.png)

1. Anzeigen der Lösungsinformationen und klicken Sie auf **Lösungspaketdetails anzeigen**.

   ![](assets/image2015-10-9-15-3a4-3a16.png)

1. Wenn Sie alle Details überprüft haben, klicken Sie auf **Schließen**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Klicken Sie nun auf der Seite Lösungsinformationen auf **Nächste**.

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. Stellen Sie sicher, dass das Kontrollkästchen SDK-Option aktiviert ist. Klicks **Import**.

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >Sie müssen Popups in Ihrem Browser aktivieren, um den Installationsprozess abzuschließen.

1. Warten Sie nun, bis der Import abgeschlossen ist. Steh auf und mach einige Strecken.

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. Klicken Sie auf **Schließen.**

   >[!NOTE]
   >
   >Möglicherweise wird eine Meldung mit der Meldung &quot;Marketo Lead Management wurde mit Warnung abgeschlossen&quot;angezeigt. Dies ist völlig zu erwarten.

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. Marketo Lead Management wird jetzt in der Liste der Lösungen angezeigt.

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. Auswählen **Marketo Lead Management** und klicken **Alle Anpassungen veröffentlichen.**

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   Hoch fünf! Die Installation ist abgeschlossen.

   >[!MORELIKETHIS]
   >
   >[Schritt 2 von 4: Einrichten der Marketo-Lösung mit Resource Owner Password Control Connection](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)
