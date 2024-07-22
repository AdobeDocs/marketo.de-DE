---
unique-page-id: 3571848
description: Microsoft Dynamics Sync - Lead Sync - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync - Lead Sync
exl-id: ea04a039-32f7-41f9-85fb-18df8e236390
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Microsoft Dynamics Sync: Lead Sync {#microsoft-dynamics-sync-lead-sync}

Marketo Engage to Dynamics Synchronisation ist super leistungsstark. Hier sind die Details.

## Wie werden die Details zwischen den beiden Systemen synchronisiert? {#how-are-details-kept-in-sync-between-the-two-systems}

Die Synchronisation erfolgt bidirektional. Wenn Sie Änderungen an einem Lead in Dynamics oder einer Person in Marketo vornehmen, wird Ihre Aktualisierung in beiden Systemen übernommen.

>[!NOTE]
>
>Löschvorgänge werden nicht immer automatisch in beide Richtungen synchronisiert. Siehe [Löschen eines Leads oder Kontakts](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/deleting-a-lead-or-contact.md){target="_blank"}.

## Was passiert, wenn in beiden Systemen gleichzeitig Änderungen an demselben Feld vorgenommen werden? (Datenkollision) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Obwohl dies selten vorkommt, gewinnt Marketo für Personen (Leads) und Dynamics gewinnt für Kontakte. Dies liegt daran, dass wir die Marketing-Abteilung für Menschen als maßgeblich betrachten, während das offizielle System der Kontaktaufnahme in der Vertriebs- (CRM-) Abteilung ist.

## Kann ich mit Marketo einen Lead in Dynamics erstellen? {#can-i-create-a-lead-in-dynamics-using-marketo}

Ja, verwenden Sie die Flussaktion &quot;[Person mit Microsoft synchronisieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md){target="_blank"}&quot;. Dadurch wird ein Lead in Dynamics erstellt, wenn der Lead nicht vorhanden ist. Wenn der Lead vorhanden ist, führt der Flussschritt keine Aktion durch.

>[!NOTE]
>
>Bei Verwendung der FlusAktion &quot;Person mit Microsoft synchronisieren&quot;(nur in einer Trigger-Kampagne) wird der Lead/Kontakt in Echtzeit in Dynamics erstellt.

## Kann ich in Dynamics manuell die Synchronisierung einer Person von Marketo mit einem Lead erzwingen? {#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

Nein, die automatisierte Hintergrundsynchronisierung ist die einzige Möglichkeit, Updates zwischen Marketo und Dynamics zu synchronisieren. Die Durchlaufaktion [Person mit Microsoft synchronisieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md){target="_blank"} erzwingt keine Synchronisierung des Leads.

## Welche Felder werden mit Marketo synchronisiert? {#what-fields-will-sync-to-marketo}

Sie können [ Felder auswählen, die während der Einrichtung synchronisiert werden sollen.](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"}

## Wird Marketo die Dynamics-Validierungsregeln einhalten? {#will-marketo-respect-the-dynamics-validation-rules}

Ja. Die Synchronisierung schlägt fehl, wenn das Datenformat falsch ist oder die erforderlichen Feldinformationen fehlen. In diesem Fall protokolliert Marketo das Ergebnis im Aktivitätsprotokoll der Person.
