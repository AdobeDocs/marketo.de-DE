---
unique-page-id: 7504736
description: Installieren Sie Marketo für Dynamics 2015 On-Prem und 2016 365 On-Prem Schritt 1 von 3 - Marketing Docs - Produktdokumentation
title: Installieren Sie Marketo für Dynamics 2015 On-Prem und 2016 365 On-Prem Schritt 1 von 3
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---


# Schritt 1 von 3: Konfigurieren des Synchronisierungsbenutzers für Marketo (On-Prem 2015 und 2016 365 On-Prem) {#step-of-configure-sync-user-for-marketo-on-premises-and-365}

Bevor Sie Microsoft Dynamics 2015 On-Premises oder 2016 (Dynamics 365) mit Marketo synchronisieren können, müssen Sie zunächst die Marketo-Lösung in Dynamics installieren.

>[!NOTE]
>
>Nachdem Sie Marketo mit einem CRM synchronisiert haben, können Sie kein neues CRM mit der vorhandenen Marketo-Instanz synchronisieren.

>[!PREREQUISITES]
>
>Wenn Sie Microsoft Dynamics On-Premise verwenden, müssen Sie [Internet Facing Deployment](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) mit [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0+ (ADFS) konfiguriert haben. Hinweis: Das IFD-Dokument wird automatisch heruntergeladen, wenn Sie auf den Link klicken.
>
>[Laden Sie die Marketing Lead Management ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) Solution vor dem Beginn herunter.

>[!NOTE]
>
>**Dynamics-Administratorberechtigungen erforderlich.**
>
>Sie benötigen CRM-Administratorrechte, um diese Synchronisierung durchzuführen.

1. Melden Sie sich bei **Dynamics an.** Klicken Sie auf das  **Microsoft Dynamics** CRM-Dropdownmenü und wählen Sie  **Einstellungen**.

   ![](assets/image2015-3-19-8-33-29.png)

1. Wählen Sie unter **Einstellungen** **Lösungen**.

   ![](assets/image2015-3-19-8-33-3.png)

1. Klicken Sie auf **Import**.

   ![](assets/image2015-3-19-8-34-8.png)

1. Klicken Sie auf **Durchsuchen** und wählen Sie die Lösung aus, die Sie [heruntergeladen haben. ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) Klicken Sie auf **Weiter**.

   ![](assets/image2015-3-19-9-20-56.png)

1. Ansicht Sie die Lösungsinformationen und klicken Sie auf **Ansicht Solution Package details**.

   ![](assets/image2015-11-18-11-12-8.png)

1. Wenn Sie alle Details überprüft haben, klicken Sie auf **Schließen**.

   ![](assets/step6.png)

1. Klicken Sie auf der Seite &quot;Lösungsinformationen&quot;auf **Weiter**.

   ![](assets/image2015-3-19-9-21-50.png)

1. Stellen Sie sicher, dass das Kontrollkästchen SDK-Option aktiviert ist. Klicken Sie auf **Import**.

   ![](assets/image2015-3-19-9-19-12.png)

1. Warten Sie, bis der Import abgeschlossen ist.

   >[!TIP]
   >
   >Sie müssen Popups in Ihrem Browser aktivieren, um den Installationsprozess abzuschließen.

   ![](assets/image2015-3-11-11-34-9.png)

1. Laden Sie eine Protokolldatei herunter (falls gewünscht) und klicken Sie auf **Schließen**.

   >[!NOTE]
   >
   >Sie sehen möglicherweise eine Meldung mit der Meldung &quot;Marketing-Lead-Management abgeschlossen mit Warnung&quot;. Das ist völlig zu erwarten.

   ![](assets/image2015-3-13-9-54-39.png)

1. Die Marketing-Interessentenverwaltung wird nun auf der Seite **Alle Lösungen** angezeigt.

   ![](assets/image2015-3-19-8-40-38.png)

1. Wählen Sie die Marketing-Lösung aus und klicken Sie auf **Alle Anpassungen veröffentlichen**.

   ![](assets/image2015-3-19-8-41-21.png)

   Hoch fünf! Die Installation ist abgeschlossen.

   >[!CAUTION]
   >
   >Die Deaktivierung eines der Marketing SDK Messaging-Prozesse führt zu einer fehlerhaften Installation!

   >[!MORELIKETHIS]
   >
   >[Installieren Sie Marketo für Dynamics 2015 On-Prem und 2016 365 On-Prem Schritt 2 von 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2015-on-premises-2016-dynamics-365-on-premises/step-2-of-3-set-up.md)
