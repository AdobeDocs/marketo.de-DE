---
unique-page-id: 3571848
description: Microsoft Dynamics Sync - Lead Sync - Marketing Docs - Produktdokumentation
title: Microsoft Dynamics Sync - Lead Sync
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Interessentenabgleich {#microsoft-dynamics-sync-lead-sync}

Marketo to to Dynamics sync ist super leistungsfähig. Im Folgenden finden Sie die Details:

## Wie werden die Details zwischen den beiden Systemen synchronisiert? {#how-are-details-kept-in-sync-between-the-two-systems}

Die Synchronisierung erfolgt bidirektional. Wenn Sie Änderungen an einem Lead in Dynamics oder einer Person in Marketo vornehmen, wird Ihr Update in beiden Systemen angezeigt.

>[!NOTE]
>
>Löscht werden nicht immer automatisch in beide Richtungen synchronisiert. Siehe [Löschen eines Interessenten oder Kontakts](http://docs.marketo.com/x/agO1Ag).

## Was ist, wenn in beiden Systemen gleichzeitig Änderungen am gleichen Feld vorgenommen werden? (Datenkollision) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Obwohl dies selten ist, wird Marketo gewinnen für Menschen (Interessenten) und Dynamics für Kontakte gewinnen. Das liegt daran, dass wir die Marketingabteilung für Menschen als maßgeblich betrachten, während das offizielle System der Kontaktaufnahme in der Verkaufsabteilung (CRM) besteht.

## Kann ich mit Marketo einen Lead in Dynamics erstellen? {#can-i-create-a-lead-in-dynamics-using-marketo}

Ja, verwenden Sie die [Aktion &quot;Person mit Microsoft](../../../../product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) synchronisieren&quot;. Dies wird einen Vorsprung in Dynamics erzeugen, wenn der Lead nicht existiert. Wenn der Interessent vorhanden ist, führt der Flussschritt keine Aktion durch.

>[!NOTE]
>
>Bei Verwendung der &quot;Synchronisierungsperson mit Microsoft&quot;-Flussaktion (nur in einer Auslöseraktion) wird der Interessent/Kontakt in Echtzeit in Dynamics erstellt.

## Kann ich manuell eine Synchronisierung einer Person von Marketo zu einem Lead in Dynamics erzwingen? {#can-i-manually-force-a-sync-of-a-person-from-marketo-to-a-lead-in-dynamics}

Nein, die automatische Hintergrundsynchronisierung ist die einzige Möglichkeit, Updates zwischen Marketo und Dynamics zu synchronisieren. Die Aktion [Person mit Microsoft](../../../../product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) synchronisieren erzwingt keine Synchronisierung des Interessenten.

## Welche Felder werden mit Marketo synchronisiert? {#what-fields-will-sync-to-marketo}

Sie können Felder [auswählen, die während der Einrichtung synchronisiert](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) werden sollen.

## Wird Marketo die Dynamikvalidierungsregeln einhalten? {#will-marketo-respect-the-dynamics-validation-rules}

Ja. Die Synchronisierung schlägt fehl, wenn das Datenformat falsch ist oder die erforderlichen Feldinformationen fehlen. Marketo protokolliert das Ergebnis im Benutzerprotokoll, wenn dies der Fall ist.

