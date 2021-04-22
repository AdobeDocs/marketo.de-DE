---
unique-page-id: 3571822
description: Schritt 1 von 3 - Installieren der Marketo-Lösung (Online) - Marketo Docs - Produktdokumentation
title: Schritt 1 von 3 - Installieren der Marketo-Lösung (Online)
exl-id: 593fc014-db38-42cc-8f9f-0dd8307751e8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---

# Schritt 1 von 3: Installieren Sie die Marketo-Lösung (Online) {#step-of-install-the-marketo-solution-online}

Bevor Sie Microsoft Dynamics 365 und Marketo synchronisieren können, müssen Sie zunächst die Marketo-Lösung in Dynamics installieren. **Dynamics-Administratorberechtigungen sind erforderlich.**

>[!CAUTION]
>
>* Aktivieren Sie keine benutzerdefinierte Entitätssynchronisierung, bevor die erste Synchronisierung abgeschlossen ist. Sie werden per E-Mail benachrichtigt, sobald die Synchronisierung abgeschlossen ist.
>* Wenn Multi-Factor Authentication (MFA) für die Dynamiksynchronisierung aktiviert ist, müssen Sie diese deaktivieren, damit Dynamics mit Marketo ordnungsgemäß synchronisiert werden kann. Weitere Informationen erhalten Sie beim [Marketo Support](https://nation.marketo.com/t5/Support/ct-p/Support).


>[!NOTE]
>
>Nach der Synchronisierung von Marketo mit einem CRM können Sie keine neue Synchronisierung durchführen, ohne die Instanz zu ersetzen.

>[!PREREQUISITES]
>
>[Marketo Lead Management Solution herunterladen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)

1. Melden Sie sich bei **[Microsoft Office 365](https://login.microsoftonline.com/)** an.

   ![](assets/image2015-3-16-15-3a58-3a55.png)

1. Klicken Sie auf das Menü ![](assets/image2015-3-16-16-3a1-3a13.png) und wählen Sie **CRM**.

   ![](assets/image2015-3-16-16-3a0-3a10.png)

1. Klicken Sie auf das Menü ![](assets/image2015-5-13-10-3a5-3a8.png). Wählen Sie im Dropdown-Menü **Einstellungen** und dann **Lösungen**.

   ![](assets/image2015-5-13-10-3a4-3a1.png)

1. Klicken Sie auf **Import.**

   ![](assets/image2015-3-19-8-3a34-3a8.png)

1. Klicken Sie auf **Datei auswählen.** Wählen Sie die von Ihnen  [heruntergeladene](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) Marketo Lead Management-Lösung aus. Klicken Sie auf **Weiter**.

   ![](assets/image2015-10-9-14-3a44-3a14.png)

1. Ansicht Sie die Lösungsinformationen und klicken Sie auf **Ansicht Solution Package details**.

   ![](assets/image2015-10-9-15-3a4-3a16.png)

1. Wenn Sie alle Details überprüft haben, klicken Sie auf **Schließen**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Klicken Sie nun auf der Seite &quot;Lösungsinformationen&quot;auf **Weiter**.

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. Stellen Sie sicher, dass das Kontrollkästchen SDK-Option aktiviert ist. Klicken Sie auf **Import**.

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >Sie müssen Popups in Ihrem Browser aktivieren, um den Installationsprozess abzuschließen.

1. Warten Sie jetzt, bis der Import abgeschlossen ist. Stehe auf und mach einige Stretches.

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. Klicken Sie auf **Schließen.**

   >[!NOTE]
   >
   >Es wird möglicherweise eine Meldung angezeigt, in der steht: &quot;Marketo Lead Management wurde mit Warnung abgeschlossen&quot;. Das ist völlig zu erwarten.

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. Marketo Lead Management wird nun in der Liste der Lösungen angezeigt.

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. Wählen Sie **Marketo Lead Management** und klicken Sie auf **Alle Anpassungen veröffentlichen.**

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   Hoch fünf! Die Installation ist abgeschlossen.

   >[!MORELIKETHIS]
   >
   >[Schritt 2 von 3: Marketo Sync User in Dynamics einrichten](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md)
