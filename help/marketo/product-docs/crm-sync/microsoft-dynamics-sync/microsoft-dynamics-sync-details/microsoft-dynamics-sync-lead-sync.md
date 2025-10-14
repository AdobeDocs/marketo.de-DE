---
unique-page-id: 3571848
description: Microsoft Dynamics-Synchronisierung - Lead-Synchronisierung - Marketo-Dokumente - Produktdokumentation
title: Microsoft Dynamics-Synchronisierung - Lead-Synchronisierung
exl-id: ea04a039-32f7-41f9-85fb-18df8e236390
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics]: Lead-Synchronisation {#microsoft-dynamics-sync-lead-sync}

Die Synchronisierung von Marketo zu [!DNL Dynamics] ist extrem leistungsstark. Im Folgenden finden Sie die Details:

## Wie werden die Details zwischen den beiden Systemen synchron gehalten? {#how-are-details-kept-in-sync-between-the-two-systems}

Die Synchronisation erfolgt bidirektional. Wenn Sie Änderungen an einem Lead in [!DNL Dynamics] oder an einer Person in Marketo vornehmen, wird Ihre Aktualisierung auf beiden Systemen angezeigt.

>[!NOTE]
>
>Löschvorgänge werden nicht immer automatisch in beide Richtungen synchronisiert. Siehe [Löschen von Leads oder Kontakten](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/deleting-a-lead-or-contact.md){target="_blank"}.

## Was passiert, wenn Änderungen am selben Feld in beiden Systemen gleichzeitig vorgenommen werden? (Datenkollision) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Obwohl dies selten ist, wird Marketo für Personen (Leads) und [!DNL Dynamics] für Kontakte gewinnen. Der Grund dafür ist, dass wir die Marketing-Abteilung für die Menschen als verbindlich betrachten, während das offizielle System der Aufzeichnung für Kontakte in der Verkaufs- (CRM)-Abteilung ist.

## Kann ich mit Marketo einen Lead in [!DNL Dynamics] erstellen? {#can-i-create-a-lead-in-dynamics-using-marketo}

Ja, die [[!UICONTROL Person mit Microsoft synchronisieren]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) verwenden. Dadurch wird ein Lead in [!DNL Dynamics] erstellt, wenn der Lead nicht vorhanden ist. Wenn der Lead vorhanden ist, führt der Flussschritt keine Aktion durch.

>[!NOTE]
>
>Bei Verwendung der Flussaktion [!UICONTROL Person mit Microsoft synchronisieren] (nur in einer Trigger-Kampagne) wird der Lead/Kontakt in Echtzeit in [!DNL Dynamics] erstellt.

## Kann ich die Synchronisierung einer Person aus Marketo mit einem Lead in [!DNL Dynamics] manuell erzwingen? {#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

Nein, die automatische Hintergrundsynchronisierung ist die einzige Möglichkeit, Aktualisierungen zwischen Marketo und [!DNL Dynamics] zu synchronisieren. Die [[!UICONTROL Person mit Microsoft synchronisieren]](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) Flussaktion erzwingt keine Synchronisierung des Leads.

## Welche Felder werden mit Marketo synchronisiert? {#what-fields-will-sync-to-marketo}

Sie können [&#x200B; Setup Felder auswählen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} die synchronisiert werden sollen.

## Wird Marketo die [!DNL Dynamics] Validierungsregeln einhalten? {#will-marketo-respect-the-dynamics-validation-rules}

Ja. Die Synchronisierung schlägt fehl, wenn das Datenformat falsch ist oder erforderliche Feldinformationen fehlen. In diesem Fall protokolliert Marketo das Ergebnis im Aktivitätsprotokoll der Person.
