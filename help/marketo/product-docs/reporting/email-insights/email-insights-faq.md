---
unique-page-id: 10100257
description: E-Mail Insights FAQ - Marketing Docs - Produktdokumentation
title: Häufig gestellte Fragen zu E-Mail Insights
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---


# Häufig gestellte Fragen zu E-Mail Insights {#email-insights-faq}

## Gibt es Unterschiede zwischen den Quotientenmetriken mit E-Mail-Insight und anderen Marketing-E-Mail-Berichten? {#are-there-any-differences-between-ratio-metrics-with-email-insights-and-other-marketo-email-reporting}

Ja. E-Mail-Einblicke korrelieren Interaktionsmetriken mit den entsprechenden Metriken für den Versand derselben E-Mail, die gesendet wird, wenn die Metrik für Interaktionen berechnet wird (Offene Rate, Klicks zu Offenheit, Abmelderate). In E-Mail-Insights wird beispielsweise bei der Betrachtung eines Zeitreihendiagramms der letzten Woche mit täglichen Aufschlüsselungen der Klickrate zu Open-Rate nun das tatsächliche korrelierte Verhältnis von Ereignissen mit &quot;open/click/unsubscribe&quot;basierend auf den entsprechenden Versand-Metriken angezeigt. Dies steht im Gegensatz zu dem Verhalten im Revenue Explorer, der einfach alles zusammenfasst. Email Insights bietet eine genauere Ansicht der Interaktionsverhältnisse.

## Warum unterstützt Email Insights nur 10 benutzerspezifische Dimensionen? {#why-does-email-insights-only-support-custom-dimensions}

Bei vielen Anwendungsfällen ist die Erweiterung der Standardsystemabmessungen um 10 zusätzliche benutzerdefinierte Dimensionen mehr als ausreichend und umfasst benutzerdefinierte Dimensionen, die auf Segmenten oder Programm-Tags basieren. In Zukunft planen wir, Kunden die Möglichkeit zu geben, die Anzahl der zulässigen benutzerspezifischen Dimensionen zu erhöhen.

## Warum kann ich benutzerdefinierte Dimensionen-Slots nicht erneut verwenden, nachdem sie zugewiesen wurden? {#why-cant-i-re-use-custom-dimensions-slots-after-theyve-been-assigned}

Wenn ein bestimmter Benutzerdefinierter Dimension-Slot zugewiesen wurde, führt eine Neuzuordnung dazu, dass frühere Daten einen Fehler verursachen, wenn sie mit einer neuen Bedeutung gemischt werden. Aus diesem Grund werden Benutzerdefinierte Dimension-Slots möglicherweise nicht wiederverwendet. Dieses Verhalten entspricht dem anderer Tools zur Analyse von Metriken, wie Google Analytics.

## Unterstützt E-Mail Insights E-Mails zu MarketingTo Sales Insight? {#does-email-insights-support-marketo-sales-insight-emails}

Ja. Alle E-Mails, die über Marketo Sales Insights gesendet werden, sind in Email Insights enthalten.

## Unterstützt Email Insights operative E-Mails? {#does-email-insights-support-operational-emails}

Ja. Standardmäßig werden operative E-Mails vor Ansicht und Abfrage ausgeblendet. Sie können diese Einstellung jedoch im Bedienfeld &quot;Persönliche Einstellungen&quot;ändern.

## Erfasst E-Mail-Insights wiederkehrende geplante oder erneut ausgeführte E-Mail-Flusstests für intelligente Kampagnen? {#does-email-insights-capture-recurring-scheduled-or-re-run-smart-campaign-email-flow-steps}

Ja und Nein. Mit der ersten Version von Email Insights werden alle E-Mail-Ereignis erfasst und stehen für alle geplanten oder erneut ausgeführten Smart-Kampagnen zur Verfügung. Aber man kann nicht zwischen verschiedenen Phasen dieser intelligenten Kampagne unterscheiden. In unserer nächsten Version unterstützen wir Sie bei der Erfassung der Informationen zum Ausführen der Smart-Kampagne für Ereignis zum Öffnen, Klicken und Abmelden, um eine Unterscheidung zu treffen.

## Warum zeigen viele Metriken null an, wenn ich nach Gerätetyp oder Gerätebetriebssystem filtere? {#why-do-many-metrics-show-zero-when-i-filter-by-device-type-or-device-os}

Mit Ausnahme von &quot;Click-to-Open Rate&quot;, &quot;Open&quot;, &quot;Clicks&quot;und &quot;Unsubscribes&quot;sind alle anderen unterstützten Metriken entweder Versand-Ereignis oder Quotienten, die von Versand-Ereignissen abgeleitet werden. Da Gerätetyp und Gerätebetriebssystem nur für Interaktionsmetriken gelten, verfügen wir einfach nicht über die anzuzeigenden Informationen. Beispielsweise ist es eine nicht definierte Abfrage, die nach Gerätetyp = mobil gefiltert wird, um die Besucherrate anzufordern, da Marketing keine Interaktionsmetriken für den zugrunde liegenden Versand und die gesendeten Ereignis erhalten hätte. Wir erforschen Möglichkeiten, den Gerätetyp und das Gerätebetriebssystem aus Interaktionsmetriken für Quotienten aus Interaktions- und Versand-Metriken anzuwenden.

## Was macht E-Mail-Insight, wenn bestimmte E-Mail-Clients Bilder blockieren? {#what-does-email-insights-do-when-certain-email-clients-block-images}

Ein allgemeines Industrieproblem ist, dass immer mehr E-Mail-Clients Bilder standardmäßig deaktivieren. Das Laden von Bildern ist die Grundlage für die Aufzeichnung von &quot;Öffnen&quot;. Es ist durchaus möglich, dass ein Benutzer eine E-Mail mit blockierten Bildern erhält, aber der Text und die Links vollständig lesbar sind. Wenn ein Benutzer dies erlebt und auf einen Link in dieser E-Mail geklickt hat, erhalten Sie am Ende ein Click-Ereignis, jedoch kein entsprechendes Open Ereignis für diese E-Mail. Marketo E-Mail Insights generiert automatisch alle fehlenden Ereignis. Die Logik ist identisch mit der, wie Marketo dies für den Bericht &quot;E-Mail-Leistung&quot;und den Bereich &quot;E-Mail-Analyse&quot;im Umsatz-Explorer tut.
