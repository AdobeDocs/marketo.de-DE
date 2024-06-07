---
unique-page-id: 12983280
description: Versionshinweise - Herbst 17 - Marketo-Dokumente - Produktdokumentation
title: Versionshinweise - Herbst 17
exl-id: 329022e6-f388-4ff9-9724-62aeed76c0b9
feature: Release Information
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '588'
ht-degree: 5%

---

# Versionshinweise: Herbst 17 {#release-notes-fall}

Die folgenden Funktionen sind in der Herbstversion 17 enthalten. Überprüfen Sie Ihre Marketo-Edition auf Funktionsverfügbarkeit.

Klicken Sie auf die Titel-Links, um detaillierte Artikel zu den einzelnen Funktionen anzuzeigen. Hinweis: Einige der in dieser Version enthaltenen Funktionen verfügen nicht über zugehörige Artikel. Wenn ein Thema mehrere Unterüberschriften enthält, werden die Links dort platziert.

## Systemzuverlässigkeit {#system-reliability}

Wir haben die Marketo-Kerninfrastruktur weiter verbessert, einschließlich einer besseren Sequenzierung, weniger Diskrepanzen und verbesserter Munchkin-Stabilität.

## SFDC Sync-Performance {#sfdc-sync-performance}

Profitieren Sie von einer umfangreicheren und schnelleren Synchronisation in Marketo und Salesforce. Datenänderungen, die Massenaktualisierungen von Konten oder Leads erfordern, können in parallele Warteschlangen aufgeteilt werden, um Rückstände zu vermeiden. Ereignisse und Aufgaben werden jetzt auch um bis zu 50 % schneller synchronisiert.

## Verbesserungen der Analyse-Performance {#analytics-performance-improvements}

Die jüngsten Infrastrukturverbesserungen bieten verbesserte Betriebszeiten und Stabilität innerhalb der Reporting- und Analysetools von Marketo, sodass Sie Ad-hoc-Berichte schneller erstellen können.

## [Zeitzone des Empfängers](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md) {#recipient-time-zone}

Mit dieser neuen Funktion können Sie jetzt E-Mails entsprechend den lokalen Zeitzonen speichern und versenden. E-Mail- und Interaktionsprogramme können so konfiguriert werden, dass sie in der Zeitzone der Empfänger versendet werden. So müssen nicht mehrere Programme erstellt werden. Der einmalige Versand und die automatische Speicherung der E-Mail durch Marketo erfolgt bis zur korrekten Ortszeit. Steigern Sie E-Mail-Metriken, beachten Sie lokale Praktiken und sparen Sie Zeit, indem Sie ein einzelnes Programm global verwenden.

![](assets/image2017-11-29-8-3a45-3a47.png)

>[!NOTE]
>
>Wenn Sie die Zeitzone der Empfänger noch nicht in Ihren E-Mail- und Interaktionsprogrammen aktivieren können, sollten Sie nicht in Panik geraten! Diese Funktion wird schrittweise allen Kunden ermöglicht.

## [Beispiel-E-Mails nach Segment überprüfen](/help/marketo/product-docs/email-marketing/general/creating-an-email/send-a-sample-email.md) {#review-sample-emails-by-segment}

Marketo bietet eine neue Option, um beim Senden von Beispiel-E-Mails zur Überprüfung ein Segment auszuwählen. Sie müssen nicht mehr manuell festlegen, zu welchem Segment ein Lead gehört, wodurch es einfacher wird, E-Mails mit dynamischen Inhalten an verschiedene Segmente zu senden.

## [LinkedIn Lead Gen Custom Questions](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md) {#linkedin-lead-gen-custom-questions}

Passen Sie Ihre LinkedIn Lead Gen-Formulare an, um benutzerdefinierte Lead-Attribute zu erfassen. Sie können jetzt bis zu drei benutzerdefinierte Fragen pro Formular stellen, aus einer einzeiligen Texteingabe oder Multiple-Choice-Fragen wählen und zu Marketo-Lead-Feldern zurückordnen.

## Slack-Integration {#slack-integration}

Im Rahmen der neuen Slack-Integration wurden zwei Funktionen veröffentlicht:

* Systembenachrichtigungen: Hier erhalten Sie Slack-Benachrichtigungen zu wichtigen Ereignissen in Ihrer Marketo-Instanz, z. B. Warnungen zum aktuellen Kampagnenstatus und zu Problemen, die sofortige Aufmerksamkeit erfordern.
* Interessante Momente: Wenn ein Marketo Insight von einer bekannten Person aus einem Verkaufskonto ausgelöst wurde, können Lead-Inhaber über Slack benachrichtigt werden. Benachrichtigungen enthalten Lead-Informationen sowie Details zum Verkaufskonto.

## ABM-Verbesserungen {#abm-enhancements}

**[Konten ohne Kontakte anzeigen](https://docs.marketo.com/x/fKCt)**

Marketo ABM synchronisiert und zeigt CRM-Konten nun ohne Kontakte an. Fügen Sie neue Konten ohne vorherigen Verkaufs- oder Marketingverlauf hinzu und verfolgen Sie den Fortschritt, indem Sie nachfolgende Leads zu den Konten abgleichen.

## ContentAI Analyse {#contentai-analytics}

**[Neuer ABM-Kontolistenfilter](https://docs.marketo.com/x/1BPG)**

Zeigen Sie die Inhaltsleistung in den ABM-Kontolisten an und vergleichen Sie sie, um vorhandene Inhalte zu optimieren. ContentAI zeigt Ihnen:

* am häufigsten angezeigter Inhalt
* Top-konvertierte Inhalte
* KI-gestützte vorgeschlagene Inhalte für Marketingaktivitäten

## Verbesserte Web-Personalisierung {#web-personalization-enhancements}

**[Token für Webkampagnen](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Token sind jetzt zur Verwendung in Webkampagnen verfügbar. Nutzen Sie Token, um personalisierte Nachrichten und Inhalte bereitzustellen und so die Interaktion mit Ihren Web-Kampagnen zu steigern.

![](assets/image2017-11-16-11-3a25-3a7.png)

**[Studio-Bilder im Webkampagnen-Editor designen](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Sparen Sie Zeit, indem Sie Kreativ-Assets und -Bilder in Marketo kanalübergreifend wiederverwenden.

![](assets/image2017-11-16-11-3a26-3a10.png)

## Integration  {#integration}

**[Email Preview API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/email-scripting)**

Sie können jetzt eine Remote-Vorschau von E-Mails außerhalb von Marketo anzeigen, wodurch die Lokalisierung von E-Mail-Inhalten vereinfacht und Fehler reduziert werden.

**[HTML-API ersetzen](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/email-scripting)**

Entwickler können den HTML-Inhalt von E-Mail-Assets remote aktualisieren, sodass sie in einem einzigen System arbeiten können, um Assets zu verwalten.
