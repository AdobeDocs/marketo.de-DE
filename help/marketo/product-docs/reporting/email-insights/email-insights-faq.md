---
unique-page-id: 10100257
description: Häufig gestellte Fragen zu Email Insights - Marketo-Dokumente - Produktdokumentation
title: Häufig gestellte Fragen zu E-Mail-Insights
exl-id: de3aca5a-08b4-4af8-ab92-675cb46dcbb2
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# Häufig gestellte Fragen zu E-Mail-Insights {#email-insights-faq}

## Gibt es Unterschiede zwischen den Quotenmetriken mit E-Mail-Insights und anderen Marketo-E-Mail-Berichten? {#are-there-any-differences-between-ratio-metrics-with-email-insights-and-other-marketo-email-reporting}

Ja. E-Mail-Insights ordnet Interaktionsmetriken den entsprechenden Versandmetriken für dieselbe E-Mail zu, die gesendet wird, wenn Interaktionsmetrikverhältnisse berechnet werden (Öffnungsrate, Klickrate, Abmelderate). Wenn Sie beispielsweise in E-Mail-Insights ein Zeitreihendiagramm der letzten Woche mit täglichen Aufschlüsselungen der Klickrate zur Offline-Rate betrachten, wird jetzt das tatsächliche korrelierte Verhältnis zwischen Öffnungs-/Klick-/Abmeldeereignissen basierend auf den entsprechenden Versandmetriken angezeigt. Dies steht im Gegensatz zum Verhalten im Umsatz-Explorer, der einfach alles zusammenfasst. Email Insights bietet eine genauere Ansicht der Interaktionsverhältnisse.

## Warum unterstützt Email Insights nur 10 benutzerspezifische Dimensionen? {#why-does-email-insights-only-support-custom-dimensions}

Für viele Anwendungsfälle ist die Erweiterung der standardmäßigen Systemdimensionen um 10 zusätzliche benutzerdefinierte Dimensionen mehr als ausreichend und umfasst benutzerdefinierte Dimensionen, die auf Segmentierungen oder Programm-Tags basieren. In Zukunft wird geplant, Kunden zu erlauben, die Anzahl der zulässigen benutzerdefinierten Dimensionen zu erhöhen.

## Warum kann ich benutzerdefinierte Dimension-Slots nicht erneut verwenden, nachdem sie zugewiesen wurden? {#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

Nachdem ein bestimmter Benutzerdefinierter Dimension-Slot zugewiesen wurde, führt eine Neukodifizierung dazu, dass frühere Daten einen Fehler auslösen, wenn sie mit einer neuen Bedeutung gemischt werden. Aus diesem Grund können benutzerdefinierte Dimension-Slots möglicherweise nicht wiederverwendet werden. Dieses Verhalten entspricht dem anderer Metrikanalysetools wie Google Analytics.

## Unterstützt Email Insights Marketo Sales Insight-E-Mails? {#does-email-insights-support-marketo-sales-insight-emails}

Ja. Alle E-Mails, die über Marketo Sales Insights gesendet werden, sind in Email Insights enthalten.

## Unterstützt Email Insights operative E-Mails? {#does-email-insights-support-operational-emails}

Ja. Standardmäßig werden operative E-Mails für Ansicht und Abfrage ausgeblendet. Sie können diese Einstellung jedoch im Bedienfeld Persönliche Einstellungen ändern.

## Erfasst E-Mail-Insights wiederkehrende geplante oder erneut ausgeführte E-Mail-Flow-Schritte für Smart-Campaign? {#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

Ja und Nein. Mit der ersten Version von Email Insights werden alle E-Mail-Ereignisse erfasst und für wiederkehrende geplante oder erneut ausgeführte Smart-Kampagnen verfügbar gemacht. Sie können jedoch nicht zwischen verschiedenen Phasen dieser Smart-Kampagne unterscheiden. Wir fügen in unserer nächsten Version Unterstützung hinzu, um die Ausführungsinformationen für Smart-Campaign für Öffnungen, Klicks und Abmeldungen zu erfassen, um eine Differenzierung vorzunehmen.

## Warum zeigen viele Metriken null an, wenn ich nach Gerätetyp oder Gerätebetriebssystem filtere? {#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

Mit Ausnahme der Klicks-zu-Öffnungen-Rate, Öffnungen, Klicks und Abmeldungen sind alle anderen unterstützten Metriken entweder Versandereignisse oder Verhältnisse, die von Versandereignissen abgeleitet wurden. Da Gerätetyp und Gerätebetriebssystem nur für Interaktionsmetriken gelten, verfügen wir einfach nicht über die anzuzeigenden Informationen. Beispielsweise ist es eine nicht definierte Abfrage, die nach der Versandrate nach Gerätetyp = Mobiltelefon gefiltert wird, da Marketo keine Interaktionsmetriken für die zugrunde liegenden Bereitstellungs- und Versandereignisse erhalten hätte. Wir erkunden, wie Sie den Gerätetyp und das Betriebssystem von den Interaktionsmetriken für Quotienten aus Interaktionsmetriken und Bereitstellungsmetriken anwenden können.

## Was macht Email Insights, wenn bestimmte E-Mail-Clients Bilder blockieren? {#what-does-email-insights-do-when-certain-email-clients-block-images}

Ein häufig auftretendes Problem in der Branche ist, dass immer mehr E-Mail-Clients standardmäßig Bilder deaktivieren. Das Laden von Bildern bildet die Grundlage für die Aufzeichnung von Öffnungen. Es ist durchaus möglich, dass ein Benutzer eine E-Mail mit blockierten Bildern erhält, der Text und die Links jedoch vollständig lesbar sind. Wenn ein Benutzer dies erlebt und auf einen Link in dieser E-Mail geklickt hat, erhalten Sie das Szenario eines Klickereignisses, aber kein entsprechendes Open-Ereignis für diese E-Mail. Marketo Email Insights generiert automatisch alle fehlenden Ereignisse. Die Logik entspricht der Leistung von Marketo für den Bericht E-Mail-Leistung sowie für den Bereich E-Mail-Analyse im Umsatz-Explorer.
