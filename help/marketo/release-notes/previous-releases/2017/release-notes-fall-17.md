---
unique-page-id: 12983280
description: Versionshinweise - Herbst '17 - Marketo-Dokumente - Produktdokumentation
title: Versionshinweise - Herbst '17
exl-id: 329022e6-f388-4ff9-9724-62aeed76c0b9
feature: Release Information
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 5%

---

# Versionshinweise: Herbst &#39;17 {#release-notes-fall}

Die folgenden Funktionen sind in der Version vom Herbst 17 enthalten. Überprüfen Sie Ihre Marketo Edition auf die Verfügbarkeit der Funktionen.

Bitte klicken Sie auf die Titel-Links, um detaillierte Artikel für jede Funktion anzuzeigen. Hinweis: Einige der in dieser Version enthaltenen Funktionen verfügen nicht über zugehörige Artikel. Wenn ein Thema mehrere Unterüberschriften hat, werden die Links dort platziert.

## Systemzuverlässigkeit {#system-reliability}

Wir haben weitere Verbesserungen an der Marketo-Kerninfrastruktur vorgenommen, einschließlich einer besseren Sequenzierung, weniger Inkongruenzen und verbesserter [!DNL Munchkin].

## SFDC Sync-Performance {#sfdc-sync-performance}

Nutzen Sie die Vorteile einer umfassenderen und schnelleren Synchronisierung zwischen Marketo und [!DNL Salesforce]. Datenänderungen, die Massenaktualisierungen von Konten oder Leads erfordern, können in parallele Warteschlangen aufgeteilt werden, um Rückstände zu vermeiden. Ereignisse und Aufgaben synchronisieren sich jetzt um bis zu 50 % schneller.

## Verbesserungen der Analyse-Performance {#analytics-performance-improvements}

Jüngste Infrastrukturverbesserungen bieten eine höhere Verfügbarkeit und Stabilität innerhalb der Reporting- und Analyse-Tools von Marketo, sodass Sie Ad-hoc-Berichte schneller erstellen können.

## [Zeitzone des Empfängers](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/understanding-recipient-time-zone.md) {#recipient-time-zone}

Mit dieser neuen Funktion können Sie jetzt E-Mails entsprechend den lokalen Zeitzonen speichern und versenden. E-Mail- und Interaktionsprogramme können so konfiguriert werden, dass sie in den Zeitzonen der Empfängerinnen und Empfänger bereitgestellt werden, sodass nicht mehrere Programme erstellt werden müssen - einmal senden und Marketo speichert die E-Mail automatisch bis zur korrekten Ortszeit. Erhöhen Sie E-Mail-Metriken, beachten Sie lokale Best Practices und sparen Sie Zeit, indem Sie global ein einziges Programm verwenden.

![](assets/image2017-11-29-8-3a45-3a47.png)

>[!NOTE]
>
>Wenn Sie die Zeitzone der Empfänger in Ihren E-Mail- und Interaktionsprogrammen noch nicht aktivieren können, geraten Sie nicht in Panik! Diese Funktion wird für alle Kunden schrittweise aktiviert.

## [Beispiel-E-Mails nach Segment überprüfen](/help/marketo/product-docs/email-marketing/general/creating-an-email/send-a-sample-email.md) {#review-sample-emails-by-segment}

Marketo bietet eine neue Option, beim Senden von Beispiel-E-Mails zur Überprüfung ein Segment auszuwählen. Sie müssen nicht mehr manuell ermitteln, zu welchem Segment ein Lead gehört, was das Senden von E-Mails mit dynamischen Inhalten an verschiedene Segmente erleichtert.

## [Benutzerdefinierte Fragen zu LinkedIn-Lead-Gen](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md) {#linkedin-lead-gen-custom-questions}

Passen Sie Ihre [!UICONTROL LinkedIn Lead Gen]-Formulare an, um benutzerdefinierte Lead-Attribute zu erfassen. Sie können jetzt bis zu drei benutzerdefinierte Fragen pro Formular stellen, aus einzeiligen Texteingaben oder Multiple-Choice-Fragen auswählen und diese wieder den Marketo-Lead-Feldern zuordnen.

## Slack-Integration {#slack-integration}

Im Rahmen unserer neuen Slack-Integration haben wir zwei Funktionen veröffentlicht:

* Systembenachrichtigungen: Erhalten Sie Slack-Benachrichtigungen zu wichtigen Ereignissen in Ihrer Marketo-Instanz, z. B. Warnhinweise zum aktuellen Kampagnenstatus und zu Problemen, die sofortiges Eingreifen erfordern.
* Interessante Momente: Wenn eine Marketo Insight von einer bekannten Person aus einem Kundenkonto ausgelöst wurde, können Lead-Inhaber über Slack benachrichtigt werden. Benachrichtigungen enthalten Lead-Informationen sowie Details zum Verkaufskonto.

## ABM-Verbesserungen {#abm-enhancements}

**[Konten ohne Kontakte anzeigen](https://docs.marketo.com/x/fKCt)**

Marketo ABM synchronisiert und zeigt jetzt CRM-Konten ohne Kontakte an. Neue Konten ohne vorherigen Verkaufs- oder Marketing-Verlauf einschließen und den Fortschritt verfolgen, indem nachfolgende Leads mit den Konten abgeglichen werden.

## ContentAI Analyse {#contentai-analytics}

**[Neuer ABM-Kontolistenfilter](https://docs.marketo.com/x/1BPG)**

Anzeigen und Vergleichen der Inhaltsleistung in allen ABM-Kontolisten zur Optimierung vorhandener Inhalte. ContentAI zeigt Ihnen:

* Am häufigsten angezeigte Inhalte
* Am häufigsten konvertierter Inhalt
* KI-gestützte vorgeschlagene Inhalte für Marketing-Aktivitäten

## Verbesserte Web-Personalisierung {#web-personalization-enhancements}

**[Token für Webkampagnen](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Token sind jetzt zur Verwendung in Web-Kampagnen verfügbar. Nutzen Sie Token zur Bereitstellung personalisierter Nachrichten und Inhalte, um die Interaktion mit Ihren Web-Kampagnen zu steigern.

![](assets/image2017-11-16-11-3a25-3a7.png)

**[Studio-Bilder im Webkampagnen-Editor designen](/help/marketo/product-docs/web-personalization/working-with-web-campaigns/using-the-web-personalization-rich-text-editor.md)**

Sparen Sie Zeit durch die Wiederverwendung von Kreativ-Assets und -Bildern auf mehreren Kanälen in Marketo.

![](assets/image2017-11-16-11-3a26-3a10.png)

## Integration  {#integration}

**[Email Preview API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/email-scripting)**

Sie können jetzt eine Remote-Vorschau von E-Mails außerhalb von Marketo anzeigen, wodurch der Prozess der Lokalisierung von E-Mail-Inhalten vereinfacht und Fehler reduziert werden.

**[HTML-API ersetzen](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/email-scripting)**

Entwicklerinnen und Entwickler können HTML-Inhalte von E-Mail-Assets remote aktualisieren, sodass sie in einem einzigen System arbeiten können, um Assets zu verwalten.
