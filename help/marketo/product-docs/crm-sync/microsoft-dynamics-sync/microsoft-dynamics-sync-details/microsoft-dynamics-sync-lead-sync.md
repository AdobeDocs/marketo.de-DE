---
unique-page-id: 3571848
description: Microsoft Dynamics Sync - Lead Sync - Marketing Docs - Produktdokumentation
title: Microsoft Dynamics Sync - Lead Sync
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Interessentensynchronisierung {#microsoft-dynamics-sync-lead-sync}

Marketo to to Dynamics sync ist super leistungsfähig. Im Folgenden finden Sie die Details:

## Wie werden die Details zwischen den beiden Systemen synchronisiert? {#how-are-details-kept-in-sync-between-the-two-systems}

Die Synchronisierung erfolgt bidirektional. Wenn Sie Änderungen an einem Lead in Dynamics oder einer Person in Marketo vornehmen, wird Ihr Update in beiden Systemen angezeigt.

>[!NOTE]
>
>Löscht werden nicht immer automatisch in beide Richtungen synchronisiert. Siehe [Löschen eines Interessenten oder Kontakts](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/deleting-a-lead-or-contact.md).

## Was ist, wenn in beiden Systemen gleichzeitig Änderungen am gleichen Feld vorgenommen werden? (Datenkollision) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Obwohl dies selten ist, wird Marketo gewinnen für Menschen (Interessenten) und Dynamics für Kontakte gewinnen. Das liegt daran, dass wir die Marketingabteilung für Menschen als maßgeblich betrachten, während das offizielle System der Kontaktaufnahme in der Verkaufsabteilung (CRM) besteht.

## Kann ich mit Marketo einen Lead in Dynamics erstellen? {#can-i-create-a-lead-in-dynamics-using-marketo}

Ja, verwenden Sie die Aktion [Person mit Microsoft ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md)-Textfluss synchronisieren. Dies wird einen Vorsprung in Dynamics erzeugen, wenn der Lead nicht existiert. Wenn der Interessent vorhanden ist, führt der Flussschritt keine Aktion durch.

>[!NOTE]
>
>Bei Verwendung der &quot;Synchronisierungsperson mit Microsoft&quot;-Flussaktion (nur in einer Trigger-Kampagne) wird der Interessent/Kontakt in Echtzeit in Dynamics erstellt.

## Kann ich manuell eine Synchronisierung einer Person von Marketo zu einem Lead in Dynamics erzwingen? {#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

Nein, die automatische Hintergrundsynchronisierung ist die einzige Möglichkeit, Updates zwischen Marketo und Dynamics zu synchronisieren. Die Aktion [Person mit Microsoft ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md)-Fluss synchronisieren erzwingt keine Synchronisierung des Interessenten.

## Welche Felder werden mit Marketo synchronisiert? {#what-fields-will-sync-to-marketo}

Sie können die zu synchronisierenden Felder [während des Setups auswählen.](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync)

## Wird Marketo die Dynamikvalidierungsregeln einhalten? {#will-marketo-respect-the-dynamics-validation-rules}

Ja. Die Synchronisierung schlägt fehl, wenn das Datenformat falsch ist oder die erforderlichen Feldinformationen fehlen. Marketo protokolliert das Ergebnis im Benutzerprotokoll, wenn dies der Fall ist.
