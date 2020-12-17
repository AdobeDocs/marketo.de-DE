---
unique-page-id: 10096583
description: Häufig gestellte Fragen zur Munchkin-Verfolgung der nächsten Generation - Marketo Docs - Produktdokumentation
title: Häufig gestellte Fragen zur Munchkin-Verfolgung der nächsten Generation
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 0%

---


# Nächste Generation Munchkin Tracking FAQ {#next-generation-munchkin-tracking-faq}

Wir freuen uns, Ihnen mitteilen zu können, dass wir bald mit der Einführung unserer Web-Tracking-Technologie der nächsten Generation beginnen werden.

Hier sind die wichtigsten Dinge zu wissen:

* Wir entfernen den Filter &quot;Ist anonym&quot; für intelligente Listen mit unserer Q1-Version (bereits fertig).
* Wir erhöhen die Anzahl der Web-Ereignisse (Webseite besuchen, Link auf Webseite anklicken), die wir erfassen können
* Ihr Munchkin-Code wird sich nicht ändern, sodass keine Aktualisierungen auf Ihrer Website erforderlich sind

## Wann wird mein Marketo-Abonnement auf Munchkin V2 sein? {#when-will-my-marketo-subscription-be-on-munchkin-v}

Wir haben noch kein genaues Datum, aber bitte schauen Sie hier nach, um Updates zu erhalten.

## Muss ich Änderungen an meiner Munchkin-Verfolgung auf meiner Website vornehmen? {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

Anzahl Der Munchkin-Trackingcode bleibt gleich. An Ihrer Website müssen keine Änderungen vorgenommen werden.

>[!NOTE]
>
>Diese Änderung hat keine Auswirkungen auf die Web-Personalisierung (Echtzeit-Personalisierung). Es identifiziert weiterhin anonyme und bekannte Web-Besucher und personalisiert Inhalte in Echtzeit für diese Besucher.

## Warum hat Marketo den Filter &quot;Ist anonym&quot;aus Smart-Listen entfernt? {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

Wir haben verändert, wie anonyme Menschen mit intelligenten Kampagnen interagieren. Früher flogen sie durch eine kluge Kampagne, genau wie bekannte Menschen. Der Filter &quot;Ist anonym&quot;wurde verwendet, um anzugeben, dass nur bekannte oder nur anonyme Personen durch die Kampagne fließen.

Mit Munchkin V2 werden wir weiterhin alle anonymen Aktivitäten verfolgen; Sie können jedoch keine Filter mehr auf anonyme Personen anwenden. Beim Zeitpunkt der Konversion (wenn die Person in Marketo bekannt wird) werden alle Aktivitäten, die beim Anonymisieren der Aktivität aufgetreten sind, an das Personenprotokoll angehängt und durchlaufen die Kampagnen, für die sie sich qualifizieren.

Wenn Sie diesen Filter bereits in einer Smart-Liste verwenden (z. B. in einer Smart-Kampagne oder einem Bericht), wird er nicht automatisch aus der Smart-Liste entfernt. Weitere Informationen finden Sie unten.

>[!NOTE]
>
>**Beispiel**
>
>**Auslöser**: Besuche Webseite, Webseite ist Preisseite\
>**Fluss**: Change Score +10 und Interest Moment,  **Web**: Angezeigte Preisseite
>
>Bei Munchkin V2 gibt eine anonyme Person, die die Preisseite besucht, nicht sofort die Kampagne ein. Sobald die anonyme Person bekannt wird, führen wir diese Kampagne auf sie. Sie wird:
>
>* Ergebnis: 10
   >
   >
* Stellen Sie die Aktivität der Webseite auf das richtige Datum ein (wenn sie tatsächlich besucht wird)
   >
   >
* Sie haben einen interessanten Moment für sie protokolliert (mit dem Datum, an dem sie die Seite tatsächlich besuchte, nicht, als sie bekannt wurde)
   >
   >
* Protokollieren Sie die Aktivität &quot;Neue Person&quot;, wie es heute der Fall ist

>



## Was passiert mit meinen intelligenten Listen, die bereits den Filter &quot;Ist anonym&quot;haben? {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

Nach unserer Winterversion &#39;16, wenn Sie alte Smart-Kampagnen mit einer Smart-Liste haben, die den Filter &quot;Ist anonym&quot; enthält, passiert eines von zwei Dingen:

1. Wenn die intelligente Liste den Filter &quot;Ist anonym = falsch&quot;hat, passiert nichts. Wir werden es einfach ignorieren.
1. Wenn die Smart-Liste über den Filter &quot;Ist anonym = true&quot;verfügt, schlägt diese Kampagne fehl und Sie erhalten eine Benachrichtigung.

## Ich benutze Marketo schon eine Weile. Woher weiß ich, welche meiner Kampagnen den Filter &quot;Ist anonym&quot; verwenden? {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

Bevor wir diese Änderung vorgenommen haben, haben wir mehrere wöchentliche Benachrichtigungen mit einer Liste von Smart-Listen, Smart-Kampagnen und Berichten, die den Filter &quot;Ist anonym&quot;verwenden, an Ihren Posteingang gesendet. Diese können Ihnen dabei helfen, herauszufinden, wo Sie diesen Filter derzeit verwenden.

Bitte überprüfen Sie sie und identifizieren Sie, wo &quot;Ist anonym&quot;auf &quot;True&quot;gesetzt ist, da dies die betroffenen Kampagnen sind. Meistens verwenden Kunden diese Einstellung für eine Art Bewertung. Sehen Sie sich das obige Beispiel an, um zu verstehen, wie diese Kampagnen jetzt funktionieren.

## Ich hätte gern eine detailliertere Dokumentation. Wo kann ich es finden? {#id-like-more-detailed-documentation-where-can-i-find-it}

Sehen Sie sich die folgenden Links an:

[Übersicht über Anonyme Lead-Upgrades](https://nation.marketo.com/docs/DOC-2937)

[Anonyme Lead-Upgrades - Änderungen in der Benutzeroberfläche von Marketing](https://nation.marketo.com/docs/DOC-2938)

[Anonyme Lead-Upgrades - Kundenaktion erforderlich](https://nation.marketo.com/docs/DOC-2939)

[Anonyme Lead-Upgrades - Analytics-Berichte](https://nation.marketo.com/docs/DOC-2940)

[Anonyme Lead-Upgrades - Versionsplan](https://nation.marketo.com/docs/DOC-2961)

[Anonyme Lead-Upgrades - unter dem Menüpfad](https://nation.marketo.com/docs/DOC-2962)

[Anonyme Interessentenwerbung zu bekanntem Interessent - Munchkin V2-Verhalten](https://nation.marketo.com/docs/DOC-2963)

## Ich habe mehr Fragen! Wie kann ich sie beantworten? {#i-have-more-questions-how-do-i-get-them-answered}

Bitte kontaktieren Sie die [community](https://nation.marketo.com/welcome). Sie können auch eine E-Mail an [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#4c3f393c3c233e380c212d3e27293823622f232162) senden. Sie werden Ihre Fragen gerne beantworten.
