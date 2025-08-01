---
unique-page-id: 10096583
description: 'Häufig gestellte  [!DNL Munchkin] : Tracking der nächsten Generation - Marketo-Dokumente - Produktdokumentation'
title: Häufig gestellte  [!DNL Munchkin]  zum Tracking der nächsten Generation
exl-id: 283189ac-c817-479a-b896-91233980608c
feature: Administration, Munchkin Tracking Code
hide: true
hidefromtoc: true
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 0%

---

# Häufig gestellte Fragen zur nächsten Generation [!DNL Munchkin] Tracking {#next-generation-munchkin-tracking-faq}

Wir freuen uns, Ihnen mitteilen zu können, dass wir in Kürze mit einem schrittweisen Rollout unserer Web-Tracking-Technologie der nächsten Generation beginnen werden.

Hier sind die wichtigsten Dinge zu wissen:

* Der Filter „Ist anonym“ der Smart-Liste wird mit unserer Version für das 1. Quartal entfernt (bereits erledigt)
* Wir erhöhen die Anzahl der Web-Ereignisse (Web-Seite besuchen, Link auf Web-Seite geklickt), die wir aufnehmen können
* Ihr [!DNL Munchkin]-Code ändert sich nicht, sodass keine Aktualisierungen auf Ihrer Website erforderlich sind

## Wann wird mein Marketo-Abonnement für [!DNL Munchkin] V2 gelten? {#when-will-my-marketo-subscription-be-on-munchkin-v}

Wir haben noch kein genaues Datum, aber bitte schauen Sie hier wieder nach Updates.

## Muss ich Änderungen an meinem [!DNL Munchkin]-Tracking auf meiner Website vornehmen? {#will-i-need-to-make-any-changes-to-my-munchkin-tracking-on-my-website}

Nein. Der [!DNL Munchkin] Trackingcode bleibt gleich. Ihre Website muss nicht geändert werden.

>[!NOTE]
>
>Diese Änderung wirkt sich nicht auf Web Personalization (Real-Time Personalization) aus. Sie identifiziert weiterhin anonyme und bekannte Web-Besucher und personalisiert Inhalte in Echtzeit für diese Besucher.

## Warum hat Marketo den Filter „Ist anonym“ aus den Smart Lists entfernt? {#why-did-marketo-remove-the-is-anonymous-filter-from-smart-lists}

Wir haben die Art und Weise verändert, wie anonyme Personen mit intelligenten Kampagnen interagieren. Vorher haben sie eine intelligente Kampagne durchlaufen, genau wie bekannte Menschen. Der Filter „Ist anonym“ wurde verwendet, um anzugeben, dass die Kampagne nur von bekannten oder nur anonymen Personen durchlaufen wird.

Mit [!DNL Munchkin] V2 verfolgen wir weiterhin alle anonymen Aktivitäten. Sie können jedoch keine Filter mehr auf anonyme Personen anwenden. Zum Zeitpunkt der Konversion (wenn die Person in Marketo bekannt wird) werden alle Aktivitäten, die bei der Anonymität der Person aufgetreten sind, an das Aktivitätsprotokoll der Person angehängt und durchlaufen zu diesem Zeitpunkt die Kampagnen, für die sie qualifiziert ist.

Wenn Sie diesen Filter bereits in einer Smart-Liste verwenden (z. B. in einer Smart-Kampagne oder einem Bericht), wird er nicht automatisch aus der Smart-Liste entfernt. Weitere Informationen finden Sie unten.

>[!NOTE]
>
>**Trigger**: Besucht die Web-Seite, die Web-Seite ist die Preisseite
>>**Fluss**: Punktzahl ändern +10 und Interessanter Moment
>>**Web**: Seite mit angezeigten Preisen
>
>Bei [!DNL Munchkin] V2 tritt eine anonyme Person, die die Preisseite besucht, nicht sofort in die Kampagne ein. Sobald die anonyme Person bekannt wird, führen wir diese Kampagne auf ihr durch. Sie wird:
>
>* Ergebnis von 10
>
>* Stellen Sie die Web-Seiten-Aktivität auf das richtige Datum ein (wann sie tatsächlich besucht hat).
>
>* Haben Sie einen interessanten Moment für sie protokolliert (mit dem Datum, an dem sie die Seite tatsächlich besucht hat, nicht, als sie bekannt wurde)
>
>* Eine „Neue Person“-Aktivität wie heute protokollieren lassen

## Was passiert mit meinen Smart Lists, die bereits den Filter „Ist anonym“ haben? {#what-happens-to-my-smart-lists-that-already-have-the-is-anonymous-filter}

Wenn Sie nach unserer Winter-Version &#39;16 alte Smart-Kampagnen mit einer Smart-Liste haben, die den Filter „Ist anonym“ enthält, passiert eines von zwei Dingen:

1. Wenn die Smart-Liste den Filter „Ist anonym = Falsch“ aufweist, passiert nichts. Wir werden es einfach ignorieren.
1. Wenn die Smart-Liste den Filter „Ist anonym = True“ aufweist, schlägt diese Kampagne fehl und Sie erhalten eine Benachrichtigung.

## Ich benutze Marketo schon eine Weile. Woher weiß ich, welche meiner Kampagnen den Filter „Ist anonym“ verwenden? {#ive-been-using-marketo-for-a-while-how-do-i-know-which-of-my-campaigns-use-the-is-anonymous-filter}

Bevor wir diese Änderung vorgenommen haben, haben wir mehrere wöchentliche Benachrichtigungen an Ihren Benachrichtigungs-Posteingang gesendet, mit einer Liste von Smart Lists, Smart Kampagnen und Berichten, die den Filter „Ist anonym“ verwenden. Auf diese Weise können Sie feststellen, wo Sie diesen Filter derzeit verwenden.

Bitte überprüfen Sie diese und ermitteln Sie, wo „Ist anonym“ auf „True“ gesetzt ist, da dies die betroffenen Kampagnen sind. In den meisten Fällen verwenden Kunden diese Einstellung für eine Art Scoring. Im obigen Beispiel erfahren Sie, wie diese Kampagnen jetzt funktionieren.

## Ich hätte gerne eine detailliertere Dokumentation. Wo finde ich es? {#id-like-more-detailed-documentation-where-can-i-find-it}

Sehen Sie sich diese Links an:

[Übersicht über anonyme Lead-Upgrades](https://nation.marketo.com/docs/DOC-2937){target="_blank"}

[Anonyme Lead-Upgrades - Änderungen in der Marketo-Benutzeroberfläche](https://nation.marketo.com/docs/DOC-2938){target="_blank"}

[Anonyme Lead-Upgrades - Kundenaktion erforderlich](https://nation.marketo.com/docs/DOC-2939){target="_blank"}

[Anonyme Lead-Upgrades - Analytics-Berichte](https://nation.marketo.com/docs/DOC-2940){target="_blank"}

[Anonyme Lead-Upgrades - Veröffentlichungszeitplan](https://nation.marketo.com/docs/DOC-2961){target="_blank"}

[Anonyme Lead-Upgrades - Unter der Haube](https://nation.marketo.com/docs/DOC-2962){target="_blank"}

[Anonyme Lead-Promotion zum bekannten Lead - [!DNL Munchkin] v2-Verhalten](https://nation.marketo.com/docs/DOC-2963){target="_blank"}

## Ich habe noch weitere Fragen! Wie bekomme ich Antworten? {#i-have-more-questions-how-do-i-get-them-answered}

Bitte kontaktieren Sie die [Community](https://nation.marketo.com/){target="_blank"}. Sie können sich auch an den [Marketo-Support](https://nation.marketo.com/t5/Support/ct-p/Support){target="_blank"} wenden. Sie werden Ihre Fragen gerne beantworten.
