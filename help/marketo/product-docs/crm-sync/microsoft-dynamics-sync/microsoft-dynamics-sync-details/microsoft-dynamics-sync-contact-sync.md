---
unique-page-id: 3571833
description: Synchronisation von Microsoft Dynamics - Kontaktsynchronisierung - Marketo-Dokumente - Produktdokumentation
title: Synchronisation von Microsoft Dynamics - Kontaktsynchronisierung
exl-id: d4583ea0-2b52-415e-b28c-a8eafebeff64
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 0%

---

# Microsoft Dynamics Sync: Kontaktsynchronisierung {#microsoft-dynamics-sync-contact-sync}

Wussten Sie, dass Marketo Engage Ihre gesamte Datenbank mit Dynamics synchronisiert? Es wird synchronisiert, dann 5 Minuten wartet und dann wieder synchronisiert, den ganzen Tag, jeden Tag. Im Folgenden finden Sie einige Details dazu, wie Marketo Dynamics-Kontakte spezifisch behandelt.

## Wie werden die Details zwischen den beiden Systemen synchronisiert? {#how-are-details-kept-in-sync-between-the-two-systems}

Die Synchronisation von Kontakten erfolgt bidirektional. Wenn Sie Änderungen an einem Kontakt in Dynamics oder einer Person in Marketo vornehmen, werden Ihre Aktualisierungen in beiden Systemen übernommen.

## Was passiert, wenn in beiden Systemen gleichzeitig Änderungen an demselben Feld vorgenommen werden? (Datenkollision) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Obwohl dies selten vorkommt, wird Marketo für Menschen gewinnen und Dynamics gewinnt Kontakte. Dies liegt daran, dass wir die Marketing-Abteilung für Menschen als maßgeblich betrachten, während das offizielle System der Kontaktaufnahme in der Vertriebs- (CRM-) Abteilung ist.

## Kann ich einen Kontakt mit Marketo erstellen? {#can-i-create-a-contact-using-marketo}

Ja. [So](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync/create-a-contact-in-microsoft-dynamics.md){target="_blank"}.

>[!NOTE]
>
>Bei Verwendung der FlusAktion &quot;Person mit Microsoft synchronisieren&quot;(nur in einer Trigger-Kampagne) wird der Lead/Kontakt in Echtzeit in Dynamics erstellt.

## Kann ich die Synchronisierung einer Person oder eines Kontakts manuell erzwingen? {#can-i-manually-force-a-sync-of-a-person-or-a-contact}

Nein, die automatisierte Hintergrundsynchronisierung ist die einzige Möglichkeit, Updates zwischen Marketo und Dynamics zu synchronisieren. Die [Person mit Microsoft synchronisieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md){target="_blank"} erzwingt keine Synchronisierung des Leads.

## Welche Felder werden mit Marketo synchronisiert? {#what-fields-will-sync-to-marketo}

Sie können [Auswahl der zu synchronisierenden Felder](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} während der Einrichtung. Marketo synchronisiert jedoch nur die Felder, auf die der Benutzer für die Synchronisierung mit Dynamics Zugriff hat.

## Wird Marketo die Dynamics-Validierungsregeln einhalten? {#will-marketo-respect-the-dynamics-validation-rules}

Ja, wenn ein Konflikt vorliegt, wird das Ergebnis im Interessenten-Aktivitätsprotokoll protokolliert.
