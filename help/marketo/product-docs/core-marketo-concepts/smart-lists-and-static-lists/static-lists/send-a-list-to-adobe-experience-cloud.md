---
unique-page-id: 37356194
description: Liste an Adobe Experience Cloud senden - Marketo-Dokumente - Produktdokumentation
title: Liste an Adobe Experience Cloud senden
exl-id: 770eefe1-05f9-409d-8e7c-b3f1e6ba8139
feature: Static Lists
source-git-commit: c10ecc0ccad28f2e480343acefe10f5eca2ae578
workflow-type: tm+mt
source-wordcount: '784'
ht-degree: 1%

---

# Liste an Adobe Experience Cloud senden {#send-a-list-to-adobe-experience-cloud}

>[!NOTE]
>
>Eine HIPAA-fähige Bereitstellung einer Marketo Engage-Instanz kann diese Funktion nicht verwenden.

>[!PREREQUISITES]
>
>[Einrichten der Adobe-Organisationszuordnung](/help/marketo/product-docs/adobe-experience-cloud-integrations/set-up-adobe-organization-mapping.md){target="_blank"}

## Unterstützte Zielanwendungen {#supported-destination-applications}

* Adobe Advertising Cloud
* Adobe Analytics (_nur_ wenn Sie eine Adobe Audience Manager-Lizenz besitzen)
* Adobe Audience Manager
* Adobe Experience Manager
* Adobe Real-time Customer Data Platform
* Adobe Target

## So senden Sie eine statische Liste {#how-to-send-a-static-list}

Eine statische Liste ist genau das: statisch. In Adobe Experience Cloud werden keine Änderungen an der Liste vorgenommen, es sei denn, Sie nehmen diese manuell vor.

1. Suchen Sie in Marketo die Liste, die Sie exportieren möchten. Klicken Sie mit der rechten Maustaste darauf und wählen Sie **[!UICONTROL An Experience Cloud senden]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-1.png)

1. Audience Manager Klicken Sie auf die Dropdown-**&#x200B;** Zielordner und wählen Sie den gewünschten Zielordner auf der Experience Cloud aus.

   ![](assets/send-a-list-to-adobe-experience-cloud-2.png)

1. Wählen Sie aus, ob eine neue Audience erstellt oder eine vorhandene überschrieben werden soll (in diesem Beispiel erstellen wir eine neue Audience). Geben Sie den neuen Zielgruppennamen ein und klicken Sie auf **[!UICONTROL Senden]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-3.png)

1. Klicken Sie auf **[!UICONTROL OK]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-4.png)

   >[!NOTE]
   >
   >Es kann bis zu 6-8 Stunden dauern, bis die Zielgruppenzugehörigkeit vollständig im Adobe angegeben ist.

## Senden einer synchronisierten Liste {#how-to-send-a-synced-list}

Das Synchronisieren einer Liste bedeutet, dass jedes Mal, wenn Sie eine Liste in Marketo aktualisieren, alle Änderungen automatisch mit der zugehörigen Audience in Adobe Experience Cloud synchronisiert werden.

1. Suchen Sie in Marketo die Liste, die Sie exportieren möchten. Klicken Sie mit der rechten Maustaste darauf und wählen Sie **[!UICONTROL An Experience Cloud senden]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-5.png)

1. Klicken Sie auf **[!UICONTROL Zielgruppenbibliotheksordner]** und wählen Sie den gewünschten Zielordner auf der Experience Cloud aus.

   ![](assets/send-a-list-to-adobe-experience-cloud-6.png)

1. Wählen Sie aus, ob eine neue Audience erstellt oder eine vorhandene überschrieben werden soll (in diesem Beispiel erstellen wir eine neue Audience). Geben Sie den neuen Zielgruppennamen ein, aktivieren Sie das Kontrollkästchen **[!UICONTROL Zielgruppenmitgliedschaft synchron halten]** und klicken Sie auf **[!UICONTROL Senden]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-7.png)

1. Klicken Sie auf **OK**.

   ![](assets/send-a-list-to-adobe-experience-cloud-8.png)

## Anleitung zum Beenden der Listensynchronisierung {#how-to-stop-a-list-sync}

Sie können die Synchronisierung Ihrer Liste jederzeit beenden.

1. Suchen Sie in Marketo die Liste, deren Synchronisierung Sie beenden möchten, und klicken Sie mit der rechten Maustaste darauf. Klicken Sie **[!UICONTROL Listensynchronisierung anhalten]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-9.png)

1. Wählen Sie die Zielgruppe(n) aus, deren Synchronisierung beendet werden soll(en), und klicken Sie auf **[!UICONTROL Beenden]**.

   ![](assets/send-a-list-to-adobe-experience-cloud-10.png)

1. Klicken Sie **[!UICONTROL Beenden]** zur Bestätigung.

   ![](assets/send-a-list-to-adobe-experience-cloud-11.png)

## Zu beachtende Punkte {#things-to-note}

**Für Adobe Analytics freigeben**

* Kunden, die sowohl Adobe Audience Manager als auch Adobe Analytics besitzen, können durch diese Integration Zielgruppen aus Marketo für Ihre Adobe Analytics Report Suites freigeben. Es müssen jedoch einige zusätzliche Konfigurationsschritte in Adobe Audience Manager vorgenommen werden, um dies zu aktivieren. Weitere Informationen zum Einrichten finden Sie in [&#128279;](https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html){target="_blank"} Dokumentation zu Adobe Audience Manager.

* Wenn eine Liste leer ist oder keine Personen mit ECID-Werten hat, wird der Listenname nicht an einen externen Ort weitergeleitet, um außerhalb von Marketo Engage referenziert zu werden.

**Nutzung von Eigenschaften für Adobe Audience Manager-Kunden**

Wenn Sie einen Listenexport in Marketo starten, werden Sie die folgenden Änderungen in Ihrer Adobe Audience Manager-Instanz feststellen:

* Für alle Personen in der exportierten Liste schreibt Marketo eine Eigenschaft mit den gehashten E-Mails als geräteübergreifende Kennung. Der Name des Merkmals stimmt mit dem Namen der Ziel-Zielgruppe überein, den Sie beim Export angegeben haben.
* Für alle ECIDs, die Marketo den Personen in der exportierten Liste zuordnen konnte, schreibt Marketo eine Eigenschaft mit der ECID-Gerätekennung. Der Name des Merkmals stimmt mit dem Namen der Ziel-Zielgruppe überein, den Sie beim Export angegeben haben.
* Marketo Audience Manager erstellt auch ein Segment in Ihrer Segmentinstanz und verwendet dabei das ECID-Merkmal als einziges Segmentierungskriterium. Der Name des Segments entspricht dem Ziel-Zielgruppennamen, den Sie beim Export angegeben haben.

## FAQs {#faq}

**Warum unterscheidet sich die Listengröße in Marketo von der in Adobe?**

Im Hintergrund funktioniert die Zielgruppenintegration durch die Synchronisierung von Marketo Munchkin-Cookies mit dem entsprechenden Adobe-ECID-Cookie. Marketo kann Mitgliedschaftsdaten nur für Personen freigeben, für die Marketo eine ECID synchronisiert hat. Um die bestmöglichen Ergebnisse zu erzielen, wird empfohlen, das Tracking-Skript munchkin.js von Marketo parallel zum Trackingcode Adobe visitor.js auf allen Seiten zu laden, die für Marketingzwecke verfolgt werden sollen.

**Wie funktioniert die Cookie-Synchronisierung?**

Wenn die Cookie-Synchronisierung für Ihr Marketo-Abonnement aktiviert ist, versucht munchkin.js von Marketo, Adobe-ECIDs für die Adobe IMS-Organisation zu erfassen und zu speichern, die Sie während der Einrichtung der Integration angegeben haben, und diese ECIDs mit der entsprechenden Marketo-Cookie-Kennung abzugleichen. Dadurch können die anonymen Benutzerprofile von Marketo mit Adobe-ECIDs angereichert werden.

Ein weiterer Schritt ist erforderlich, um das anonyme Benutzerprofil mit einem Personenprofil zu verknüpfen, das mithilfe einer Nur-Text-E-Mail identifiziert wird. Wie das genau funktioniert, [ hier beschrieben](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md){target="_blank"}.

**Welche Informationen werden freigegeben?**

Diese Integration gibt nur Informationen zur Listenmitgliedschaft von Marketo an Adobe weiter (z. B. das Wissen, dass Person X Mitglied von Liste Y ist). Über diese Integration werden keine zusätzlichen Personenattribute für Adobe freigegeben.
