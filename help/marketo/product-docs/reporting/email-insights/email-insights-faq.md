---
unique-page-id: 10100257
description: Häufig gestellte Fragen zu E-Mail-Einblicken - Marketo-Dokumente - Produktdokumentation
title: Häufig gestellte Fragen zu E-Mail-Einblicken
exl-id: de3aca5a-08b4-4af8-ab92-675cb46dcbb2
feature: Reporting
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Häufig gestellte Fragen zu E-Mail-Einblicken {#email-insights-faq}

## Gibt es Unterschiede zwischen Verhältnismetriken mit E-Mail-Einblicken und anderen E-Mail-Berichten in Marketo? {#are-there-any-differences-between-ratio-metrics-with-email-insights-and-other-marketo-email-reporting}

Ja. E-Mail-Insights korreliert Interaktionsmetriken mit den entsprechenden Versandmetriken für dieselbe E-Mail, die bei der Berechnung der Interaktionsmetrikverhältnisse gesendet wurde (Öffnungsrate, Klickrate zum Öffnen, Abmelderate). Beispiel: In E-Mail-Einblicken zeigen wir jetzt bei der Betrachtung eines Zeitreihendiagramms der letzten Woche mit täglichen Aufschlüsselungen der Klick-zu-Öffnen-Rate das tatsächliche korrelierte Verhältnis von Öffnungs-/Klick-/Abmelde-Ereignissen, basierend auf den entsprechenden Versandmetriken. Dies steht im Gegensatz zum Verhalten im Revenue Explorer, der einfach alles zusammenfasst. E-Mail-Einblicke bieten eine genauere Ansicht der Interaktionsraten.

## Warum unterstützt Email Insights nur 10 benutzerdefinierte Dimensionen? {#why-does-email-insights-only-support-custom-dimensions}

Für viele Anwendungsfälle ist die Erweiterung der standardmäßigen Systemdimensionen um 10 zusätzliche benutzerdefinierte Dimensionen mehr als ausreichend. Sie enthält benutzerdefinierte Dimensionen, die auf Segmentierungen oder Programm-Tags basieren. In Zukunft planen wir, es Kunden zu ermöglichen, die Anzahl der zulässigen benutzerdefinierten Dimensionen zu erhöhen.

## Warum kann ich die Slots für benutzerdefinierte Dimensionen nicht wiederverwenden, nachdem sie zugewiesen wurden? {#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

Nachdem ein bestimmter Steckplatz für benutzerdefinierte Dimensionen zugewiesen wurde, würde eine Neuzuordnung dazu führen, dass vorherige Daten einen Fehler erzeugen, wenn sie mit einer neuen Bedeutung vermischt werden. Aus diesem Grund können Steckplätze für benutzerdefinierte Dimensionen nicht wiederverwendet werden. Dieses Verhalten stimmt mit dem anderer Metrikanalyse-Tools wie Google Analytics überein.

## Unterstützt Email Insights E-Mails mit Verkaufserkenntnissen aus Marketo? {#does-email-insights-support-marketo-sales-insight-emails}

Ja. Alle über Marketo Sales Insights gesendeten E-Mails sind in E-Mail-Insights enthalten.

## Unterstützt Email Insights operative E-Mails? {#does-email-insights-support-operational-emails}

Ja. Standardmäßig werden operative E-Mails nicht angezeigt und abgefragt. Sie können diese Einstellung jedoch im Bedienfeld Persönliche Einstellungen ändern.

## Erfasst Email Insights wiederkehrende geplante oder erneut ausgeführte E-Mail-Flussschritte von Smart Campaign? {#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

Ja und Nein. Mit der ersten Veröffentlichung von E-Mail-Einblicken werden alle E-Mail-Ereignisse erfasst und sind für alle wiederkehrenden geplanten oder erneuten Ausführungen von Smart Campaign verfügbar. Sie werden jedoch nicht zwischen den verschiedenen Ausführungen dieser intelligenten Kampagne unterscheiden können. In unserer nächsten Version wird Unterstützung hinzugefügt, um die Informationen zum Ausführen von Smart Campaign für Öffnungs-, Klick- und Abmeldeereignisse zu erfassen und so zu unterscheiden.

## Warum wird bei vielen Metriken null angezeigt, wenn ich nach Gerätetyp oder Gerätebetriebssystem filtere? {#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

Mit Ausnahme der Klicks-zum-Öffnen-Rate, Öffnungen, Klicks und Abmeldungen sind alle anderen unterstützten Metriken entweder Versandereignisse oder Verhältnisse, die von Versandereignissen abgeleitet wurden. Da Gerätetyp und Gerätebetriebssystem nur für Interaktionsmetriken gelten, verfügen wir einfach nicht über die anzuzeigenden Informationen. Beispielsweise ist es eine undefinierte Abfrage, nach der Versandrate zu fragen, wenn sie nach Gerätetyp = Mobiltelefon gefiltert wird, da Marketo keine Interaktionsmetriken für die zugrunde liegenden Versand- und Gesendetereignisse erhalten hätte. Wir untersuchen Möglichkeiten, den Gerätetyp und das Gerätebetriebssystem aus Interaktionsmetriken für Verhältnisse anzuwenden, die sowohl Interaktions- als auch Bereitstellungsmetriken umfassen.

## Was bewirkt Email Insights, wenn bestimmte E-Mail-Clients Bilder blockieren? {#what-does-email-insights-do-when-certain-email-clients-block-images}

Ein häufiges Branchenproblem ist die wachsende Anzahl von E-Mail-Clients, die Bilder standardmäßig deaktivieren. Das Laden von Bildern ist die Grundlage für die Aufzeichnung von Öffnungen. Es ist durchaus möglich, dass ein Benutzer eine E-Mail mit blockierten Bildern erhält, jedoch mit vollständig lesbarem Text und Links. Wenn dies ein Benutzer erlebt hat und auf einen Link in dieser E-Mail geklickt hat, erhalten Sie ein Szenario mit einem Klick-Ereignis, aber kein entsprechendes Öffnen-Ereignis für diese E-Mail. Marketo Email Insights generiert automatisch alle Ereignisse, die fehlten. Die Logik entspricht der Vorgehensweise von Marketo im E-Mail-Leistungsbericht sowie im Bereich E-Mail-Analyse im Umsatz-Explorer.
