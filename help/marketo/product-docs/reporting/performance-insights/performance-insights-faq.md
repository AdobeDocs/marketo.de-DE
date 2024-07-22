---
unique-page-id: 12979858
description: Häufig gestellte Fragen zu Leistungseinblicken - Marketo-Dokumente - Produktdokumentation
title: Häufig gestellte Fragen zu Leistungseinblicken
exl-id: cee791c3-1845-4fca-b803-c0dc1c644549
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1346'
ht-degree: 0%

---

# Häufig gestellte Fragen zu Leistungseinblicken {#performance-insights-faq}

## Wie lautet die Definition von &quot;Erfolg&quot;im Tab Interaktion? {#what-is-the-definition-of-success-in-the-engagement-tab}

Der Erfolg ist ein Maß für die sinnvolle Interaktion in Marketo. Ziel eines Programms ist es, eine sinnvolle Interaktion mit der Person oder dem Interessenten herzustellen. Der Erfolg wird markiert, wenn eine Person den Status erreicht, der dieses Ziel erreicht. Sie können an einem Webinar teilnehmen, auf einen Link in einer E-Mail klicken oder ein Webformular ausfüllen. Der Erfolg variiert je nach Programmkanal.

>[!NOTE]
>
>In einem Webinar-Programm können mehrere Status vorhanden sein, z. B.: Eingeladen, Registriert und Eingestiegen. Eingeladene oder registrierte Interaktionen sind nicht aussagekräftig, da die Leute sich das Webinar nicht ansehen. Die Teilnahme wird in diesem Fall als Erfolg betrachtet.

## Funktioniert MPI mit jedem CRM-System? {#will-mpi-work-with-any-crm}

Ja. Technisch betrachtet interagiert MPI nicht direkt mit dem CRM für die Datensynchronisation. MPI verwendet Daten, die auf der Marketo Analytics-Data Warehouse gespeichert sind. Da die CRM-Synchronisation in der Lead-Management-Anwendung erfolgt, werden in allen von Marketo unterstützten CRM-Systemen, die in die Lead-Management-Anwendung integriert sind, die Daten korrekt angezeigt. Die CRM-Opportunitätsfelder müssen jedoch den Marketo-Opportunities-Feldern korrekt zugeordnet werden.

## Ich habe keine anderen Marketing Analytics-Produkte (ARB, RCE, RCA, Programmanalyse). Wird MPI für mich arbeiten? {#i-do-not-have-any-other-marketing-analytics-products-arb-rce-rca-program-analysis-will-mpi-work-for-me}

MPI ist ein unabhängiges Add-on zur Anwendung &quot;Lead Management&quot;. Die Verwendung anderer Analyseprodukte ist nicht erforderlich.

## RCA zeigt auch Daten zur Programmleistung an. Gibt es einen Unterschied zwischen den in MPI und RCA angezeigten Daten? {#rca-shows-me-program-performance-data-as-well-is-there-a-difference-between-the-data-shown-in-mpi-and-rca}

Anz. MPI liefert Daten aus demselben Data Warehouse wie RCA. Daher gibt es keine Datenunterschiede zwischen den beiden. Mit RCA können Sie direkt Ihre eigenen Berichte erstellen. MPI bietet Ihnen Zugriff auf leicht verständliche visuelle Dashboards.

## Ich möchte nicht, dass einige meiner Programme (z.B. operationell) in MPI angezeigt werden. Wie kann ich die Sichtbarkeit bestimmter Programme steuern? {#i-don-t-want-some-of-my-programs-e-g-operational-to-show-up-in-mpi-how-do-i-control-the-visibility-of-specific-programs}

Sie können die Sichtbarkeit Ihrer Programme steuern, indem Sie das Analytics-Verhalten Ihrer Programme auf &quot;Operativ&quot;setzen. Dadurch wird das Programm aus den Analyseberechnungen ausgeschlossen.

>[!NOTE]
>
>Erfahren Sie mehr über das Festlegen des Analytics-Verhaltens [hier](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/edit-analytics-behavior-settings.md).

## Ich führe eine kanalübergreifende Kampagne für einen neuen Produktstart durch. Wie kann ich die Leistung dieser Kampagne über alle Kanäle hinweg an einem Ort anzeigen? {#i-am-running-a-multi-channel-campaign-for-a-new-product-launch-how-can-i-view-the-performance-for-this-campaign-across-all-the-different-channels-in-one-place}

Es wird empfohlen, für Programme, die Teil einer solchen Kampagne sind, Programm-Tags zu verwenden. Programm-Tags werden automatisch mit MPI synchronisiert und Sie können sie in allen MPI-Dashboards filtern, um Ihre kanalübergreifende Kampagnenleistung anzuzeigen.

## Habe ich Zugriff auf Attributionseinstellungen, wenn ich keine RCA habe? {#will-i-have-access-to-attribution-settings-if-i-do-not-have-rca}

Sie erhalten Zugriff auf Attributionseinstellungen bei MPI, unabhängig davon, ob Sie über RCA verfügen oder nicht.

## Ich erhalte eine Warnung in MPI, wenn ich mich anmelde und mir sage, dass meine Attributionseinstellungen falsch sind. Was ist los? {#i-get-an-alert-in-mpi-when-i-log-in-telling-me-that-my-attribution-settings-are-incorrect-what-s-wrong}

MPI berechnet, ob alle Ihre Möglichkeiten in die Analyse einbezogen werden. Andernfalls werden Sie aufgefordert, eine Änderung Ihrer Attributionseinstellungen (explizit, implizit, Hybrid) in Erwägung zu ziehen, um weitere Möglichkeiten einzuschließen.

Möglicherweise fehlen Ihnen auch Chancen aufgrund der fehlenden Programmkosten in Ihren Programmen. Bitte überprüfen Sie das Analytics-Verhalten Ihrer Programme. Sie können:

1. Standard - Das Standardverhalten ist, dass das Programm NUR dann in MPI enthalten ist, wenn es mindestens einen Zeitraum kostet, selbst wenn einem keine Dollar zugewiesen ist.

1. Einschließlich - Mit dieser Option wird sichergestellt, dass das Programm in MPI verfügbar ist, unabhängig davon, ob Sie Zeitraumkosten angegeben haben oder nicht.

1. [Operativ](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs.md#operational-programs) - Diese Option führt dazu, dass das Programm nicht in MPI angezeigt wird.

>[!NOTE]
>
>Period Cost **has** werden für die Berichterstellung &quot;Success&quot;und &quot;New Names&quot;im Interaktions-Dashboard eingerichtet. In diesem Dashboard werden Daten zu den Period-Kosten verwendet, um Erfolge und neue Namen zu aggregieren. Wenn die Zeitkosten nicht eingerichtet sind, wird das Interaktions-Dashboard unabhängig von den oben genannten Analytics-Verhaltenseinstellungen nicht korrekt berichtet.

## Warum vermisse ich einige Möglichkeiten in MPI? {#why-am-i-missing-some-opportunities-in-mpi}

Zwei wesentliche Gründe, aus denen Ihnen möglicherweise Chancen in MPI fehlen:

1. Die Attributionseinstellung ist auf Explizit festgelegt, aber den Möglichkeiten sind keine Kontaktrollen zugewiesen.
1. Die Zeitkosten sind nicht in Ihren Programmen enthalten.

MPI berechnet, ob alle Ihre Möglichkeiten in die Analyse einbezogen werden. Andernfalls werden Sie aufgefordert, eine Änderung Ihrer Attributionseinstellungen (explizit, implizit, Hybrid) in Erwägung zu ziehen, um weitere Möglichkeiten einzuschließen.

Möglicherweise fehlen Ihnen auch Chancen aufgrund der fehlenden Programmkosten in Ihren Programmen. Der Warnhinweis wird angezeigt, zeigt aber nicht an, auf welche Programme Kosten fehlen. Bitte überprüfen Sie Ihre Programmeinrichtung, um Kosten einzubeziehen, um sicherzustellen, dass alle Ihre Programme und Möglichkeiten in MPI enthalten sind.

## Warum werden im Interaktions-Dashboard keine benutzerdefinierten Felder, Opportunity Type und ABM-Filter angezeigt? {#why-do-i-not-see-custom-fields-opportunity-type-and-abm-filters-on-the-engagement-dashboard}

Benutzerdefinierte Felder, Opportunity-Typ und ABM-Filter sind alle Attribute, die sich auf eine Chance beziehen. Mit dem Interaktions-Dashboard können Sie Ihre Interaktion messen und Akquise leiten, unabhängig davon, ob sie mit einer Gelegenheit verbunden sind oder nicht. Da das Interaktions-Dashboard die Möglichkeiten nicht berücksichtigt, gelten benutzerdefinierte Felder, Opportunity Type und ABM Filters nicht.

## Ich möchte ein benutzerdefiniertes Feld für Salesforce-Chancen für Umsatzberichte anstelle des standardmäßigen Felds Salesforce Opportunity Amount verwenden. Ermöglicht mir MPI das? {#i-want-to-use-a-custom-salesforce-opportunity-field-for-revenue-reporting-instead-of-the-standard-salesforce-opportunity-amount-field-will-mpi-allow-me-to-do-that}

Ja. Der [Marketo-Support](https://nation.marketo.com/t5/Support/ct-p/Support) kann das Marketo-Feld &quot;Opportunity Amount&quot;in ein benutzerdefiniertes Salesforce Opportunity-Feld umwandeln, sofern der Feldtyp eine Währung ist. Da MPI auf das Feld Marketo Opportunity amount verweist, kann MPI die Daten aus dem neu zugeordneten benutzerdefinierten Salesforce-Feld verwenden.

>[!NOTE]
>
>Nach der Neukodifizierung zeigt MPI die Daten an. Der historische Betrag wird nicht geändert.

## Wenn ich keine Möglichkeiten verwende, kann ich MPI trotzdem verwenden? {#if-i-don-t-use-opportunities-can-i-still-use-mpi}

Mit MPI können Sie die Programmleistung von oben im Trichter bis hin zu den Auswirkungen auf den Umsatz messen. Wenn Sie keine Möglichkeiten nutzen, können Sie weiterhin:

* Zeigen Sie die Leistung Ihrer Pflegeprogramme für die Interaktion mit Zielgruppen an.
* Zeigen Sie die Leistung Ihrer Lead-Akquiseprogramme an.
* Anzeigen der Leistung von kanalübergreifenden Kampagnen über Programm-Tags.
* Siehe Interaktionstrends der Zielgruppen in den letzten 12 Monaten.
* Speichern und exportieren Sie Leistungsdaten in PowerPoint.

## Kann ich den Erfolg von kontobasierten Strategien in MPI messen? {#can-i-measure-the-success-of-account-based-strategies-in-mpi}

Ja. MPI kann mit [Marketo TAM](https://docs.marketo.com/display/DOCS/Account+Based+Marketing+Overview) integriert werden, um ABM-Kontolisten nahtlos in MPI abzurufen. Sie können den Filter ABM-Kontoliste verwenden, um die gewünschte ABM-Liste auszuwählen, nach der die Daten gefiltert werden sollen.

## Ist die Attribution sofort verfügbar, wenn ich MPI kaufe? {#is-attribution-instantly-available-when-i-purchase-mpi}

Die Marketo-Attributionsfunktionen stehen unseren Kunden beim Kauf von MPI zur Verfügung. Allerdings ist [ordnungsgemäßes Setup](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md) erforderlich, um sicherzustellen, dass die Chancen- und Programmdaten korrekt in MPI fließen.

## Was muss ich tun, um eine Attribution einzurichten? {#what-do-i-have-to-do-to-set-up-attribution}

1. Einrichtung von Chancen

   1. Stellen Sie sicher, dass die Möglichkeiten mit Ihrem CRM-System synchronisiert werden
   1. Wenn Ihre Attributionseinstellungen auf Explizit festgelegt sind, stellen Sie sicher, dass Kontaktrollen zu Chancen gefüllt werden.
   1. Es wird empfohlen, die Attributionseinstellung in Hybrid zu ändern.
   1. Programm-Installation

      1. Programmkosten in Ihre Programme aufnehmen
      1. Überprüfen Sie das Analyseverhalten, um anzugeben, ob ein Programm in die Analyse einbezogen werden soll.
      1. Festlegen der Erfolgskriterien für jeden Kanal, den Sie haben
      1. Personen an Programme binden

         1. Stellen Sie sicher, dass das Akquiseprogramm und das Akquisedatum für jede Person in Ihrer Datenbank festgelegt wurden, damit die Erstkontaktzuordnung funktioniert.
         1. Stellen Sie sicher, dass Ihre Programme Erfolgsstatus für Personen in Ihrer Datenbank festlegen.

>[!TIP]
>
>Alle erforderlichen Einrichtungsschritte werden in [diesem Artikel](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md) beschrieben.

## Was ist der Unterschied zwischen MPI und dem Programm Analyzer? {#whats-the-difference-between-mpi-and-the-program-analyzer}

Mit dem Programm-Analyzer können Sie Ihre Programme mit bis zu vier Kennzahlen vergleichen. Mit MPI können Sie Ihren Kanal- und Programmbeitrag zu einer ausgewählten Metrik analysieren, z. B. Erfolg, neu erstellte Chancen usw. Sie können damit auch den 12-Monats-Kanal-Trend basierend auf einer bestimmten Metrik anzeigen, die Sie ausgewählt haben.

## Was ist der Unterschied zwischen MPI und dem Advanced Report Builder? {#whats-the-difference-between-mpi-and-the-advanced-report-builder}

Der erweiterte Report Builder (manchmal auch als RCE bezeichnet) ist für Self-Service-Berichte (oder Ad-hoc-Berichte) konzipiert, die normalerweise von Marketing-Vorgängen durchgeführt werden. MPI wurde entwickelt, um Marketing-Experten und Marketing-Experten einen einmaligen Zugriff auf die Leistungsanalyse zu ermöglichen. Es ist eine minimale Einrichtung erforderlich.

## Was ist mit der Option &quot;Vorheriges Jahr&quot;im Datumsfilter des Beitrags passiert? {#what-happened-to-the-previous-year-option-in-contributions-date-filter}

Die Auswahl &quot;Vorheriges Jahr&quot;wurde vorübergehend entfernt. Sie haben weiterhin die Möglichkeit, die Leistungsdaten des gesamten Jahres mithilfe der Auswahl des benutzerdefinierten Datumsbereichs anzuzeigen.
