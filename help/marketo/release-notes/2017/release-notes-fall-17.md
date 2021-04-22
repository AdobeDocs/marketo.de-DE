---
unique-page-id: 12983280
description: Versionshinweise - Herbst 17 - Marketo Docs - Produktdokumentation
title: Versionshinweise - Herbst 17
exl-id: 329022e6-f388-4ff9-9724-62aeed76c0b9
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 11%

---

# Versionshinweise: Fall &#39;17 {#release-notes-fall}

Die folgenden Funktionen sind in der Version Herbst 17 enthalten. Überprüfen Sie Ihre Marketo Edition auf Funktionsverfügbarkeit.

Bitte klicken Sie auf die Titellinks, um detaillierte Ansichten zu den einzelnen Funktionen anzuzeigen. Hinweis: Einige der in dieser Version enthaltenen Funktionen verfügen nicht über zugehörige Artikel. Wenn ein Thema mehrere Unterüberschriften enthält, werden die Links dort platziert.

## Systemzuverlässigkeit {#system-reliability}

Wir haben die Marketo-Kerninfrastruktur weiter verbessert, einschließlich einer besseren Sequenzierung, weniger Diskrepanzen und verbesserter Munchkin-Stabilität.

## SFDC Sync-Performance {#sfdc-sync-performance}

Profitieren Sie von einer umfangreicheren und schnelleren Synchronisierung in Marketo und Salesforce. Datenänderungen, die Massenaktualisierungen von Konten oder Interessenten erfordern, können in parallele Warteschlangen aufgeteilt werden, um Rückstände zu vermeiden. Ereignisse und Aufgaben werden jetzt auch bis zu 50 % schneller synchronisiert.

## Verbesserungen der Analyse-Performance {#analytics-performance-improvements}

Die jüngsten Infrastrukturverbesserungen haben Angebot zu höherer Betriebszeit und Stabilität in den Marketo Berichte- und Analysetools geführt, sodass Sie schneller Ad-hoc-Berichte erstellen können.

## [Zeitzone des Empfängers](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md) {#recipient-time-zone}

Mit dieser neuen Funktion können Sie jetzt E-Mails gemäß den örtlichen Zeitzonen speichern und senden. E-Mail- und Interaktions-Programm können so konfiguriert werden, dass sie in den Zeitzonen der Empfänger bereitgestellt werden. Dadurch müssen nicht mehr mehrere Programm erstellt werden. Einmalig senden und Marketo hält die E-Mail automatisch bis zur richtigen Ortszeit. Steigern Sie E-Mail-Metriken, beachten Sie lokale Praktiken und sparen Sie Zeit, indem Sie ein einzelnes Programm global verwenden.

![](assets/image2017-11-29-8-3a45-3a47.png)

>[!NOTE]
>
>Wenn Sie die Zeitzone des Empfängers noch nicht in Ihren E-Mail- und Interaktions-Programmen aktivieren können, sollten Sie sich nicht panisch verhalten! Diese Funktion wird schrittweise allen Kunden zur Verfügung gestellt.

## [Überprüfung von Beispiel-E-Mails je Segment](/help/marketo/product-docs/email-marketing/general/creating-an-email/send-a-sample-email.md) {#review-sample-emails-by-segment}

Marketo verfügt über eine neue Option zum Auswählen eines Segments, wenn E-Mails zum Review gesendet werden. Sie müssen nicht mehr manuell festlegen, zu welchem Segment ein Interessent gehört, sodass es einfacher ist, E-Mails mit dynamischen Inhalten an verschiedene Segmente zu senden.

## [Kundenspezifische Fragen zur LinkedIn Lead-Generierung](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md) {#linkedin-lead-gen-custom-questions}

Passen Sie Ihre Formulare zur LinkedIn Lead-Generierung an, um so benutzerdefinierte Lead-Attribute zu sammeln. Sie können jetzt bis zu drei benutzerspezifische Fragen pro Formular stellen, aus einer einzeiligen Texteingabe oder Fragen mit mehreren Auswahlmöglichkeiten wählen und wieder den Marketo-Interessentenfeldern zuordnen.

## [Slack-Integration](/help/marketo/product-docs/administration/additional-integrations/add-slack-as-a-launchpoint-service.md) {#slack-integration}

Im Rahmen der neuen Slack-Integration haben wir zwei Funktionen veröffentlicht:

* Systembenachrichtigungen: Erhalten Sie Benachrichtigungen über wichtige Ereignis in Ihrer Marketo-Instanz, z. B. Warnungen über den Status der aktuellen Kampagne und Probleme, die sofortige Aufmerksamkeit erfordern.
* Interessante Momente: Wenn ein Marketo Insight von einer bekannten Person aus einem Kundenkonto ausgelöst wurde, können Interessenteninhaber per Slack benachrichtigt werden. Benachrichtigungen enthalten Interessenteninformationen sowie Details zum Kundenkonto.

## ABM-Verbesserungen {#abm-enhancements}

**[Konten ohne Kontakte anzeigen](https://docs.marketo.com/x/fKCt)**

Marketo ABM synchronisiert und zeigt CRM-Konten ohne Kontakte an. Schließen Sie neue Konten ohne vorherigen Verkauf oder Marketingverlauf ein und verfolgen Sie den Fortschritt, indem Sie nachfolgende Interessenten zu den Konten abgleichen.

## ContentAI Analyse {#contentai-analytics}

**[Neuer ABM-Kontenlistenfilter](https://docs.marketo.com/x/1BPG)**

Ansicht und Vergleich der Content-Performance über ABM-Listen hinweg, um vorhandene Inhalte zu optimieren. ContentAI zeigt Ihnen:

* Hauptinhalt angezeigt
* Top-konvertierte Inhalte
* AI-basierte vorgeschlagene Inhalte für Marketing-Aktivitäten

## Verbesserte Web-Personalisierung {#web-personalization-enhancements}

**[Token für Webkampagnen](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Token stehen jetzt zur Verwendung in Web-Kampagnen zur Verfügung. Nutzen Sie Token, um personalisierte Nachrichten und Inhalte bereitzustellen, um die Interaktion mit Ihren Web-Kampagnen zu steigern.

![](assets/image2017-11-16-11-3a25-3a7.png)

**[Studio-Bilder im Webkampagnen-Editor designen](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Sparen Sie Zeit, indem Sie kreative Assets und Bilder über mehrere Kanal innerhalb von Marketo hinweg wiederverwenden.

![](assets/image2017-11-16-11-3a26-3a10.png)

## Integration  {#integration}

**[E-Mail-Vorschau API](https://developers.marketo.com/rest-api/assets/emails/)**

Sie können E-Mails nun remote außerhalb von Marketo Vorschau haben, wodurch die lokale Anpassung von E-Mail-Inhalten vereinfacht und Fehler reduziert werden.

**[HTML API ersetzen](https://developers.marketo.com/rest-api/assets/emails/)**

Entwickler können HTML-Inhalte von E-Mail-Assets remote aktualisieren, sodass sie in einem System arbeiten können, um Assets zu verwalten.
