---
unique-page-id: 3571833
description: Microsoft Dynamics Sync - Contact Sync - Marketing Docs - Produktdokumentation
title: Microsoft Dynamics Sync - Contact Sync
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Kontaktsynchronisierung {#microsoft-dynamics-sync-contact-sync}

Wussten Sie, dass Marketo Ihre gesamte Datenbank mit Dynamics synchronisiert? Es synchronisiert, wartet dann 5 Minuten und synchronisiert dann den ganzen Tag, jeden Tag. Hier sind einige Details darüber, wie Marketo Dynamikkontakte speziell behandelt.

## Wie werden die Details zwischen den beiden Systemen synchronisiert? {#how-are-details-kept-in-sync-between-the-two-systems}

Die Kontaktsynchronisierung erfolgt in beide Richtungen. Wenn Sie Änderungen an einem Kontakt in Dynamics oder einer Person in Marketo vornehmen, werden Ihre Updates in beiden Systemen übernommen.

## Was ist, wenn in beiden Systemen gleichzeitig Änderungen am gleichen Feld vorgenommen werden? (Datenkollision) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Obwohl dies selten ist, wird Marketo für Menschen gewinnen und Dynamics für Kontakte gewinnen. Das liegt daran, dass wir die Marketingabteilung für Menschen als maßgeblich betrachten, während das offizielle System der Kontaktaufnahme in der Verkaufsabteilung (CRM) besteht.

## Kann ich einen Kontakt mit Marketo erstellen? {#can-i-create-a-contact-using-marketo}

Ja. [So](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync/create-a-contact-in-microsoft-dynamics.md) geht&#39;s.

>[!NOTE]
>
>Bei Verwendung der &quot;Synchronisierungsperson mit Microsoft&quot;-Flussaktion (nur in einer Trigger-Kampagne) wird der Interessent/Kontakt in Echtzeit in Dynamics erstellt.

## Kann ich eine Synchronisierung einer Person oder eines Kontakts manuell erzwingen? {#can-i-manually-force-a-sync-of-a-person-or-a-contact}

Nein, die automatische Hintergrundsynchronisierung ist die einzige Möglichkeit, Updates zwischen Marketo und Dynamics zu synchronisieren. Die Variable [Person mit Microsoft ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) synchronisieren erzwingt keine Synchronisierung des Interessenten.

## Welche Felder werden mit Marketo synchronisiert? {#what-fields-will-sync-to-marketo}

Sie können die zu synchronisierenden Felder [während des Setups auswählen. ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) Marketo synchronisiert jedoch nur die Felder, auf die Ihr Dynamics Sync-Benutzer Zugriff hat.

## Wird Marketo die Dynamikvalidierungsregeln einhalten? {#will-marketo-respect-the-dynamics-validation-rules}

Ja, wenn ein Konflikt vorliegt, wird das Ergebnis im Protokoll der Interessenten-Aktivität protokolliert.
