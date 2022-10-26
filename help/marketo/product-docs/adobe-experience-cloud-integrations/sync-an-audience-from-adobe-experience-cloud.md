---
description: Zielgruppe aus Adobe Experience Cloud synchronisieren - Marketo-Dokumente - Produktdokumentation
title: Zielgruppe aus Adobe Experience Cloud synchronisieren
exl-id: 2288ee01-2c2e-4f33-b5c9-da3a431c1816
source-git-commit: 492f21f090dc2478271172cf7db470e16f202366
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# Zielgruppe aus Adobe Experience Cloud synchronisieren {#sync-an-audience-from-adobe-experience-cloud}

>[!NOTE]
>
>Eine HIPAA-bereite Bereitstellung einer Marketo-Instanz kann diese Integration nicht verwenden.

>[!PREREQUISITES]
>
>[Einrichten der Adobe-Organisationszuordnung](/help/marketo/product-docs/adobe-experience-cloud-integrations/set-up-adobe-organization-mapping.md){target=&quot;_blank&quot;}

## Synchronisieren von Zielgruppen {#how-to-sync-an-audience}

1. Klicken Sie in My Marketo auf die **Datenbank** Kachel.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. Klicken Sie auf **Neu** und wählen Sie **Aus Experience Cloud-Zielgruppe synchronisieren**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. Klicken Sie auf **Zielgruppenbibliotheksordner** und wählen Sie den gewünschten Herkunftsordner aus.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. Wählen Sie eine **Zielgruppenname**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. Für das Ziel können Sie eine vorhandene Liste auswählen oder den Namen einer neuen eingeben. In diesem Beispiel erstellen wir ein neues. Klicken **Synchronisieren** wann geschehen.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. Klicken **OK**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## FAQs {#faq}

**Wie funktioniert die Cookie-Synchronisierung?**

Wenn die Cookie-Synchronisierung für Ihr Marketo-Abonnement aktiviert ist, versucht die Marketo-Datei munchkin.js, ECIDs der Adobe für die Adobe IMS-Organisation zu erfassen und zu speichern, die Sie bei der Integrationseinrichtung angegeben haben, und diese ECIDs mit der entsprechenden Marketo-Cookie-ID abzugleichen. Dadurch können anonyme Marketo-Benutzerprofile mit Adobe ECIDs angereichert werden.

Ein weiterer Schritt ist erforderlich, um das anonyme Benutzerprofil einem Lead-Profil zuzuordnen, das mithilfe einer Text-E-Mail identifiziert wird. Genau wie dies funktioniert [wird hier beschrieben](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md){target=&quot;_blank&quot;}.

**Warum unterscheidet sich die Listengröße in Marketo von der in Adobe?**

Eine Person wird auch nicht synchronisiert, wenn wir eine ECID-Cookie-ID nicht mit einer bekannten Person in Marketo verknüpfen können.

**Ist dies eine einmalige Synchronisation?**

Sie müssen die Synchronisierung nur einmal starten. Danach werden Datensätze automatisch synchronisiert. Die anfängliche Synchronisation kann bis zu 24 Stunden dauern. In Zukunft werden neue Datensätze in 2-3 Stunden synchronisiert.
