---
unique-page-id: 10096583
description: Nächste Generation [!DNL Munchkin] Häufig gestellte Fragen zum Tracking - Marketo-Dokumente - Produktdokumentation
title: Nächste Generation [!DNL Munchkin] Häufig gestellte Fragen zum Tracking
exl-id: 283189ac-c817-479a-b896-91233980608c
feature: Administration, Munchkin Tracking Code
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 0%

---

# Häufig gestellte Fragen zur Verfolgung der nächsten Generation [!DNL Munchkin] {#next-generation-munchkin-tracking-faq}

Wir freuen uns, Ihnen mitteilen zu können, dass wir bald mit der Einführung unserer Webtrackingtechnologie der nächsten Generation beginnen werden.

Im Folgenden finden Sie die wichtigsten Informationen:

* Wir entfernen den Filter &quot;Ist anonym&quot;für die intelligente Liste mit unserer Version Q1 (bereits abgeschlossen).
* Wir erhöhen die Anzahl der Web-Ereignisse (Webseite besuchen, Link auf Webseite angeklickt), die wir aufnehmen können.
* Ihr [!DNL Munchkin] -Code ändert sich nicht, sodass keine Aktualisierungen auf Ihrer Website erforderlich sind

## Wann wird mein Marketo-Abonnement auf [!DNL Munchkin] V2 sein? {#when-will-my-marketo-subscription-be-on-munchkin-v}

Wir haben noch kein genaues Datum, aber bitte schauen Sie hier zurück, um Updates zu erhalten.

## Muss ich Änderungen an meinem [!DNL Munchkin]-Tracking auf meiner Website vornehmen? {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

Nein. Der Trackingcode für [!DNL Munchkin] bleibt gleich. An Ihrer Website müssen keine Änderungen vorgenommen werden.

>[!NOTE]
>
>Diese Änderung betrifft nicht Web Personalization (Real-Time Personalization). Es identifiziert weiterhin anonyme und bekannte Webbesucher und personalisiert Inhalte in Echtzeit für diese Besucher.

## Warum hat Marketo den Filter &quot;Ist anonym&quot;aus Smart-Listen entfernt? {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

Die Interaktion anonymer Personen mit Smart-Kampagnen wurde geändert. Zuvor flogen sie durch eine intelligente Kampagne, genau wie bekannte Menschen. Der Filter &quot;Ist anonym&quot;wurde verwendet, um anzugeben, dass nur bekannte oder nur anonyme Personen durch die Kampagne fließen.

Mit [!DNL Munchkin] V2 werden wir weiterhin alle anonymen Aktivitäten verfolgen. Sie können jedoch keine Filter mehr auf anonyme Personen anwenden. Zum Zeitpunkt der Konversion (wenn die Person in Marketo bekannt wird) werden alle Aktivitäten, die zum Zeitpunkt der Anonymität der Person aufgetreten sind, an das Personen-Aktivitätsprotokoll angehängt und durchlaufen zu diesem Zeitpunkt die Kampagnen, für die sie qualifiziert ist.

Wenn Sie diesen Filter bereits in einer Smart-Liste verwenden (z. B. in einer Smart-Kampagne oder einem Bericht), wird er nicht automatisch aus der Smart-Liste entfernt. Weitere Informationen finden Sie unten.

>[!NOTE]
>
>**Trigger**: Besuche der Webseite, Webseite ist Preisseite\
>**Fluss**: Wert +10 ändern und interessanten Moment
>**Web**: Angesehene Preisseite
>
>Wenn eine anonyme Person bei [!DNL Munchkin] V2 die Preisseite besucht, tritt sie nicht sofort in die Kampagne ein. Sobald die anonyme Person bekannt wird, führen wir diese Kampagne auf sie aus. Sie wird:
>
>* 10 Punkte abrufen
>
>* Setzen Sie die Aktivität Webseite auf das richtige Datum (wenn sie die Seite tatsächlich besucht hat)
>
>* Sie haben einen interessanten Moment für sie protokolliert (mit dem Datum, an dem sie die Seite tatsächlich besucht hat, nicht, an dem sie bekannt wurde).
>
>* Lassen Sie die Aktivität &quot;Neue Person&quot;wie heute protokolliert.

## Was passiert mit meinen Smart-Listen, die bereits den Filter &quot;Ist anonym&quot;haben? {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

Nach unserer Winterversion 16 werden, wenn Sie alte Smart-Kampagnen mit einer Smart-Liste haben, in der der Filter &quot;Ist anonym&quot;enthalten ist, eine von zwei Dingen passieren:

1. Wenn die Smart-Liste den Filter &quot;Is Anonymous = False&quot;enthält, wird nichts geschehen. Wir werden es einfach ignorieren.
1. Wenn die Smart-Liste den Filter &quot;Is Anonymous = True&quot;aufweist, schlägt diese Kampagne fehl und Sie erhalten eine Benachrichtigung.

## Ich benutze Marketo schon eine Weile. Woher weiß ich, welche meiner Kampagnen den Filter &quot;Ist anonym&quot; verwenden? {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

Bevor wir diese Änderung vorgenommen haben, haben wir mehrere wöchentliche Benachrichtigungen an Ihren Benachrichtigungs-Posteingang mit einer Liste von Smart-Listen, Smart-Kampagnen und Berichten gesendet, die den Filter &quot;Ist anonym&quot;verwenden. Diese können Ihnen dabei helfen, herauszufinden, wo Sie diesen Filter derzeit verwenden.

Überprüfen Sie sie und identifizieren Sie, wo &quot;Is Anonymous&quot;auf True festgelegt ist, da dies die betroffenen Kampagnen sind. Meistens verwenden Kunden diese Einstellung für eine Art Scoring. Im obigen Beispiel erfahren Sie, wie diese Kampagnen jetzt funktionieren.

## Ich hätte gern eine detailliertere Dokumentation. Wo kann ich es finden? {#id-like-more-detailed-documentation-where-can-i-find-it}

Sehen Sie sich diese Links an:

[Anonyme Lead-Upgrades - Überblick](https://nation.marketo.com/docs/DOC-2937){target="_blank"}

[Anonyme Lead-Upgrades - Änderungen innerhalb der Marketo-Benutzeroberfläche](https://nation.marketo.com/docs/DOC-2938){target="_blank"}

[Anonyme Lead-Upgrades - Kundenaktion erforderlich](https://nation.marketo.com/docs/DOC-2939){target="_blank"}

[Anonyme Lead-Upgrades - Analytics-Berichte](https://nation.marketo.com/docs/DOC-2940){target="_blank"}

[Anonyme Lead-Upgrades - Veröffentlichungszeitplan](https://nation.marketo.com/docs/DOC-2961){target="_blank"}

[Anonyme Lead-Upgrades - unter dem Hood](https://nation.marketo.com/docs/DOC-2962){target="_blank"}

[Anonyme Lead-Promotion zu bekanntem Lead - [!DNL Munchkin] V2-Verhalten](https://nation.marketo.com/docs/DOC-2963){target="_blank"}

## Ich habe mehr Fragen! Wie bekomme ich Antworten? {#i-have-more-questions-how-do-i-get-them-answered}

Bitte kontaktieren Sie die [Community](https://nation.marketo.com/){target="_blank"}. Sie können sich auch an den [Marketo-Support](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"} wenden. Sie werden sich freuen, Ihre Fragen zu beantworten.
