---
description: Installieren Sie Marketo für Microsoft Dynamics 2016/Dynamics 365 On-Premises 1 von 3 - Marketo Docs - Produktdokumentation
title: Installieren von Marketo für Microsoft Dynamics 2016/Dynamics 365 On-Premises Schritt 1 von 3
exl-id: 0a494ae7-87da-4ff9-bb47-990b957533e1
source-git-commit: 3fb93520a653109845c3b40aba20304c6163214f
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---

# Schritt 1 von 3: Konfigurieren der Synchronisierungsbenutzer für Marketo (On-Premise 2016/Dynamics 365 On-Premises) {#step-of-configure-sync-user-for-marketo-on-premises-2016}

Bevor Sie Microsoft Dynamics 2016 On-Prem/Dynamics 365 mit Marketo synchronisieren können, müssen Sie zunächst die Marketo-Lösung in Dynamics installieren.

>[!NOTE]
>
>Nachdem Sie Marketo mit einem CRM synchronisiert haben, können Sie kein neues CRM mit der bestehenden Marketo-Instanz synchronisieren.

>[!PREREQUISITES]
>
>Wenn Sie Microsoft Dynamics On-Premise verwenden, müssen Sie [Bereitstellung im Internet](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) mit [Active Directory Federation-Dienste](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0+ (ADFS) konfiguriert. Hinweis: Das IFD-Dokument wird automatisch heruntergeladen, wenn Sie auf den Link klicken.
>
>[Marketo-Lead-Management-Lösung herunterladen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) bevor Sie beginnen.

>[!NOTE]
>
>**Dynamics-Administratorberechtigungen erforderlich.**
>
>Sie benötigen CRM-Administratorberechtigungen, um diese Synchronisierung durchzuführen.

1. Anmelden bei **Dynamics.** Klicken Sie auf **Microsoft Dynamics CRM** Dropdown-Menü und **Einstellungen**.

   ![](assets/image2015-3-19-8-33-29.png)

1. under **Einstellungen** auswählen **Lösungen**.

   ![](assets/image2015-3-19-8-33-3.png)

1. Klicken **Import**.

   ![](assets/image2015-3-19-8-34-8.png)

1. Klicken **Durchsuchen** und wählen Sie die gewünschte Lösung aus [heruntergeladen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Klicken **Nächste**.

   ![](assets/image2015-3-19-9-20-56.png)

1. Zeigen Sie die Lösungsinformationen an und klicken Sie auf **Lösungspaketdetails anzeigen**.

   ![](assets/image2015-11-18-11-12-8.png)

1. Wenn Sie alle Details überprüft haben, klicken Sie auf **Schließen**.

   ![](assets/step6.png)

1. Klicken Sie auf der Seite Lösungsinformationen auf **Nächste**.

   ![](assets/image2015-3-19-9-21-50.png)

1. Stellen Sie sicher, dass das Kontrollkästchen SDK-Option aktiviert ist. Klicken **Import**.

   ![](assets/image2015-3-19-9-19-12.png)

1. Warten Sie, bis der Import abgeschlossen ist.

   >[!TIP]
   >
   >Sie müssen Popups in Ihrem Browser aktivieren, um den Installationsprozess abzuschließen.

   ![](assets/image2015-3-11-11-34-9.png)

1. Laden Sie eine Protokolldatei herunter (falls gewünscht) und klicken Sie auf **Schließen**.

   >[!NOTE]
   >
   >Möglicherweise wird eine Meldung mit der Meldung &quot;Marketo Lead Management wurde mit Warnung abgeschlossen&quot;angezeigt. Dies ist völlig zu erwarten.

   ![](assets/image2015-3-13-9-54-39.png)

1. Die Marketo-Lead-Verwaltung wird jetzt im **Alle Lösungen** Seite.

   ![](assets/image2015-3-19-8-40-38.png)

1. Wählen Sie die Marketo-Lösung aus und klicken Sie auf **Alle Anpassungen veröffentlichen**.

   ![](assets/image2015-3-19-8-41-21.png)

   Hoch fünf! Die Installation ist abgeschlossen.

   >[!CAUTION]
   >
   >Die Deaktivierung eines der Marketo SDK Messaging-Prozesse führt zu einer fehlerhaften Installation!

   >[!MORELIKETHIS]
   >
   >[Installieren Sie Marketo für Dynamics 2015 On-Prem und 2016 365 On-Prem Schritt 2 von 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)