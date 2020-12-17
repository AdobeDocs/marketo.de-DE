---
unique-page-id: 12983280
description: Versionshinweise - Herbst 17 - Marketing Docs - Produktdokumentation
title: Versionshinweise - Herbst 17
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---


# Versionshinweise: Fall &#39;17 {#release-notes-fall}

Die folgenden Funktionen sind in der Version Herbst 17 enthalten. Überprüfen Sie Ihre Marketo-Edition auf Funktionsverfügbarkeit.

Bitte klicken Sie auf die Titellinks, um detaillierte Ansichten zu den einzelnen Funktionen anzuzeigen. Hinweis: Einige der in dieser Version enthaltenen Funktionen verfügen nicht über zugehörige Artikel. Wenn ein Thema mehrere Unterüberschriften enthält, werden die Links dort platziert.

## Systemzuverlässigkeit {#system-reliability}

Wir haben die Kerninfrastruktur von Marketo weiter verbessert, einschließlich einer besseren Sequenzierung, weniger Diskrepanzen und verbesserter Munchkin-Stabilität.

## SFDC-Synchronisierungsleistung {#sfdc-sync-performance}

Profitieren Sie von einer umfangreicheren und schnelleren Synchronisierung über Marketo und Salesforce. Datenänderungen, die Massenaktualisierungen bei Konten oder Interessenten erfordern, können in parallele Warteschlangen aufgeteilt werden, um Rückstände zu vermeiden. Ereignisse und Aufgaben werden jetzt auch bis zu 50 % schneller synchronisiert.

## Leistungsverbesserungen bei Analytics {#analytics-performance-improvements}

Die jüngsten Infrastrukturverbesserungen haben Angebot zu höherer Betriebszeit und Stabilität in den Marketing Berichte- und Analysetools geführt, sodass Sie schneller Ad-hoc-Berichte erstellen können.

## [Zeitzone des Empfängers](https://docs.marketo.com/x/_xvG) {#recipient-time-zone}

Mit dieser neuen Funktion können Sie jetzt E-Mails gemäß den örtlichen Zeitzonen speichern und senden. E-Mail- und Interaktions-Programm können so konfiguriert werden, dass sie in den Zeitzonen der Empfänger ausgeliefert werden, sodass nicht mehr mehrere Programm erstellt werden müssen. Einmalig senden und Marketo hält die E-Mail bis zur richtigen Ortszeit automatisch ab. Steigern Sie E-Mail-Metriken, beachten Sie lokale Praktiken und sparen Sie Zeit, indem Sie ein einzelnes Programm global verwenden.

![](assets/image2017-11-29-8-3a45-3a47.png)

>[!NOTE]
>
>Wenn Sie die Zeitzone des Empfängers noch nicht in Ihren E-Mail- und Interaktions-Programmen aktivieren können, sollten Sie sich nicht panisch verhalten! Diese Funktion wird schrittweise allen Kunden zur Verfügung gestellt.

## [Beispiel-E-Mails nach Segment überprüfen](https://docs.marketo.com/x/2IER) {#review-sample-emails-by-segment}

Marketo verfügt über eine neue Option, um ein Segment auszuwählen, wenn E-Mails zum Review gesendet werden. Sie müssen nicht mehr manuell festlegen, zu welchem Segment ein Interessent gehört, sodass es einfacher ist, E-Mails mit dynamischen Inhalten an verschiedene Segmente zu senden.

## [LinkedIn-Interessentenanwerbung - Benutzerspezifische Fragen](https://docs.marketo.com/x/ngLG) {#linkedin-lead-gen-custom-questions}

Passen Sie Ihre LinkedIn-Lead-Gen-Formulare an, um benutzerdefinierte Interessentenattribute zu erfassen. Sie können jetzt bis zu drei benutzerspezifische Fragen pro Formular stellen, aus einer einzeiligen Texteingabe oder Fragen mit mehreren Auswahlmöglichkeiten wählen und wieder Marketo-Interessentenfelder zuordnen.

## [Slack-Integration](../../product-docs/administration/additional-integrations/add-slack-as-a-launchpoint-service.md) {#slack-integration}

Im Rahmen der neuen Slack-Integration haben wir zwei Funktionen veröffentlicht:

* Systembenachrichtigungen: Erhalten Sie Benachrichtigungen über wichtige Ereignis in Ihrer Marketo-Instanz, z. B. Warnungen über den Status der aktuellen Kampagne und alle Probleme, die sofortige Aufmerksamkeit erfordern.
* Interessante Momente: Wenn ein Marketo Insight von einer bekannten Person aus einem Kundenkonto ausgelöst wurde, können Interessenteninhaber per Slack benachrichtigt werden. Benachrichtigungen enthalten Interessenteninformationen sowie Details zum Kundenkonto.

## ABM-Erweiterungen {#abm-enhancements}

** [Konten ohne Kontakte anzeigen](https://docs.marketo.com/x/fKCt)**

Marketo ABM synchronisiert und zeigt CRM-Konten ohne Kontakte an. Schließen Sie neue Konten ohne vorherigen Verkauf oder Marketingverlauf ein und verfolgen Sie den Fortschritt, indem Sie nachfolgende Interessenten zu den Konten abgleichen.

## Inhalt`<sup>AI </sup>`Analytics {#contentai-analytics}

** [Neue ABM-Kontofilter-Liste](https://docs.marketo.com/x/1BPG) **

Ansicht und Vergleich der Content-Performance über ABM-Listen hinweg, um vorhandene Inhalte zu optimieren. Inhalt`<sup>AI</sup>` zeigt Ihnen:

* Hauptinhalt angezeigt
* Top-konvertierte Inhalte
* AI-basierte vorgeschlagene Inhalte für Marketing-Aktivitäten

## Web-Personalisierungsverbesserungen {#web-personalization-enhancements}

** [Tokens für Web-Kampagnen](https://docs.marketo.com/x/SwJI)**

Token stehen jetzt zur Verwendung in Web-Kampagnen zur Verfügung. Nutzen Sie Token, um personalisierte Nachrichten und Inhalte bereitzustellen, um die Interaktion mit Ihren Web-Kampagnen zu steigern.

![](assets/image2017-11-16-11-3a25-3a7.png)

** [Design Studio Images in Web Kampagne Editor](https://docs.marketo.com/x/SwJI)**

Sparen Sie Zeit, indem Sie kreative Assets und Bilder in mehreren Kanälen in Marketing erneut verwenden.

![](assets/image2017-11-16-11-3a26-3a10.png)

## Integration {#integration}

** [Email-Vorschau-API](https://developers.marketo.com/rest-api/assets/emails/)**

Sie können E-Mails nun remote außerhalb von Marketo Vorschau haben, wodurch die lokale Anpassung von E-Mail-Inhalten vereinfacht und Fehler reduziert werden.

** [Ersetzen Sie HTML-API](https://developers.marketo.com/rest-api/assets/emails/)**

Entwickler können HTML-Inhalte von E-Mail-Assets remote aktualisieren, sodass sie in einem System arbeiten können, um Assets zu verwalten.
