---
description: Synchronisieren einer Zielgruppe aus Adobe Experience Cloud - Marketo-Dokumente - Produktdokumentation
title: Synchronisieren einer Zielgruppe aus Adobe Experience Cloud
exl-id: 2288ee01-2c2e-4f33-b5c9-da3a431c1816
feature: Integrations
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 1%

---

# Synchronisieren einer Zielgruppe aus Adobe Experience Cloud {#sync-an-audience-from-adobe-experience-cloud}

>[!NOTE]
>
>Eine HIPAA-fähige Bereitstellung einer Marketo-Instanz kann diese Integration nicht verwenden.

>[!PREREQUISITES]
>
>[Einrichten der Adobe-Organisationszuordnung](/help/marketo/product-docs/adobe-experience-cloud-integrations/set-up-adobe-organization-mapping.md){target="_blank"}

## So synchronisieren Sie eine Zielgruppe {#how-to-sync-an-audience}

1. Klicken Sie in My Marketo auf die Kachel **[!UICONTROL Datenbank]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. Klicken Sie auf **[!UICONTROL Neu]** und wählen Sie **[!UICONTROL Von Experience Cloud-Zielgruppe synchronisieren]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. Klicken Sie auf **[!UICONTROL Zielgruppenbibliotheksordner]** und wählen Sie den gewünschten Ursprungsordner aus.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. Wählen Sie einen **[!UICONTROL Zielgruppennamen]** aus.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. Für das Ziel können Sie eine vorhandene Liste auswählen oder den Namen einer neuen Liste eingeben. In diesem Beispiel erstellen wir ein neues. Klicken Sie **[!UICONTROL auf]** Synchronisieren“.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. Klicken Sie auf **[!UICONTROL OK]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## FAQs {#faq}

**Wie funktioniert die Cookie-Synchronisierung?**

Wenn die Cookie-Synchronisierung für Ihr Marketo-Abonnement aktiviert ist, versucht munchkin.js von Marketo, Adobe-ECIDs für die Adobe IMS-Organisation zu erfassen und zu speichern, die Sie während der Einrichtung der Integration angegeben haben, und diese ECIDs mit der entsprechenden Marketo-Cookie-Kennung abzugleichen. Dadurch können die anonymen Benutzerprofile von Marketo mit Adobe-ECIDs angereichert werden.

Ein weiterer Schritt ist erforderlich, um das anonyme Benutzerprofil mit einem Lead-Profil zu verknüpfen, das mithilfe einer Nur-Text-E-Mail identifiziert wird. Wie das genau funktioniert [wird hier beschrieben](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md){target="_blank"}.

**Warum unterscheidet sich die Listengröße in Marketo von der in Adobe?**

Eine Person wird auch nicht synchronisiert, wenn wir eine ECID-Cookie-ID nicht an eine bekannte Person in Marketo binden können.

**Handelt es sich um eine einmalige Synchronisation?**

Sie müssen die Synchronisierung nur einmal starten. Danach werden die Datensätze automatisch synchronisiert. Die Erstsynchronisierung kann bis zu 24 Stunden dauern. Ab sofort werden neue Datensätze in 2-3 Stunden synchronisiert.
