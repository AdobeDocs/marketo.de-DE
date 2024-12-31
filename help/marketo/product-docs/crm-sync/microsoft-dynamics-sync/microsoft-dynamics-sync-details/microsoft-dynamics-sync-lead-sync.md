---
unique-page-id: 3571848
description: Microsoft Dynamics-Synchronisierung - Lead-Synchronisierung - Marketo-Dokumente - Produktdokumentation
title: Microsoft Dynamics-Synchronisierung - Lead-Synchronisierung
exl-id: ea04a039-32f7-41f9-85fb-18df8e236390
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Microsoft Dynamics-Synchronisierung: Lead-Synchronisierung {#microsoft-dynamics-sync-lead-sync}

Marketo Engage zu Dynamics Sync ist super leistungsstark. Im Folgenden finden Sie die Details.

## Wie werden die Details zwischen den beiden Systemen synchron gehalten? {#how-are-details-kept-in-sync-between-the-two-systems}

Die Synchronisation erfolgt bidirektional. Wenn Sie Änderungen an einem Lead in Dynamics oder an einer Person in Marketo vornehmen, wird die Aktualisierung auf beiden Systemen angezeigt.

>[!NOTE]
>
>Löschvorgänge werden nicht immer automatisch in beide Richtungen synchronisiert. Siehe [Löschen von Leads oder Kontakten](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/deleting-a-lead-or-contact.md){target="_blank"}.

## Was passiert, wenn Änderungen am selben Feld in beiden Systemen gleichzeitig vorgenommen werden? (Datenkollision) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Obwohl dies selten ist, wird Marketo für Personen (Leads) und Dynamics für Kontakte gewinnen. Der Grund dafür ist, dass wir die Marketing-Abteilung für die Menschen als verbindlich betrachten, während das offizielle System der Aufzeichnung für Kontakte in der Verkaufs- (CRM)-Abteilung ist.

## Kann ich mit Marketo einen Lead in Dynamics erstellen? {#can-i-create-a-lead-in-dynamics-using-marketo}

Ja, die [Person mit Microsoft synchronisieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md){target="_blank"} verwenden. Dadurch wird ein Lead in Dynamics erstellt, wenn der Lead nicht vorhanden ist. Wenn der Lead vorhanden ist, führt der Flussschritt keine Aktion durch.

>[!NOTE]
>
>Bei Verwendung der Flussaktion „Person mit Microsoft synchronisieren“ (nur in einer Trigger-Kampagne) wird der Lead/Kontakt in Echtzeit in Dynamics erstellt.

## Kann ich in Dynamics manuell eine Synchronisierung einer Person aus Marketo mit einem Lead erzwingen? {#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

Nein, die automatische Hintergrundsynchronisierung ist die einzige Möglichkeit, Aktualisierungen zwischen Marketo und Dynamics zu synchronisieren. Die [Person mit Microsoft synchronisieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md){target="_blank"} Flussaktion erzwingt keine Synchronisierung des Leads.

## Welche Felder werden mit Marketo synchronisiert? {#what-fields-will-sync-to-marketo}

Sie können [ Setup Felder auswählen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} die synchronisiert werden sollen.

## Hält Marketo die Dynamics-Validierungsregeln ein? {#will-marketo-respect-the-dynamics-validation-rules}

Ja. Die Synchronisierung schlägt fehl, wenn das Datenformat falsch ist oder erforderliche Feldinformationen fehlen. In diesem Fall protokolliert Marketo das Ergebnis im Aktivitätsprotokoll der Person.
