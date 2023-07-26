---
unique-page-id: 3571813
description: 'Schritt 1 von 3: Installieren der Marketo-Lösung in Dynamics (On-Premises 2013) - Marketo Docs - Produktdokumentation'
title: 'Schritt 1 von 3: Installieren der Marketo-Lösung in Dynamics (On-Premises 2013)'
exl-id: 89f90bca-b459-447f-bbdd-363f232a1059
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# Schritt 1 von 3: Installieren der Marketo-Lösung in Dynamics (On-Premises 2013) {#step-of-install-the-marketo-solution-in-dynamics-on-premises}

Bevor Sie Microsoft Dynamics On-Premises und Marketo synchronisieren können, müssen Sie zunächst die Marketo-Lösung in Dynamics installieren.

>[!NOTE]
>
>Nachdem Sie Marketo mit einem CRM synchronisiert haben, können Sie keine neue Synchronisierung durchführen, ohne die Instanz zu ersetzen.

>[!PREREQUISITES]
>
>Sie müssen [Bereitstellung im Internet](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) mit [Active Directory Federation-Dienste](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0, 2.1 oder 3.0 (ADFS) konfiguriert. Hinweis: Das IFD-Dokument wird beim Klicken auf den Link automatisch heruntergeladen.
>
>[Marketo-Lösung herunterladen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) bevor Sie beginnen.

>[!NOTE]
>
>**Dynamics-Administratorberechtigungen erforderlich.**
>
>Sie benötigen CRM-Administratorberechtigungen, um diese Synchronisierung durchzuführen.

1. Anmelden **Dynamics**. Klicken Sie auf **Microsoft Dynamics CRM** Dropdown-Menü und wählen Sie **Einstellungen**.

   ![](assets/image2014-12-11-10-3a39-3a41.png)

1. under **Einstellungen** auswählen **Lösungen**.

   ![](assets/image2014-12-11-10-3a39-3a51.png)

1. Klicks **Import**.

   ![](assets/image2015-3-26-9-3a52-3a10.png)

1. Klicks **Durchsuchen** und wählen Sie die [heruntergeladene Lösung](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Klicks **Nächste**.

   ![](assets/image2015-3-26-9-3a54-3a1.png)

1. Anzeigen der Lösungsinformationen und klicken Sie auf **Lösungspaketdetails anzeigen**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Wenn Sie alle Details überprüft haben, klicken Sie auf **Schließen**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Klicken Sie auf der Seite Lösungsinformationen auf **Nächste**.

   ![](assets/image2015-3-26-9-3a55-3a17.png)

1. Stellen Sie sicher, dass die SDK-Option aktiviert ist. Klicks **Import**.

   ![](assets/image2015-3-26-10-3a3-3a11.png)

1. Warten Sie, bis der Import abgeschlossen ist.

   >[!TIP]
   >
   >Sie müssen Popups in Ihrem Browser aktivieren, um den Installationsprozess abzuschließen.

   ![](assets/image2014-12-11-10-3a41-3a5.png)

1. Laden Sie eine Protokolldatei herunter (falls gewünscht) und klicken Sie auf **Schließen**.

   >[!NOTE]
   >
   >Möglicherweise wird eine Meldung mit der Meldung &quot;Marketo Lead Management wurde mit Warnung abgeschlossen&quot;angezeigt. Dies ist völlig zu erwarten.

   ![](assets/image2014-12-11-10-3a41-3a14.png)

1. Die Marketo-Lead-Verwaltung wird jetzt im **Alle Lösungen** Seite.

   ![](assets/image2015-3-26-10-3a1-3a21.png)

1. Wählen Sie die Marketo-Lösung aus und klicken Sie auf **Alle Anpassungen veröffentlichen**.

   ![](assets/image2014-12-11-10-3a41-3a32.png)

War nicht zu schlecht? Komm schon, ich werde dich durch den Rest führen.

>[!CAUTION]
>
>Die Deaktivierung eines der Marketo SDK Messaging-Prozesse führt zu einer fehlerhaften Installation!

>[!MORELIKETHIS]
>
>[Schritt 2 von 3: Konfigurieren der Synchronisierungsbenutzer für Marketo (On-Premises 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-configure-2013.md)
