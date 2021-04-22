---
unique-page-id: 13795395
description: Versionshinweise - Winter 18 - Marketo Docs - Produktdokumentation
title: Versionshinweise - Winter 18
exl-id: f08bdc91-86d3-4ea2-a74a-1398ed525bbb
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 8%

---

# Versionshinweise: Winter &#39;18 {#release-notes-winter}

Die folgenden Funktionen sind in der Version Winter &#39;18 enthalten. Überprüfen Sie Ihre Marketo Edition auf Funktionsverfügbarkeit.

Bitte klicken Sie auf die Titellinks, um detaillierte Ansichten zu den einzelnen Funktionen anzuzeigen. **Hinweis**: Einige der in dieser Version enthaltenen Funktionen verfügen nicht über zugehörige Artikel. Wenn ein Thema mehrere Unterüberschriften enthält, werden die Links dort platziert.

## Verbesserungen der Leistung und des Durchsatzes von Kampagnen {#campaign-performance-and-throughput-enhancements}

Marketo nutzt unsere Big-Data-Architektur, um den Durchsatz der Trigger-Kampagne zu steigern und die Verarbeitung der Web-Aktivität zu verbessern, sodass Sie schneller auf die Aktionen Ihrer Audience reagieren können.

## Verbesserungen der Salesforce CRM-Integration von Marketo {#enhancements-to-marketo-s-salesforce-crm-integration}

Wir haben zwei Verbesserungen an unserer Salesforce CRM-Integration:

* [Marketo-](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications/notification-types.md) Administratorbenachrichtigungen für bestimmte CRM-Synchronisierungsfehler (Anmeldeinformationen abgelaufen, API-Beschränkungen erreicht usw.)

* [Möglichkeit, E-Mail-](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/turn-off-email-notifications-to-lead-owner.md) Benachrichtigungen bei Interessentenzuweisungen zu deaktivieren

Diese Verbesserungen werden im Laufe des Jahres 2018 eingeführt.

## [Marketo Leistungseinblicke](/help/marketo/product-docs/reporting/performance-insights/performance-insights-overview.md) {#marketo-performance-insights}

>[!AVAILABILITY]
>
>Performance Insights ist ein Zusatzprodukt. Wenden Sie sich an Ihren Marketo Customer Success Manager oder Kundenbetreuer, um ein Angebot zu erhalten.

Informieren Sie sich, wie Ihre Kampagnen und Kanal mit Zuordnungsanalysen, interaktiven Visualisierungen und einer detaillierten Datentabelle die Geschäftsergebnisse beeinflussen.

![](assets/image2018-2-5-7-3a55-3a46.png)

## Kontobasierte Marketingverbesserungen {#account-based-marketing-enhancements}

**[ABM-Hierarchien](/help/marketo/product-docs/target-account-management/target/named-accounts/tam-hierarchies.md)**

Für ABM-Kunden mit Salesforce oder Microsoft Dynamics übernimmt ABM nun automatisch die im CRM eingerichteten Beziehungen zwischen Mutter und Kind (und zeigt sie an). Sie können diese Beziehungen sowohl beim Rollup-Berichte als auch bei der Ausführung von Kampagnen verwenden.

## E-Mail-Marketing {#email-marketing}

**[Dynamisches E-Mail-Skript](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)**

Velocity-Scripting wird nun auch bei E-Mails mit dynamischem Inhalt unterstützt. Kombinieren Sie Geschwindigkeit und segmentierungsbasierte dynamische Inhalte, um hochpersonalisierte E-Mails zu erstellen.

**Zeitzone des Empfängers**

* **[Monatliche Krankenpflege](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)**: Wir haben die Möglichkeit hinzugefügt, Programme mit monatlicher Kadenz zu planen.

* **[Versand](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)** beenden: Sie können jetzt alle verbleibenden Sends während der Ausführung stoppen.

## Ad-Netzwerk-Integrationen {#ad-network-integrations}

**[Google Customer Match Integration](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-google-customer-match-as-a-launchpoint-service.md)**

Mit dieser Integration können Sie eine Marketo-Audience an Google senden, die mit Google AdWords als Ziel ausgewählt werden soll, sowie Audiencen zur erneuten Zielgruppe über YouTube, Search und Gmail hinweg.

**[API-Verbesserung für linkedIn-übereinstimmende Audiencen](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md)**

Mit der neuen LinkedIn-API können Sie jetzt Personen in Ihrer Marketo-Datenbank über mehrere LinkedIn Kampagne Manager-Konten neu Zielgruppe werden.

## Web-Personalisierung {#web-personalization}

**Japanische Datenquelle für die Web-Personalisierung**

Marketo fügt eine zusätzliche japanische Datenquelle für die Web-Personalisierung hinzu, um die Identifizierung von Web-Besuchern (Reverse-IP-Suche) und die Personalisierung von Besuchern aus Japan zu verbessern. Die Organisationsnamen werden auf Japanisch angezeigt.

**[Web-Segment mithilfe statischer Listen erstellen](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-segment-using-a-static-list.md)**

Mit der Web-Personalisierung können Inhalte nun an einen bekannten Web-Besucher angepasst werden, der Teil einer statischen Liste ist, die in Marketing-Aktivitäten (MLM) definiert ist. Mit dieser Verbesserung können Sie jetzt auf statische Listen über Kanal hinweg vermarkten und Personen auf diesen Listen mit personalisierten Inhalten auf Ihrer Website Zielgruppe geben.

## ContentAI {#contentai}

**Prädiktive Algorithmusverbesserung**

Inhalte, die über die optimierten ContentAI-Algorithmen von Marketo empfohlen werden, generieren bis zu doppelt so viele Klicks wie zufällige Inhalte.

## Integration {#integration}

**[Kampagnen-API aktivieren/deaktivieren](https://developers.marketo.com/rest-api/assets/campaigns/)**

Mit dieser neuen API können Sie Trigger-Kampagnen remote aktivieren und deaktivieren, sodass Sie jetzt vollständig automatisierte Programm-Vorlagen erstellen können. Erstellen Sie einmal eine Vorlage für ein Programm und automatisieren Sie dann das Klonen, Marketingmaterial-Updates und jetzt die Aktivierung/Planung intelligenter Kampagnen.

## ToutApp {#toutapp}

**Update abbestellen**

Ab dem 1. März 2018 wird an allen E-Mails, die von [ToutApp.com](https://ToutApp.com) gesendet werden (und über die Schaltfläche &quot;E-Mail mit Tout&quot;in Salesforce), ein Link zum Abbestellen des Abonnements am Ende angehängt.

**Live-Feed-Update**

Wir haben das Erscheinungsbild der Registerkarten Interaktion und Aufgabe aktualisiert, damit Vertriebsmitarbeiter die Aktivitäten ihrer Kunden direkt aus dem Live Feed heraus leichter und schneller beantworten können.

**People Detail View aktualisieren**

Die verbesserte People Detail Ansicht (PDV) Angebot eine umfassende Ansicht Ihrer Kontakte, indem Sie Ihre Tout- und Salesforce CRM-Kontaktdaten zusammenführen.
