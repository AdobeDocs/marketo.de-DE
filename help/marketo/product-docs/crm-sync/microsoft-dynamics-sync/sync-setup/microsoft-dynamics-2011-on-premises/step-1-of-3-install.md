---
unique-page-id: 3571805
description: Schritt 1 von 3 - Installieren der Marketing Solution (On-Premises 2011) - Marketing Docs - Produktdokumentation
title: Schritt 1 von 3 - Installieren der Marketing Solution (On-Premises 2011)
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---


# Schritt 1 von 3: Installieren Sie die Marketing Solution (On-Premises 2011) {#step-of-install-the-marketo-solution-on-premises}

Bevor Sie Microsoft Dynamics On-Premises und Marketo synchronisieren können, müssen Sie zunächst die Marketo-Lösung in Dynamics installieren.

>[!NOTE]
>
>Nach der Synchronisierung von Marketo mit einem CRM können Sie keine neue Synchronisierung durchführen, ohne die Instanz zu ersetzen.

>[!NOTE]
>
>**Voraussetzungen**
>
>Sie müssen über eine [Internet Facing Deployment](http://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) mit [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0, 2.1 oder 3.0 (ADFS) verfügen. **Hinweis**: Das IFD-Dokument wird automatisch heruntergeladen, wenn Sie auf den Link klicken.
>
>[Laden Sie die Marketing Lead Management Solution](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) vor dem Beginn herunter.

>[!NOTE]
>
>**Dynamics-Administratorberechtigungen erforderlich.**
>
>Sie benötigen CRM-Administratorrechte, um diese Synchronisierung durchzuführen.

1. Melden Sie sich bei **Dynamics** an und wählen Sie im Menü unten links die Option **Einstellungen** .

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. Wählen Sie in der Struktur **Lösungen** aus.

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. Klicken Sie auf **Importieren**.

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. Klicken Sie auf **Durchsuchen**. Wählen Sie die von Ihnen [heruntergeladene](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)Marketing Lead Management-Lösung aus. Klicken Sie auf **Weiter**.

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. Ansicht der Lösungsinformationen und klicken Sie auf Details zum **Ansicht-Lösungspaket**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Wenn Sie alle Details überprüft haben, klicken Sie auf **Schließen**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Klicken Sie auf der Seite &quot;Lösungsinformationen&quot;auf **Weiter**.

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. Vergewissern Sie sich, dass das Kontrollkästchen für die SDK-Meldung aktiviert ist. Klicken Sie auf **Weiter**.

   ![](assets/image2015-4-2-11-3a42-3a37.png)

   >[!TIP]
   >
   >Sie müssen Popups in Ihrem Browser aktivieren, um den Installationsprozess abzuschließen.

1. Warten Sie jetzt, bis der Import abgeschlossen ist. Stehe auf und mach einige Stretches.

   ![](assets/image2015-4-2-11-3a43-3a51.png)

1. Klicken Sie auf **Schließen**.

   >[!NOTE]
   >
   >Sie sehen möglicherweise eine Meldung mit der Meldung &quot;Marketing-Lead-Management abgeschlossen mit Warnung&quot;. Das ist völlig zu erwarten.

   ![](assets/image2015-4-2-11-3a44-3a44.png)

1. Die Marketing-Interessentenverwaltung wird jetzt auf der Seite **Alle Lösungen** angezeigt.

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. Wählen Sie Marketing-to-Interessentenverwaltung und klicken Sie auf Alle Anpassungen **veröffentlichen.**

   ![](assets/image2015-4-2-11-3a48-3a21.png)

War das nicht zu schlecht? Los, ich werde dich durch den Rest führen.

>[!CAUTION]
>
>Die Deaktivierung eines der Marketing SDK Messaging-Prozesse führt zu einer fehlerhaften Installation!

>[!NOTE]
>
>**Verwandte Artikel**
>
>[Schritt 2 von 3: Einrichten von Marketo Sync User in Dynamics (On-Premises 2011)](step-2-of-3-set-up.md)
