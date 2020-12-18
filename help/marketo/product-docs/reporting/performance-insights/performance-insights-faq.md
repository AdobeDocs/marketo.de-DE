---
unique-page-id: 12979858
description: Häufig gestellte Fragen zu Performance Insights - Marketing Docs - Produktdokumentation
title: Häufig gestellte Fragen zu Performance Insights
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '1404'
ht-degree: 0%

---


# Häufig gestellte Fragen zu Performance Insights {#performance-insights-faq}

## Was ist die Definition von &quot;Erfolg&quot;in der Registerkarte &quot;Interaktion&quot;? {#what-is-the-definition-of-success-in-the-engagement-tab}

Erfolg ist ein Maß für sinnvolle Interaktion in Marketo. Der Zweck eines Programms besteht darin, eine aussagekräftige Interaktion mit der Person oder dem Potenzieller Kunde herzustellen. Der Erfolg wird markiert, wenn eine Person den Status erreicht, der dieses Ziel erreicht. Sie kann an einem Webinar teilnehmen, auf einen Link in einer E-Mail klicken oder ein Webformular ausfüllen. Der Erfolg hängt vom Kanal des Programms ab.

>[!NOTE]
>
>**Beispiel**
>
>In einem Webinar-Programm können mehrere Status vorhanden sein, z. B.: Eingeladen, registriert und teilgenommen. Eingeladene oder registrierte Interaktionen sind keine sinnvollen Interaktionen, weil die Leute das Webinar nicht wirklich ansehen. Die Teilnahme wird in diesem Fall als Erfolg betrachtet.

## Funktioniert MPI mit jedem CRM-System? {#will-mpi-work-with-any-crm}

Ja. Technisch betrachtet interagiert MPI nicht direkt mit dem CRM für die Datensynchronisierung. MPI verwendet Daten, die in der Data Warehouse von Marketing-Analytics gespeichert sind. Da die CRM-Synchronisierung in der Lead Management-Anwendung stattfindet, werden die Daten in allen in die Lead Management-Anwendung integrierten, von Marketing unterstützten CRM-Systemen korrekt angezeigt. Die CRM-Opportunitätsfelder müssen jedoch den Marketo-Opportunitätsfeldern korrekt zugeordnet werden.

## Ich habe keine anderen Marketing Analytics-Produkte (ARB, RCE, RCA, Programm-Analyse). Wird MPI für mich arbeiten? {#i-do-not-have-any-other-marketing-analytics-products-arb-rce-rca-program-analysis-will-mpi-work-for-me}

MPI ist ein unabhängiges Add-on zur Anwendung &quot;Lead Management&quot;. Die Verwendung anderer Analyseprodukte ist nicht erforderlich.

## RCA zeigt mir auch Leistungsdaten zum Programm. Gibt es einen Unterschied zwischen den in MPI und RCA angezeigten Daten? {#rca-shows-me-program-performance-data-as-well-is-there-a-difference-between-the-data-shown-in-mpi-and-rca}

Anzahl MPI liefert Daten aus demselben Data Warehouse wie RCA. Daher werden keine Datenunterschiede zwischen den beiden angezeigt. Mit RCA können Sie jederzeit eigene Berichte erstellen. MPI ermöglicht Ihnen den Zugriff auf leicht verständliche visuelle Dashboard.

## Ich möchte nicht, dass einige meiner Programm (z.B. Operational) in MPI angezeigt werden. Wie kann ich die Sichtbarkeit bestimmter Programm steuern? {#i-don-t-want-some-of-my-programs-e-g-operational-to-show-up-in-mpi-how-do-i-control-the-visibility-of-specific-programs}

Sie können die Sichtbarkeit Ihrer Programm steuern, indem Sie das Analytics-Verhalten Ihrer Programm auf Operational einstellen. Dadurch wird das Programm aus den Analytics-Berechnungen ausgeschlossen.

>[!NOTE]
>
>Weitere Informationen zum Festlegen des Analyseverhaltens [hier](http://docs.marketo.com/display/public/DOCS/Edit+Analytics+Behavior+Settings).

## Ich führe eine Kampagne mit mehreren Kanälen für einen neuen Produktstart aus. Wie kann ich die Leistung für diese Kampagne an einem Ort an allen verschiedenen Kanälen Ansicht leisten? {#i-am-running-a-multi-channel-campaign-for-a-new-product-launch-how-can-i-view-the-performance-for-this-campaign-across-all-the-different-channels-in-one-place}

Wir empfehlen, dass Sie für Programme, die Teil einer solchen Kampagne sind, Programm-Tags verwenden. Programm-Tags werden automatisch mit MPI synchronisiert und Sie können sie in allen MPI-Dashboards filtern, um die Leistung Ihrer Kampagne mit mehreren Kanälen Ansicht.

## Habe ich Zugriff auf Zuordnungseinstellungen, wenn ich keine RCA habe? {#will-i-have-access-to-attribution-settings-if-i-do-not-have-rca}

Sie erhalten Zugriff auf Zuordnungseinstellungen, wenn Sie MPI haben, unabhängig davon, ob Sie RCA haben oder nicht.

## Ich erhalte eine Warnung in MPI, wenn ich mich anmelde und mir sage, dass meine Zuordnungseinstellungen falsch sind. Was ist los? {#i-get-an-alert-in-mpi-when-i-log-in-telling-me-that-my-attribution-settings-are-incorrect-what-s-wrong}

MPI berechnet, ob alle Ihre Möglichkeiten in die Analyse einbezogen werden. Andernfalls werden Sie aufgefordert, eine Änderung Ihrer Zuordnungseinstellungen (Explizit, Implizit, Hybrid) in Erwägung zu ziehen, um weitere Möglichkeiten einzubeziehen.

Möglicherweise fehlen Ihnen auch Chancen aufgrund der fehlenden Programm-Kosten in Ihren Programmen. Bitte überprüfen Sie das Analytics-Verhalten Ihrer Programm. Sie können:

1. Standard - Das Standardverhalten ist, dass das Programm NUR in MPI enthalten ist, wenn mindestens ein Periodenkosten, auch wenn kein Dollar zugewiesen ist, vorhanden ist.
1. Inklusiv - Mit dieser Option wird sichergestellt, dass das Programm in MPI verfügbar ist, unabhängig davon, ob Sie einen Zeitraumpreis angegeben haben oder nicht.
1. [Operational](http://docs.marketo.com/display/DOCS/Best+Practice%3A+How+to+Organize+your+Programs#BestPractice:HowtoOrganizeyourPrograms-OperationalPrograms)  - Diese Option führt dazu, dass das Programm nicht in MPI angezeigt wird.

>[!NOTE]
>
>Die Zeitkosten **müssen für den Berichte &quot;Erfolg&quot;und &quot;Neue Namen&quot;im Dashboard &quot;Interaktion&quot;eingerichtet werden.** Dieses Dashboard nutzt Period Cost-Daten, um Aggregat-Erfolge und neue Namen zu erhalten. Wenn die Zeitraumkosten nicht eingerichtet sind, wird das Dashboard der Interaktion unabhängig von den oben genannten Analytics-Verhaltenseinstellungen nicht korrekt gemeldet.

## Warum vermisse ich einige Gelegenheiten in MPI? {#why-am-i-missing-some-opportunities-in-mpi}

Zwei wichtige Gründe, aus denen Ihnen möglicherweise Chancen in MPI fehlen, sind:

1. Die Zuordnungseinstellung ist auf Explizit eingestellt, aber den Möglichkeiten sind keine Kontaktrollen zugewiesen.
1. Die Zeitkosten sind in Ihren Programmen nicht inbegriffen.

MPI berechnet, ob alle Ihre Möglichkeiten in die Analyse einbezogen werden. Andernfalls werden Sie aufgefordert, eine Änderung Ihrer Zuordnungseinstellungen (Explizit, Implizit, Hybrid) in Erwägung zu ziehen, um weitere Möglichkeiten einzubeziehen.

Möglicherweise fehlen Ihnen auch Chancen aufgrund der fehlenden Programm-Kosten in Ihren Programmen. Die Warnmeldung wird angezeigt, aber nicht darauf, welche Programm fehlen. Bitte überprüfen Sie Ihre Programm-Einrichtung, um die Kosten zu berücksichtigen und sicherzustellen, dass alle Ihre Programme und Möglichkeiten in MPI enthalten sind.

## Warum werden im Interaktions-Dashboard keine benutzerdefinierten Felder, Opportunity Type und ABM-Filter angezeigt? {#why-do-i-not-see-custom-fields-opportunity-type-and-abm-filters-on-the-engagement-dashboard}

Benutzerdefinierte Felder, Opportunity Type und ABM-Filter sind alle Attribute, die sich auf eine Gelegenheit beziehen. Mit dem Dashboard Interaktion können Sie Ihren Einsatz und Ihre Interessentenakquisition messen, unabhängig davon, ob sie mit einer Gelegenheit verbunden sind oder nicht. Da das Dashboard Interaktion keine Gelegenheit berücksichtigt, gelten die Filter Benutzerdefinierte Felder, Opportunity Type und ABM nicht.

## Ich möchte ein benutzerdefiniertes Feld für Salesforce-Chancen für den Berichte Umsatz anstelle des Standardfelds Salesforce-Opportunity-Betrag verwenden. Wird MPI mir erlauben, das zu tun? {#i-want-to-use-a-custom-salesforce-opportunity-field-for-revenue-reporting-instead-of-the-standard-salesforce-opportunity-amount-field-will-mpi-allow-me-to-do-that}

Ja. [Marketo ](http://docs.marketo.com/cdn-cgi/l/email-protection#b5c6c0c5c5dac7c1f5d8d4c7ded0c1da9bd6dad8) Support kann das Feld &quot;Opportunity Amount&quot;von Marketo in ein benutzerdefiniertes Feld &quot;Salesforce Opportunity&quot;umwandeln, solange der Feldtyp Währung ist. Da MPI auf das Feld &quot;Größe der Marketing-Chance&quot;verweist, kann MPI die Daten aus dem neu zugeordneten Feld Salesforce verwenden.

>[!NOTE]
>
>Nach der Neuzuordnung zeigt MPI die Daten für die Zukunft an. Der historische Betrag wird nicht geändert.

## Kann ich MPI trotzdem verwenden, wenn ich keine Möglichkeiten verwende? {#if-i-don-t-use-opportunities-can-i-still-use-mpi}

MPI ist so konzipiert, dass Sie die Performance des Programms von oben im Trichter bis hin zu den Auswirkungen auf den Umsatz messen können. Wenn Sie keine Chancen nutzen, können Sie trotzdem:

* Leistung der Ansicht Ihrer Programme zur Pflege der Audience.
* Ansicht der Performance Ihrer Interessentenakquise-Programm.
* Ansicht von Kampagnen mit mehreren Kanälen über Programm-Tags.
* Sehen Sie sich die Interaktionstrends der letzten 12 Audiencen an.
* Speichern und exportieren Sie Leistungsdaten in PowerPoint.

## Kann ich den Erfolg von kontobasierten Strategien in MPI messen? {#can-i-measure-the-success-of-account-based-strategies-in-mpi}

Ja. MPI wird mit [Marketo ABM](http://docs.marketo.com/display/DOCS/Account+Based+Marketing+Overview) integriert, um ABM-Konto-Listen nahtlos in MPI zu ziehen. Mit dem ABM-Liste-Filter können Sie die gewünschte ABM-Liste zum Filtern von Daten auswählen.

## Ist die Zuordnung sofort verfügbar, wenn ich MPI kaufe? {#is-attribution-instantly-available-when-i-purchase-mpi}

Die Marketing Attribution Funktionen stehen unseren Kunden zur Verfügung, wenn sie MPI erwerben. Allerdings ist [das richtige Setup](http://docs.marketo.com/x/mRPG) erforderlich, um sicherzustellen, dass Chancen- und Programm-Daten korrekt in MPI fließen.

## Was muss ich tun, um eine Zuordnung einzurichten? {#what-do-i-have-to-do-to-set-up-attribution}

1. Einrichtung von Chancen

   1. Stellen Sie sicher, dass Chancen mit Ihrem CRM-System synchronisiert werden
   1. Wenn Ihre Zuordnungseinstellungen auf Explizit eingestellt sind, stellen Sie sicher, dass Kontaktrollen zu den Möglichkeiten ausgefüllt werden
   1. Es wird empfohlen, die Attributseinstellung auf Hybrid zu ändern
   1. Programm einrichten

      1. Programm-Kosten in Ihre Programm einschließen
      1. Überprüfen Sie das Analyseverhalten, um anzugeben, ob ein Programm in die Analyse einbezogen werden soll.
      1. Festlegen der Erfolgskriterien für jeden Kanal
      1. Personen mit Programmen verbinden

         1. Stellen Sie sicher, dass für jede Person in Ihrer Datenbank Akquise-Programm und Akquise-Datum festgelegt wurden, damit die Zuordnung von First Touch funktioniert.
         1. Stellen Sie sicher, dass Ihre Programm Erfolgsstatus für Personen in Ihrer Datenbank festlegen

>[!TIP]
>
>Alle erforderlichen Einrichtungsschritte werden in [diesem Artikel](http://docs.marketo.com/x/mRPG) beschrieben.

## Was ist der Unterschied zwischen MPI und dem Programm Analyzer? {#whats-the-difference-between-mpi-and-the-program-analyzer}

Mit dem Programm Analyzer können Sie Ihre Programm mit bis zu vier Messwerten vergleichen. Mit MPI können Sie Ihren Kanal- und Programm-Beitrag zu einer bestimmten Metrik wie z. B. &quot;Erfolg&quot;, &quot;Erstellte neue Chancen&quot;usw. analysieren. Sie können auch den 12-monatigen Kanal-Trend basierend auf einer bestimmten Metrik, die Sie ausgewählt haben, Ansicht.

## Was ist der Unterschied zwischen MPI und dem Advanced Report Builder? {#whats-the-difference-between-mpi-and-the-advanced-report-builder}

Der Advanced-Report Builder (auch als RCE bezeichnet) ist für den Self-Service (oder Ad-hoc-Berichte) konzipiert, der in der Regel von Marketing Operations ausgeführt wird. MPI wurde entwickelt, um Marketingfachleuten und Marketingfachleuten einen 1-Klick-Zugriff auf die Performance-Analyse zu gewähren. Es ist eine minimale Einrichtung erforderlich.

## Was ist mit der Option &quot;Vorheriges Jahr&quot;im Datumsfilter des Beitrags passiert? {#what-happened-to-the-previous-year-option-in-contributions-date-filter}

Die Auswahl für &quot;Vorheriges Jahr&quot;wurde vorübergehend entfernt. Sie haben weiterhin die Möglichkeit, die Leistungsdaten des gesamten Jahres mithilfe der Auswahl des benutzerspezifischen Datumsbereichs anzuzeigen.
