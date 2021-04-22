---
unique-page-id: 1147091
description: Informationen zur Programm-Mitgliedschaft - Marketo Docs - Produktdokumentation
title: Informationen zur Programm-Mitgliedschaft
exl-id: 02480a93-b499-4e0f-8a1c-a22f7d3b7178
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 1%

---

# Informationen zur Programm-Mitgliedschaft {#understanding-program-membership}

>[!NOTE]
>
>Marketo standardisiert jetzt die Sprache für alle Abonnements, sodass Sie möglicherweise Interessenten/Interessenten in Ihrem Abonnement und Personen/Personen in docs.marketo.com sehen können. Diese Begriffe bedeuten dasselbe. Es hat keine Auswirkungen auf die Artikelanweisungen. Es gibt auch noch einige andere Änderungen. [Weitere Informationen](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md).

>[!NOTE]
>
>**Definition:** Ein Mitglied ist eine Person, die in einem Programm den Status hat.

## So werden Personen Mitglieder eines Programms {#how-people-become-members-of-a-program}

1. Eine Person füllt ein [Formular auf einer Landingpage](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md) im Programm aus.

   1. Die Person hat automatisch den ersten Status in der Progression.

1. Sie [importieren Mitglieder aus einer CSV-Datei in das Programm](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-members-from-a-spreadsheet-into-a-program.md).

   1. Die Person hat automatisch den ersten Status in der Progression.

1. Verwenden Sie den Flussschritt [Programm ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md).
1. Eine Person registriert oder besucht ein [Webinar, das mit einem Ereignis-Programm](/help/marketo/product-docs/demand-generation/events/understanding-events/launchpoint-event-partners.md) synchronisiert wird.
1. Eine Person wird mit der Marketo iPad-Eincheckanwendung [erstellt.](/help/marketo/product-docs/core-marketo-concepts/mobile-apps/event-check-in/check-people-into-your-event-from-your-tablet.md)
1. Eine Person wird zu einer SFDC-Kampagne hinzugefügt, die mit dem Programm [synchronisiert wird.](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-campaign-sync.md)

>[!NOTE]
>
>Bei einem E-Mail-Programm wird eine Person nur dann zur Mitgliedschaft hinzugefügt, wenn die E-Mail gesendet wird.

## Programm-Status {#program-statuses}

Programm-Statusangaben sind die Schritte, die Personen in einem Programm ausführen (z. B. &quot;Eingeladen&quot;, &quot;RSVP&quot;d, &quot;Teilnehmer&quot;oder &quot;Keine Anzeige&quot;). Diese Schritte werden durch den [Kanal](/help/marketo/product-docs/administration/tags/create-a-program-channel.md) definiert.

![](assets/image2015-2-5-15-3a14-3a48.png)

>[!NOTE]
>
>Eine Person kann nicht rückwärts zu einem früheren Programm wechseln. Statusprogression ist nur eine Möglichkeit.

## Erfolgsstatus {#success-statuses}

Der Zweck eines Programms besteht darin, eine aussagekräftige Interaktion mit der Person oder dem Potenzieller Kunde herzustellen. Der Erfolg wird markiert, wenn eine Person den Status erreicht, der dieses Ziel erreicht.

>[!NOTE]
>
>Bei einem Webinar ist die Registrierung keine sinnvolle Interaktion, wenn sie das Webinar nicht wirklich anschauen. Die Teilnahme ist in diesem Fall ein Erfolg.

## Akquisitionsprogramm  {#acquisition-program}

Wenn ein neuer Programm als Systemmitglied in das System aufgenommen wird, legt Marketo dieses Programm automatisch als &quot;Akquise&quot;fest. Dadurch wird die Gutschrift für [First Touch-Zuordnung](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/understanding-attribution.md) eingerichtet.

>[!MORELIKETHIS]
>
>* [Tags in einem Programm verwenden](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags/use-tags-in-a-program.md)
>* [Erstellen eines Programm-Leistungsberichts](/help/marketo/product-docs/core-marketo-concepts/programs/program-performance-report/create-a-program-performance-report.md)

