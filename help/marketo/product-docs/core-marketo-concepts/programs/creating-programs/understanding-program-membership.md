---
unique-page-id: 1147091
description: Grundlagen zur Programmmitgliedschaft - Marketo-Dokumente - Produktdokumentation
title: Grundlegendes zur Programmmitgliedschaft
exl-id: 02480a93-b499-4e0f-8a1c-a22f7d3b7178
feature: Programs
source-git-commit: 93d6e498ee69a1a9fdee7956ac351764cf18a87a
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---

# Grundlegendes zur Programmmitgliedschaft {#understanding-program-membership}

>[!NOTE]
>
>**Definition:** Ein Mitglied ist eine Person, die einen Status in einem Programm hat.

## Wie Personen Mitglieder eines Programms werden {#how-people-become-members-of-a-program}

1. Eine Person füllt ein [Formular auf einer Landingpage](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"} im Programm aus.

   * Die Person hat automatisch den ersten Status in der Progression.

1. Sie [ Mitglieder aus einer CSV](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-members-from-a-spreadsheet-into-a-program.md){target="_blank"}Datei in das Programm importieren.

   * Die Person hat automatisch den ersten Status in der Progression.

1. Sie verwenden den [Programmstatus ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md){target="_blank"} Flussschritt.
1. Eine Person registriert sich oder nimmt an einem [Webinar teil, das mit einem Veranstaltungsprogramm synchronisiert ](/help/marketo/product-docs/demand-generation/events/understanding-events/event-partners.md){target="_blank"}.
1. Eine Person wird [mithilfe des Marketo iPad-Eincheckprogramms erstellt](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/check-people-into-your-event-from-your-tablet.md){target="_blank"}.
1. Eine Person wird zu einer SFDC-Kampagne hinzugefügt, die mit [ Programm synchronisiert ](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md){target="_blank"}.

>[!NOTE]
>
>Bei einem E-Mail-Programm wird eine Person nur dann zur Mitgliedschaft hinzugefügt, wenn die E-Mail gesendet wird.

## Programmstatus {#program-statuses}

Programmstatus sind die Schritte, die Benutzer in einem Programm durchlaufen (z. B. „Eingeladen“, „Bewerbungsunterlagen“, „Teilgenommen“, „Keine Sendung„). Diese Schritte werden durch den [channel](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"} definiert.

![](assets/image2015-2-5-15-3a14-3a48.png)

>[!NOTE]
>
>Eine Person kann nicht zu einem früheren Programmstatus zurückkehren. Statusfortschritt ist nur eine Möglichkeit.

## Erfolgsstatus {#success-statuses}

Zweck eines Programms ist es, eine sinnvolle Interaktion mit der Person oder dem potenziellen Kunden herzustellen. Erfolg wird markiert, wenn eine Person den Status erreicht, der dieses Ziel erreicht.

>[!NOTE]
>
>Für ein Webinar ist die Registrierung keine sinnvolle Interaktion, wenn sie sich das Webinar nicht tatsächlich ansehen. Die Teilnahme ist in diesem Fall erfolgreich.

## Akquirierungsprogramm {#acquisition-program}

Wenn ein neuer Name als Programmteilnehmer in das System eintritt, setzt Marketo dieses Programm automatisch auf „Akquise“. Dadurch wird eine Gutschrift für [Erstkontakt-Attribution](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md){target="_blank"} erstellt.

>[!MORELIKETHIS]
>
>* [Verwenden von Tags in einem Programm](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/use-tags-in-a-program.md){target="_blank"}
>* [Erstellen eines Programmleistungsberichts](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report.md){target="_blank"}
