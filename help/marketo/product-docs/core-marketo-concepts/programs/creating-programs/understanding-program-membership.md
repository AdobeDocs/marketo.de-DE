---
unique-page-id: 1147091
description: Grundlegendes zur Programmmitgliedschaft - Marketo-Dokumente - Produktdokumentation
title: Grundlegendes zur Programmmitgliedschaft
exl-id: 02480a93-b499-4e0f-8a1c-a22f7d3b7178
feature: Programs
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 1%

---

# Grundlegendes zur Programmmitgliedschaft {#understanding-program-membership}

>[!NOTE]
>
>Marketo standardisiert jetzt die Sprache für alle Abonnements, sodass Sie Leads/Leads in Ihrem Abonnement und Personen in unseren Dokumenten sehen können. Diese Begriffe bedeuten das Gleiche; sie wirken sich nicht auf Artikelanweisungen aus. Es gibt auch einige andere Änderungen. [Weitere Informationen](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md).

>[!NOTE]
>
>**Definition:** Ein Mitglied ist eine Person, die einen Status in einem Programm hat.

## Wie Menschen Mitglieder eines Programms werden {#how-people-become-members-of-a-program}

1. Eine Person füllt eine [Formular auf einer Landingpage](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md) im Programm.

   1. Der erste Status des Fortschritts wird automatisch von Person übernommen.

1. You [Mitglieder in das Programm importieren](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-members-from-a-spreadsheet-into-a-program.md) aus einer CSV-Datei.

   1. Der erste Status des Fortschritts wird automatisch von Person übernommen.

1. Sie verwenden die [Ändern des Programmstatus](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md) Flussschritt.
1. Eine Person registriert oder besucht eine [Webinar mit einem Veranstaltungsprogramm synchronisiert](/help/marketo/product-docs/demand-generation/events/understanding-events/event-partners.md).
1. Eine Person ist [mit der Marketo iPad-Eincheckanwendung erstellt wurde](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/check-people-into-your-event-from-your-tablet.md).
1. Eine Person wird zu einer SFDC-Kampagne hinzugefügt, die [mit dem Programm synchronisiert](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md).

>[!NOTE]
>
>Bei E-Mail-Programmen wird eine Person nur zum Zeitpunkt des Versands der E-Mail zur Mitgliedschaft hinzugefügt.

## Programmstatus {#program-statuses}

Programmstatus sind die Schritte, die Benutzer in einem Programm durchlaufen (z. B. Eingeladene, RSVP&#39;d, Teilnehmer, Keine Sendung). Diese Schritte werden durch die Variable [channel](/help/marketo/product-docs/administration/tags/create-a-program-channel.md).

![](assets/image2015-2-5-15-3a14-3a48.png)

>[!NOTE]
>
>Eine Person kann nicht zu einem früheren Programmstatus zurückkehren. Der Statusfortschritt ist nur eine Möglichkeit.

## Erfolgsstatus {#success-statuses}

Ziel eines Programms ist es, eine sinnvolle Interaktion mit der Person oder dem Interessenten herzustellen. Der Erfolg wird markiert, wenn eine Person den Status erreicht, der dieses Ziel erreicht.

>[!NOTE]
>
>Für ein Webinar ist die Registrierung keine sinnvolle Interaktion, wenn sie sich das Webinar nicht ansehen. In diesem Fall ist die Teilnahme ein Erfolg.

## Akquirierungsprogramm  {#acquisition-program}

Wenn ein neuer Name in das System als Programmmitglied aufgenommen wird, setzt Marketo dieses Programm automatisch als &quot;Akquise&quot;. Dadurch wird die Gutschrift für [Erstkontakt-Attribution](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md).

>[!MORELIKETHIS]
>
>* [Verwenden von Tags in einem Programm](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags/use-tags-in-a-program.md)
>* [Erstellen eines Berichts zur Programmleistung](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report.md)
