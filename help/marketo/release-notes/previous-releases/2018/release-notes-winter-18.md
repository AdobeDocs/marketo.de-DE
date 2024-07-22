---
unique-page-id: 13795395
description: Versionshinweise - Winter 18 - Marketo-Dokumente - Produktdokumentation
title: Versionshinweise - Winter '18
exl-id: f08bdc91-86d3-4ea2-a74a-1398ed525bbb
feature: Release Information
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 6%

---

# Versionshinweise: Winter &#39;18 {#release-notes-winter}

Die folgenden Funktionen sind in der Version Winter 18 enthalten. Überprüfen Sie Ihre Marketo-Edition auf Funktionsverfügbarkeit.

Klicken Sie auf die Titel-Links, um detaillierte Artikel zu den einzelnen Funktionen anzuzeigen. **Hinweis**: Einige der in dieser Version enthaltenen Funktionen verfügen nicht über zugehörige Artikel. Wenn ein Thema mehrere Unterüberschriften enthält, werden die Links dort platziert.

## Verbesserungen der Kampagnenleistung und des Durchsatzes {#campaign-performance-and-throughput-enhancements}

Marketo nutzt unsere Big-Data-Architektur, um den Durchsatz von Trigger-Kampagnen zu steigern und die Verarbeitung von Web-Aktivitäten zu verbessern, sodass Sie schneller auf die Aktionen Ihrer Zielgruppe reagieren können.

## Verbesserungen in der Salesforce CRM-Integration von Marketo {#enhancements-to-marketo-s-salesforce-crm-integration}

Wir haben zwei Verbesserungen an unserer Salesforce CRM-Integration:

* [Marketo-Administratorbenachrichtigungen](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications/notification-types.md) für bestimmte Fehler bei der CRM-Synchronisierung (Anmeldeinformationen abgelaufen, API-Beschränkungen erreicht usw.)

* [Möglichkeit, E-Mail-Benachrichtigungen zu deaktivieren](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/turn-off-email-notifications-to-lead-owner.md), um Lead-Inhaber bei der Lead-Zuweisung zu informieren

Diese Verbesserungen werden im Laufe des Jahres 2018 eingeführt.

## [Marketo Leistungseinblicke](/help/marketo/product-docs/reporting/performance-insights/performance-insights-overview.md) {#marketo-performance-insights}

>[!AVAILABILITY]
>
>Performance Insights ist ein Zusatzprodukt. Wenden Sie sich für ein Angebot an Ihren Marketo-Kundenbetreuer oder Kundenbetreuer.

Erfahren Sie, wie sich Ihre Kampagnen und Kanäle mit Attributionsanalysen, interaktiven Visualisierungen und einer detaillierten Datentabelle auf die Geschäftsergebnisse auswirken.

![](assets/image2018-2-5-7-3a55-3a46.png)

## Kontobasierte Marketing-Verbesserungen {#account-based-marketing-enhancements}

**[ABM-Hierarchien](/help/marketo/product-docs/target-account-management/target/named-accounts/tam-hierarchies.md)**

Für ABM-Kunden mit Salesforce oder Microsoft Dynamics übernimmt ABM jetzt automatisch die im CRM eingerichteten übergeordneten und untergeordneten Beziehungen (und zeigt sie an). Sie können diese Beziehungen sowohl in der Datenaggregations-Berichterstellung als auch in der Kampagnenausführung verwenden.

## E-Mail-Marketing {#email-marketing}

**[Dynamisches E-Mail-Skript](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)**

Velocity-Skripterstellung wird jetzt in E-Mails mit dynamischen Inhalten unterstützt. Kombinieren Sie Geschwindigkeit und segmentierungsbasierten dynamischen Inhalt, um hochpersonalisierte E-Mails zu erstellen.

**Zeitzone des Empfängers**

* **[Monatlicher Kurszeitraum](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)**: Wir haben die Möglichkeit hinzugefügt, Pflegeprogramme monatlich zu planen.

* **[Versand stoppen](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)**: Sie können jetzt alle verbleibenden Sendungen während der Ausführung stoppen.

## Anzeigennetzwerkintegrationen {#ad-network-integrations}

**[Google Customer Match Integration](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-google-customer-match-as-a-launchpoint-service.md)**

Mit dieser Integration können Sie eine Marketo-Zielgruppe an Google senden, um mithilfe von Google AdWords Targeting durchzuführen und Zielgruppen in YouTube, Search und Gmail erneut anzusprechen.

**[API-Erweiterung für LinkedIn Matched Audiences](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md)**

Mit der neuen LinkedIn-API können Sie jetzt Personen in Ihrer Marketo-Datenbank über mehrere LinkedIn Campaign Manager-Konten hinweg erneut ansprechen.

## Web-Personalisierung {#web-personalization}

**Japanische Daten-Source für Web Personalization**

Marketo fügt eine zusätzliche japanische Datenquelle für Web Personalization hinzu, um die Identifizierung von Webbesuchern (Reverse-IP-Suche) und die Personalisierung von Besuchern aus Japan zu verbessern. Die Organisationsnamen werden auf Japanisch angezeigt.

**[Web-Segment mithilfe statischer Listen erstellen](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-segment-using-a-static-list.md)**

Web Personalization kann Inhalte nun für einen bekannten Webbesucher personalisieren, der Teil einer statischen Liste ist, die in Marketingaktivitäten (MLM) definiert ist. Mit dieser Verbesserung können Sie jetzt kanalübergreifend statische Listen vermarkten und Personen auf diesen Listen mit personalisierten Inhalten auf Ihrer Website ansprechen.

## ContentAI {#contentai}

**Prädiktive Algorithmusverbesserung**

Inhalte, die über die optimierten ContentAI-Algorithmen von Marketo empfohlen werden, generieren bis zu doppelt so viele Klicks wie zufällige Inhalte.

## Integration {#integration}

**[Aktivieren/Deaktivieren der Campaign-API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/assets/smart-campaigns)**

Mit dieser neuen API können Sie Trigger-Kampagnen remote aktivieren und deaktivieren, sodass Sie jetzt vollständig automatisierte Programmvorlagen erstellen können. Erstellen Sie einmal eine Programmvorlage und automatisieren Sie dann das Klonen, Marketingmaterial-Updates und jetzt die Aktivierung/Planung intelligenter Kampagnen.

## ToutApp {#toutapp}

**Update abbestellen**

Ab dem 1. März 2018 wird allen E-Mails, die von [ToutApp.com](https://ToutApp.com) gesendet werden (und durch Verwendung der Schaltfläche &quot;E-Mail mit Tout&quot;in Salesforce), ein Abmelde-Link am Ende angehängt.

**Live-Feed-Update**

Das Erscheinungsbild der Registerkarten &quot;Interaktion&quot;und &quot;Aufgabe&quot;wurde aktualisiert, damit Vertriebsmitglieder einfacher und schneller direkt über den Live-Feed auf die Aktivitäten ihrer Kunden reagieren können.

**People Detail View aktualisieren**

Die verbesserte Personen-Detailansicht (PDV) bietet einen umfassenden Überblick über Ihre Kontakte, indem Sie Ihre Tout- und Salesforce CRM-Kontaktdaten zusammenführen.
