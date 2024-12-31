---
unique-page-id: 13795395
description: Versionshinweise - Winter '18 - Marketo-Dokumentation - Produktdokumentation
title: Versionshinweise - Winter '18
exl-id: f08bdc91-86d3-4ea2-a74a-1398ed525bbb
feature: Release Information
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 6%

---

# Versionshinweise: Winter &#39;18 {#release-notes-winter}

Die folgenden Funktionen sind in der Version Winter &#39;18 enthalten. Überprüfen Sie Ihre Marketo Edition auf die Verfügbarkeit der Funktionen.

Bitte klicken Sie auf die Titel-Links, um detaillierte Artikel für jede Funktion anzuzeigen. **Hinweis**: Einige der in dieser Version enthaltenen Funktionen verfügen nicht über zugehörige Artikel. Wenn ein Thema mehrere Unterüberschriften hat, werden die Links dort platziert.

## Verbesserungen der Kampagnenleistung und des Durchsatzes {#campaign-performance-and-throughput-enhancements}

Marketo nutzt unsere Big-Data-Architektur, um den Durchsatz von Trigger-Kampagnen zu erhöhen und die Verarbeitung von Web-Aktivitäten zu verbessern, damit Sie schneller auf die Aktionen Ihrer Zielgruppe reagieren können.

## Verbesserungen in der Salesforce CRM-Integration von Marketo {#enhancements-to-marketo-s-salesforce-crm-integration}

Unsere Salesforce CRM-Integration wurde in zweifacher Hinsicht verbessert:

* [Marketo Admin-](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications/notification-types.md): für bestimmte CRM-Synchronisierungsfehler (abgelaufene Anmeldeinformationen, API-Beschränkungen erreicht usw.)

* [Möglichkeit zum Deaktivieren von E-Mail](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/turn-off-email-notifications-to-lead-owner.md)Benachrichtigungen an Lead-Inhaber bei der Lead-Zuweisung

Diese Verbesserungen werden im Laufe des Jahres 2018 eingeführt.

## [Marketo Leistungseinblicke](/help/marketo/product-docs/reporting/performance-insights/performance-insights-overview.md) {#marketo-performance-insights}

>[!AVAILABILITY]
>
>Performance Insights ist ein Zusatzprodukt. Wenden Sie sich an Ihren Marketo Account Manager oder Account Executive, um ein Angebot zu erhalten.

Erfahren Sie mit Attributionsanalysen, interaktiven Visualisierungen und einer detaillierten Datentabelle, wie sich Ihre Kampagnen und Kanäle auf die Geschäftsergebnisse auswirken.

![](assets/image2018-2-5-7-3a55-3a46.png)

## Verbesserungen beim Account-basierten Marketing {#account-based-marketing-enhancements}

**[ABM-Hierarchien](/help/marketo/product-docs/target-account-management/target/named-accounts/tam-hierarchies.md)**

Für ABM-Kunden mit Salesforce oder Microsoft Dynamics erbt ABM jetzt automatisch die im CRM eingerichteten hierarchischen Beziehungen (und zeigt sie an). Sie können diese Beziehungen sowohl in der Datenaggregationsberichterstattung als auch in der Kampagnenausführung verwenden.

## E-Mail-Marketing {#email-marketing}

**[Dynamisches E-Mail-Skript](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md)**

Velocity-Skripterstellung wird jetzt in E-Mails mit dynamischen Inhalten unterstützt. Kombinieren Sie Geschwindigkeit und segmentierungsbasierte dynamische Inhalte, um hochgradig personalisierte E-Mails zu erstellen.

**Zeitzone des Empfängers**

* **[Monthly Nurture Cadence](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/schedule-email-programs-with-recipient-time-zone.md)**: Wir haben die Möglichkeit hinzugefügt, Nurture-Programme mit einer monatlichen Kadenz zu planen.

* **[Versand stoppen](/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/scheduling-with-recipient-time-zone/abort-delivery-of-email-programs-scheduled-with-recipient-time-zone.md)**: Sie können jetzt alle verbleibenden Sendungen in der Mitte des Durchgangs stoppen.

## Netzwerkintegrationen hinzufügen {#ad-network-integrations}

**[Google Customer Match Integration](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-google-customer-match-as-a-launchpoint-service.md)**

Mit dieser Integration können Sie eine Marketo-Zielgruppe an Google senden, um sie mit Google AdWords anzusprechen, und Zielgruppen in YouTube, Search und Gmail erneut ansprechen.

Verbesserung der **[LinkedIn Matched Audiences-API](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md)**

Mit unserer neuen LinkedIn-API können Sie jetzt Personen in Ihrer Marketo-Datenbank über mehrere LinkedIn Campaign Manager-Konten hinweg erneut ansprechen.

## Web-Personalisierung {#web-personalization}

**Japanische Daten-Source für Web-Personalization**

Marketo fügt eine zusätzliche japanische Datenquelle für Web Personalization hinzu, um die Identifizierung von Web-Besuchern (Reverse-IP-Lookup) und die Personalisierung für Besucher aus Japan zu verbessern. Organisationsnamen werden auf Japanisch angezeigt.

**[Web-Segment mithilfe statischer Listen erstellen](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-segment-using-a-static-list.md)**

Web Personalization kann jetzt Inhalte für einen bekannten Web-Besucher personalisieren, der Teil einer in Marketing-Aktivitäten (MLM) definierten statischen Liste ist. Mit dieser Verbesserung können Sie jetzt kanalübergreifend statische Listen vermarkten und Personen auf diesen Listen mit personalisierten Inhalten auf Ihrer Website ansprechen.

## ContentAI {#contentai}

**Verbesserung des prädiktiven Algorithmus**

Inhalte, die über die optimierten ContentAI-Algorithmen von Marketo empfohlen werden, generieren bis zu doppelt so viele Klicks wie zufällige Inhalte.

## Integration {#integration}

**[Campaign-API aktivieren/deaktivieren](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/assets/smart-campaigns)**

Mit dieser neuen API können Sie Trigger-Kampagnen per Fernzugriff aktivieren und deaktivieren, sodass Sie jetzt vollständig automatisierte Programmvorlagen erstellen können. Erstellen Sie einmal eine Programmvorlage und automatisieren Sie dann das Klonen, die Aktualisierung von Marketing-Marketingmaterial und jetzt die Aktivierung/Planung von Smart-Kampagnen.

## ToutApp {#toutapp}

**Update abbestellen**

Ab dem 1. März 2018 wird für alle E-Mails, die von [ToutApp.com](https://ToutApp.com) (und über die Schaltfläche „E-Mail mit Tout“ in Salesforce) gesendet werden, unten ein Abmelde-Link angehängt.

**Live-Feed-Update**

Das Erscheinungsbild der Registerkarten Interaktion und Aufgabe wurde aktualisiert, damit die Vertriebsmitarbeiter direkt über den Live-Feed einfacher und schneller auf die Aktivitäten ihrer Kunden reagieren können.

**People Detail View aktualisieren**

Die verbesserte Personen-Detailansicht (PDV) bietet eine umfassende Ansicht Ihrer Kontakte, indem Sie Ihre Tout- und Salesforce CRM-Kontaktdaten zusammenführen.
