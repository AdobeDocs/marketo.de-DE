---
description: Zielgruppe aus Adobe Experience Cloud synchronisieren - Marketo-Dokumente - Produktdokumentation
title: Zielgruppe aus Adobe Experience Cloud synchronisieren
exl-id: 2288ee01-2c2e-4f33-b5c9-da3a431c1816
feature: Integrations
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 0%

---

# Zielgruppe aus Adobe Experience Cloud synchronisieren {#sync-an-audience-from-adobe-experience-cloud}

>[!NOTE]
>
>Eine HIPAA-bereite Bereitstellung einer Marketo-Instanz kann diese Integration nicht verwenden.

>[!PREREQUISITES]
>
>[Einrichten der Adobe-Organisationszuordnung](/help/marketo/product-docs/adobe-experience-cloud-integrations/set-up-adobe-organization-mapping.md){target="_blank"}

## Synchronisieren von Zielgruppen {#how-to-sync-an-audience}

1. Klicken Sie in My Marketo auf die Kachel **[!UICONTROL Database]** .

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. Klicken Sie auf das Dropdown-Menü **[!UICONTROL Neu]** und wählen Sie **[!UICONTROL Aus Experience Cloud-Audience synchronisieren]** aus.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. Klicken Sie auf die Dropdownliste **[!UICONTROL Zielgruppenbibliotheksordner]** und wählen Sie den gewünschten Herkunftsordner aus.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. Wählen Sie einen **[!UICONTROL Zielgruppennamen]** aus.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. Für das Ziel können Sie eine vorhandene Liste auswählen oder den Namen einer neuen eingeben. In diesem Beispiel erstellen wir ein neues. Klicken Sie abschließend auf **[!UICONTROL Synchronisieren]** .

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. Klicken Sie auf **[!UICONTROL OK]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## FAQs {#faq}

**Wie funktioniert die Cookie-Synchronisierung?**

Wenn die Cookie-Synchronisierung für Ihr Marketo-Abonnement aktiviert ist, versucht die Marketo-Datei munchkin.js, Adobe-ECIDs für die Adobe IMS-Organisation zu erfassen und zu speichern, die Sie während der Integrationseinrichtung angegeben haben, und diese ECIDs mit der entsprechenden Marketo-Cookie-ID abzugleichen. Dadurch können anonyme Benutzerprofile von Marketo mit Adobe ECIDs angereichert werden.

Ein weiterer Schritt ist erforderlich, um das anonyme Benutzerprofil einem Lead-Profil zuzuordnen, das mithilfe einer Text-E-Mail identifiziert wird. Die genaue Funktionsweise von [wird hier ](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md){target="_blank"} beschrieben.

**Warum unterscheidet sich die Listengröße in Marketo von der in Adobe?**

Eine Person wird auch nicht synchronisiert, wenn wir eine ECID-Cookie-ID nicht mit einer bekannten Person in Marketo verknüpfen können.

**Ist dies eine einmalige Synchronisation?**

Sie müssen die Synchronisierung nur einmal starten. Danach werden Datensätze automatisch synchronisiert. Die anfängliche Synchronisation kann bis zu 24 Stunden dauern. In Zukunft werden neue Datensätze in 2-3 Stunden synchronisiert.
