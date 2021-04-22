---
description: Synchronisieren einer Audience von Adobe Experience Cloud - Marketo Docs - Produktdokumentation
title: Synchronisieren einer Audience von Adobe Experience Cloud
exl-id: 2288ee01-2c2e-4f33-b5c9-da3a431c1816
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---

# Synchronisieren einer Audience von Adobe Experience Cloud {#sync-an-audience-from-adobe-experience-cloud}

>[!NOTE]
>
>Eine HIPAA-bereite Bereitstellung einer Marketo-Instanz kann diese Integration nicht verwenden.

>[!PREREQUISITES]
>
>[Einrichten der Freigabe von Adobe Experience Cloud-Audiencen](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/set-up-adobe-experience-cloud-audience-sharing.md)

## Synchronisieren einer Audience {#how-to-sync-an-audience}

1. Klicken Sie in My Marketo auf die Kachel **Database**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. Klicken Sie auf die Dropdownliste **Neu** und wählen Sie **Von Experience Cloud-Audience synchronisieren**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. Klicken Sie auf die Dropdownliste **Audience-Bibliotheksordner** und wählen Sie den gewünschten Herkünfte-Ordner aus.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. Wählen Sie einen **Audiencen-Namen**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. Für das Ziel können Sie eine vorhandene Liste auswählen oder den Namen einer neuen eingeben. In diesem Beispiel erstellen wir ein neues. Klicken Sie abschließend auf **Synchronisieren**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. Klicken Sie auf **OK**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## FAQ {#faq}

**Wie funktioniert die Cookie-Synchronisierung?**

Wenn die Cookie-Synchronisierung für Ihr Marketo-Abonnement aktiviert ist, versucht Marketo&#39;s munchkin.js, ECIDs der Adobe für die Adobe IMS Org zu erfassen und zu speichern, die Sie bei der Integrationseinrichtung angegeben haben, und diese ECIDs mit der entsprechenden Marketo-Cookie-ID abzustimmen. Dadurch können die anonymen Marketo-Profil mit Adobe-ECIDs bereichert werden.

Ein weiterer Schritt ist erforderlich, um das anonyme Benutzerkonto mit einem Lead-Profil zu verknüpfen, das mit einer E-Mail-Adresse ohne Text identifiziert wird. Wie genau dies funktioniert [wird hier beschrieben.](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md)

**Warum unterscheidet sich die Liste in Marketo von der in der Adobe?**

Eine Person wird auch nicht synchronisiert, wenn es nicht möglich ist, eine ECID-Cookie-ID mit einer bekannten Person in Marketo zu verknüpfen.

**Ist das eine einmalige Synchronisierung?**

Sie müssen die Synchronisierung nur einmal starten. Danach werden die Datensätze automatisch synchronisiert. Die anfängliche Synchronisierung kann bis zu 24 Stunden dauern. In Zukunft werden neue Datensätze in 2-3 Stunden synchronisiert.
