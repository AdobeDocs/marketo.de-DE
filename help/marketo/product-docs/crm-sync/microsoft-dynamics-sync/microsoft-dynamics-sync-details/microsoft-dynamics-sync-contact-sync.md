---
unique-page-id: 3571833
description: Microsoft Dynamics-Synchronisierung - Kontaktsynchronisierung - Marketo-Dokumente - Produktdokumentation
title: Microsoft Dynamics-Synchronisierung - Kontaktsynchronisierung
exl-id: d4583ea0-2b52-415e-b28c-a8eafebeff64
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics]: Kontaktsynchronisierung {#microsoft-dynamics-sync-contact-sync}

Wussten Sie, dass Marketo Ihre gesamte Datenbank mit [!DNL Dynamics] synchronisiert? Er synchronisiert, wartet dann 5 Minuten und synchronisiert dann erneut, den ganzen Tag, jeden Tag. Im Folgenden finden Sie einige Details dazu, wie Marketo [!DNL Dynamics] Kontakte spezifisch behandelt.

## Wie werden die Details zwischen den beiden Systemen synchron gehalten? {#how-are-details-kept-in-sync-between-the-two-systems}

Die Kontaktsynchronisation erfolgt bidirektional. Wenn Sie Änderungen an einem Kontakt in [!DNL Dynamics] oder an einer Person in Marketo vornehmen, werden Ihre Aktualisierungen auf beiden Systemen angezeigt.

## Was passiert, wenn Änderungen am selben Feld in beiden Systemen gleichzeitig vorgenommen werden? (Datenkollision) {#what-if-changes-are-made-to-the-same-field-in-both-systems-at-the-same-time-data-collision}

Obwohl dies selten vorkommt, wird Marketo für die Menschen gewinnen und [!DNL Dynamics] für die Kontakte. Der Grund dafür ist, dass wir die Marketing-Abteilung für die Menschen als verbindlich betrachten, während das offizielle System der Aufzeichnung für Kontakte in der Verkaufs- (CRM)-Abteilung ist.

## Kann ich mit Marketo einen Kontakt erstellen? {#can-i-create-a-contact-using-marketo}

Ja. [So geht&#39;](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync/create-a-contact-in-microsoft-dynamics.md){target="_blank"}.

>[!NOTE]
>
>Bei Verwendung der Flussaktion „Person mit Microsoft synchronisieren“ (nur in einer Trigger-Kampagne) wird der Lead/Kontakt in Echtzeit in [!DNL Dynamics] erstellt.

## Kann ich die Synchronisierung einer Person oder eines Kontakts manuell erzwingen? {#can-i-manually-force-a-sync-of-a-person-or-a-contact}

Nein, die automatische Hintergrundsynchronisierung ist die einzige Möglichkeit, Aktualisierungen zwischen Marketo und [!DNL Dynamics] zu synchronisieren. Die [Person mit Microsoft synchronisieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md) erzwingt keine Synchronisierung des Leads.

## Welche Felder werden mit Marketo synchronisiert? {#what-fields-will-sync-to-marketo}

Sie können [ Setup Felder auswählen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) die synchronisiert werden sollen. Marketo synchronisiert jedoch nur die Felder, auf die der [!DNL Dynamics] Synchronisierungsbenutzer Zugriff hat.

## Wird Marketo die [!DNL Dynamics] Validierungsregeln einhalten? {#will-marketo-respect-the-dynamics-validation-rules}

Ja, wenn ein Konflikt auftritt, wird das Ergebnis im Aktivitätsprotokoll des Leads protokolliert.
