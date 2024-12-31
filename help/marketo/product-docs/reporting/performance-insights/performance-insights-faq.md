---
unique-page-id: 12979858
description: Häufig gestellte Fragen zu Performance Insights - Marketo-Dokumente - Produktdokumentation
title: Häufig gestellte Fragen zu Performance Insights
exl-id: cee791c3-1845-4fca-b803-c0dc1c644549
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1346'
ht-degree: 0%

---

# Häufig gestellte Fragen zu Performance Insights {#performance-insights-faq}

## Was ist die Definition von „Erfolg“ auf der Registerkarte Interaktion? {#what-is-the-definition-of-success-in-the-engagement-tab}

Erfolg ist ein Maßstab für sinnvolle Interaktion in Marketo. Zweck eines Programms ist es, eine sinnvolle Interaktion mit der Person oder dem potenziellen Kunden herzustellen. Erfolg wird markiert, wenn eine Person den Status erreicht, der dieses Ziel erreicht. Er kann an einem Webinar teilnehmen, auf einen Link in einer E-Mail klicken oder ein Web-Formular ausfüllen. Der Erfolg hängt vom Programmkanal ab.

>[!NOTE]
>
>Ein Webinar-Programm kann mehrere Status aufweisen, z. B. „Eingeladen“, „Registriert“ und „Teilgenommen“. Eingeladene oder registrierte Personen sind keine sinnvollen Interaktionen, da die Teilnehmer das Webinar nicht ansehen. Teilgenommen gilt in diesem Fall als erfolgreich.

## Funktioniert das MPI mit jedem CRM? {#will-mpi-work-with-any-crm}

Ja. Technisch gesehen interagiert MPI für die Datensynchronisation nicht direkt mit dem CRM. MPI nutzt die auf der Marketo Analytics-Data Warehouse gespeicherten Daten. Da die CRM-Synchronisierung in der Lead-Management-Anwendung erfolgt, zeigt jedes von Marketo unterstützte CRM, das in die Lead-Management-Anwendung integriert ist, die Daten korrekt an. Die CRM-Opportunity-Felder müssen jedoch korrekt den Marketo-Opportunity-Feldern zugeordnet werden.

## Ich besitze keine anderen Marketing Analytics-Produkte (ARB, RCE, RCA, Programmanalyse). Arbeitet MPI für mich? {#i-do-not-have-any-other-marketing-analytics-products-arb-rce-rca-program-analysis-will-mpi-work-for-me}

MPI ist ein unabhängiges Add-on zur Lead Management-Anwendung. Sie erfordert keine Verwendung anderer Analytics-Produkte.

## RCA zeigt mir auch Programmleistungsdaten. Gibt es einen Unterschied zwischen den in MPI und RCA angezeigten Daten? {#rca-shows-me-program-performance-data-as-well-is-there-a-difference-between-the-data-shown-in-mpi-and-rca}

Nein. MPI bezieht Daten aus demselben Data Warehouse wie RCA. Daher werden keine Datenunterschiede zwischen den beiden angezeigt. Mit RCA können Sie direkt eigene Berichte erstellen. Mit MPI erhalten Sie Zugriff auf visuelle Dashboards, die leicht verständlich sind.

## Ich möchte nicht, dass einige meiner Programme (z.B. operative Programme) im MPI angezeigt werden. Wie kontrolliere ich die Sichtbarkeit bestimmter Programme? {#i-don-t-want-some-of-my-programs-e-g-operational-to-show-up-in-mpi-how-do-i-control-the-visibility-of-specific-programs}

Sie können die Sichtbarkeit Ihrer Programme steuern, indem Sie das Analytics-Verhalten Ihrer Programme auf „Operativ“ festlegen. Dies führt dazu, dass das Programm aus den Analyseberechnungen ausgeschlossen wird.

>[!NOTE]
>
>Weitere Informationen zum Festlegen des Analytics-Verhaltens [hier](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/edit-analytics-behavior-settings.md).

## Ich führe eine Multi-Channel-Kampagne für eine neue Produkteinführung durch. Wie kann ich die Leistung dieser Kampagne über alle Kanäle hinweg an einem Ort anzeigen? {#i-am-running-a-multi-channel-campaign-for-a-new-product-launch-how-can-i-view-the-performance-for-this-campaign-across-all-the-different-channels-in-one-place}

Es wird empfohlen, für Programme, die Teil einer solchen Kampagne sind, Programm-Tags zu verwenden. Programm-Tags werden automatisch mit MPI synchronisiert, und Sie können sie in allen MPI-Dashboards filtern, um die Leistung Ihrer Multi-Channel-Kampagnen anzuzeigen.

## Habe ich Zugriff auf Attributionseinstellungen, wenn ich keine RCA habe? {#will-i-have-access-to-attribution-settings-if-i-do-not-have-rca}

Sie erhalten Zugriff auf Attributionseinstellungen, wenn Sie MPI haben, unabhängig davon, ob Sie RCA haben oder nicht.

## Ich erhalte einen Warnhinweis in MPI, wenn ich mich anmelde und meine Attributionseinstellungen falsch sind. Was ist los? {#i-get-an-alert-in-mpi-when-i-log-in-telling-me-that-my-attribution-settings-are-incorrect-what-s-wrong}

MPI berechnet, ob alle Ihre Opportunitys in Analytics einbezogen werden oder nicht. Andernfalls werden Sie aufgefordert, eine Änderung Ihrer Attributionseinstellungen (explizit, implizit, Hybrid) zu erwägen, um weitere Opportunitys einzuschließen.

Möglicherweise fehlen auch Opportunitys aufgrund fehlender Programmkosten in Ihren Programmen. Überprüfen Sie das Analytics-Verhalten Ihrer Programme. Sie können Folgendes sein:

1. Standard : Das Standardverhalten ist, dass das Programm NUR dann in MPI enthalten ist, wenn mindestens ein Zeitraum mit Kosten verbunden ist, auch wenn ein Zeitraum ohne Dollarzuweisung vorhanden ist.

1. Inklusiv : Mit dieser Option wird sichergestellt, dass das Programm in MPI verfügbar ist, unabhängig davon, ob Sie einen Kostenzeitraum einbezogen haben oder nicht.

1. [Operativ](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/best-practice-how-to-organize-your-programs.md#operational-programs) - Diese Option führt dazu, dass das Programm nicht im MPI angezeigt wird.

>[!NOTE]
>
>Der Kostenzeitraum **muss** für die Berichterstellung „Erfolg“ und „Neue Namen“ im Interaktions-Dashboard eingerichtet werden. Dieses Dashboard verwendet Daten zu den Periodenkosten, um Erfolge und neue Namen zu aggregieren. Wenn der Kostenzeitraum nicht eingerichtet ist, wird das Interaktions-Dashboard unabhängig von den obigen Einstellungen für das Analytics-Verhalten nicht korrekt ausgewertet.

## Warum verpasse ich einige Gelegenheiten im MPI? {#why-am-i-missing-some-opportunities-in-mpi}

Zwei Hauptgründe, warum Sie Chancen in MPI verpassen könnten, sind:

1. Die Attributionseinstellung ist auf „Explizit“ gesetzt, Opportunities ist jedoch keine Kontaktrolle zugewiesen
1. Periodenkosten sind nicht in Ihren Programmen enthalten

MPI berechnet, ob alle Ihre Opportunitys in Analytics einbezogen werden oder nicht. Andernfalls werden Sie aufgefordert, eine Änderung Ihrer Attributionseinstellungen (explizit, implizit, Hybrid) zu erwägen, um weitere Opportunitys einzuschließen.

Möglicherweise fehlen auch Opportunitys aufgrund fehlender Programmkosten in Ihren Programmen. Der Warnhinweis wird angezeigt, zeigt Ihnen jedoch nicht an, welche Programme Kosten vermissen. Bitte überprüfen Sie Ihre Programmeinrichtung, um Kosten einzubeziehen, um sicherzustellen, dass alle Ihre Programme und Möglichkeiten im MPI enthalten sind.

## Warum werden im Interaktions-Dashboard keine benutzerdefinierten Felder, Opportunity-Typen und ABM-Filter angezeigt? {#why-do-i-not-see-custom-fields-opportunity-type-and-abm-filters-on-the-engagement-dashboard}

Benutzerdefinierte Felder, Opportunity-Typ und ABM-Filter sind alle Attribute, die sich auf eine Opportunity beziehen. Mit dem Interaktions-Dashboard können Sie Ihre Interaktion und Lead-Akquise messen, unabhängig davon, ob sie mit einer Opportunity verbunden sind oder nicht. Da das Interaktions-Dashboard Opportunities nicht berücksichtigt, werden benutzerdefinierte Felder, Opportunity-Typ und ABM-Filter nicht angewendet.

## Ich möchte ein benutzerdefiniertes Salesforce-Opportunity-Feld anstelle des standardmäßigen Salesforce-Opportunity-Summenfelds für die Umsatzberichterstattung verwenden. Erlaubt mir das MPI? {#i-want-to-use-a-custom-salesforce-opportunity-field-for-revenue-reporting-instead-of-the-standard-salesforce-opportunity-amount-field-will-mpi-allow-me-to-do-that}

Ja. [Der Marketo-](https://nation.marketo.com/t5/Support/ct-p/Support) kann das Feld „Opportunity-Betrag“ von Marketo einem benutzerdefinierten Salesforce-Opportunity-Feld zuordnen, solange der Feldtyp „Währung“ ist. Da MPI auf das Marketo Opportunity-Summenfeld verweist, kann MPI die Daten aus dem neu zugeordneten benutzerdefinierten Salesforce-Feld verwenden.

>[!NOTE]
>
>Nach der Neuzuordnung zeigt MPI die Daten für die Zukunft an. Der historische Betrag wird nicht geändert.

## Wenn ich Opportunities nicht nutze, kann ich dann trotzdem MPI nutzen? {#if-i-don-t-use-opportunities-can-i-still-use-mpi}

Mit MPI können Sie die Programmleistung von der Trichterspitze bis hin zur Umsatzauswirkung messen. Wenn Sie Opportunities nicht nutzen, können Sie trotzdem:

* Zeigen Sie die Leistung Ihrer Nurture-Programme für die Interaktion mit Zielgruppen an.
* Leistung Ihrer Lead-Akquise-Programme anzeigen.
* Anzeigen der Leistung von Multi-Channel-Kampagnen mithilfe von Programm-Tags.
* Siehe Trends bei der Interaktion mit Zielgruppen in den letzten 12 Monaten.
* Speichern und Exportieren von Leistungsdaten in PowerPoint.

## Kann ich den Erfolg Account-basierter Strategien im MPI messen? {#can-i-measure-the-success-of-account-based-strategies-in-mpi}

Ja. MPI lässt sich mit [Marketo TAM](https://docs.marketo.com/display/DOCS/Account+Based+Marketing+Overview) integrieren, um ABM-Kontolisten nahtlos in MPI abzurufen. Sie können den Filter ABM-Kontenliste verwenden, um die gewünschte ABM-Liste zum Filtern von Daten nach auszuwählen.

## Ist Attribution beim Kauf von MPI sofort verfügbar? {#is-attribution-instantly-available-when-i-purchase-mpi}

Die Attributionsfunktionen von Marketo stehen unseren Kunden beim Kauf von MPI zur Verfügung. Es [ jedoch eine ](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md) Einrichtung erforderlich, um sicherzustellen, dass Opportunities und Programmdaten korrekt in das MPI fließen.

## Was muss ich tun, um Attribution einzurichten? {#what-do-i-have-to-do-to-set-up-attribution}

1. Opportunity-Einrichtung

   1. Sicherstellen, dass Opportunities mit Ihrem CRM synchronisiert werden
   1. Wenn Ihre Attributionseinstellungen auf „Explizit“ eingestellt sind, stellen Sie sicher, dass die Kontaktrollen für Opportunities ausgefüllt sind
   1. Es wird empfohlen, die Einstellung Attribution auf Hybrid zu ändern
   1. Programm-Installation

      1. Programmkosten in Ihre Programme einbeziehen
      1. Überprüfen Sie das Analytics-Verhalten, um anzugeben, ob ein Programm in Analytics eingeschlossen werden soll
      1. Festlegen der Erfolgskriterien für jeden Kanal, den Sie haben
      1. Person an Programme binden

         1. Stellen Sie sicher, dass das Akquiseprogramm und das Akquisedatum für jede Person in Ihrer Datenbank festgelegt wurden, damit die Erstkontakt-Attribution funktioniert.
         1. Stellen Sie sicher, dass Ihre Programme Erfolgsstatus für Personen in Ihrer Datenbank festlegen

>[!TIP]
>
>Alle erforderlichen Einrichtungsschritte werden in [diesem Artikel) ](/help/marketo/product-docs/reporting/performance-insights/setting-up-performance-insights.md).

## Was ist der Unterschied zwischen MPI und dem Programm-Analyzer? {#whats-the-difference-between-mpi-and-the-program-analyzer}

Mit dem Programm-Analyzer können Sie Ihre Programme mit bis zu vier Kennzahlen vergleichen. Mit MPI können Sie Ihren Kanal- und Programmbeitrag für eine ausgewählte Metrik wie Erfolg, neu erstellte Chancen usw. analysieren. Darüber hinaus können Sie den 12-monatigen Kanal-Trend basierend auf einer bestimmten von Ihnen ausgewählten Metrik anzeigen.

## Was ist der Unterschied zwischen MPI und dem erweiterten Report Builder? {#whats-the-difference-between-mpi-and-the-advanced-report-builder}

Der erweiterte Report Builder (manchmal auch als RCE bezeichnet) ist für Self-Service- (oder Ad-hoc-) Berichte konzipiert, die normalerweise von Marketing-Vorgängen ausgeführt werden. MPI wurde entwickelt, um Marketing-Experten und Marketing-Experten 1-Klick-Zugriff auf Leistungsanalysen zu bieten. Es ist nur eine minimale Einrichtung erforderlich.

## Was ist mit der Option „Vorheriges Jahr“ im Datumsfilter von Contribution passiert? {#what-happened-to-the-previous-year-option-in-contributions-date-filter}

Wir haben die Auswahl „Vorjahr“ vorübergehend entfernt. Sie haben weiterhin die Möglichkeit, die Leistungsdaten des gesamten Jahres mithilfe der benutzerdefinierten Datumsbereichsauswahl anzuzeigen.
