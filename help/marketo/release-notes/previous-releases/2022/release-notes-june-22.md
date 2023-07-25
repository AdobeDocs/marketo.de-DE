---
description: Juni 2022 - Versionshinweise - Marketo-Dokumente - Produktdokumentation
title: Juni 2022 - Versionshinweise
exl-id: f4438ea8-1657-4955-9f9f-640b3ecf5caa
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 0%

---

# Versionshinweise: Juni 2022 {#release-notes-june-22}

Unten finden Sie alle Funktionen der Version vom 22. Juni. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf Funktionsverfügbarkeit.

>[!AVAILABILITY]
>
>Mit einem Stern gekennzeichnete Funktionen (![star](assets/yellow-star.png)) sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie von Ihrem Marketo Engage-Support-Mitarbeiter.

Die folgenden Funktionen werden ab der Veröffentlichung auf **24. Juni 2022**, wobei die verbleibenden Funktionen in den folgenden Wochen schrittweise eingeführt werden (sofern nicht anders angegeben).

## Marketing-Datenumgebung {#marketing-data-environment}

* **Felder CreatedAt/UpdatedAt für benutzerdefinierte Objekte verfügbar machen**: Bietet Ihnen die Möglichkeit, diese Felder im Bildschirm &quot;Personendetails&quot;zu überprüfen, um weitere Einblicke zu erhalten.

## Kanalübergreifende Orchestrierung {#cross-channel-orchestration}

* **Verbesserte Verwendung von Stream Designer für Dynamic Chat**: Fügen Sie Karten direkt aus der Arbeitsfläche von Stream Designer hinzu, ohne sie per Drag-and-Drop verschieben zu müssen. Die Dynamic Chat-Oberfläche wurde ebenfalls verbessert, um eine bessere Sichtbarkeit des Inhalts auf einzelnen Karten zu ermöglichen.

* **Erweiterte Regeln für die Zuweisung von Routing für Dynamic Chat**: Dynamic Chat bietet weitere Optionen für zielgerichtetes Terminrouting. Geben Sie an, welche Agentenbestellungen auf der Grundlage von Marketo Engage-Attributen weitergeleitet werden sollen, und stellen Sie sicher, dass die Leads an die entsprechenden Agenten weitergeleitet werden.

* **Fortschrittliche Dialogfeldberichte für Dynamic Chat**: Zeigen Sie die Leistung Ihrer Dynamic Chat-Kampagnen mithilfe der neuen Datenvisualisierungen für Interaktions- und Konversionsmetriken detaillierter an.

* **Nicht verwendete Marketo Engage-Attribute für Dynamic Chat aufheben**: Heben Sie die Synchronisierung von nicht verwendeten Marketo Engage-Attributen aus Ihrem Dynamic Chat-Abonnement auf, was Ihnen hilft, Datenbereinigungen zu erleichtern und die Synchronisierung alternativer  nach Bedarf zu ermöglichen.

## Erlebnis der nächsten Generation

**Neue Umschaltansichten**: Die folgenden Ansichten sind jetzt im Erlebnis der nächsten Generation verfügbar:

* [Ansicht mit E-Mail-Details](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [E-Mail-Listenansicht](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## Erlebnisautomatisierung {#experience-automation}

* **Ausnahmen für globale Formularfeldvalidierungsregeln**: Schließen Sie bestimmte Formulare aus den Regeln zur globalen Formularüberprüfung aus, damit Abonnementzentren und andere geschäftskritische Workflows alle Werte akzeptieren können.

* **Selbstbedienungs-Flussschritte**: Erweitern Sie die Konnektivität zwischen Marketo Engage und dem Rest Ihres Stapels mit der Möglichkeit, benutzerdefinierte Flussschritte zur Verwendung in Smart-Kampagnen zu erstellen. Sowohl Marketo Engage-Benutzer als auch -Partner können diese Funktion nutzen, um die Verwendung externer Webdienste in Trigger-, Batch- und ausführbaren Kampagnen im Gegensatz zu Webhooks zu ermöglichen, die nur in Trigger-Kampagnen verwendet werden können.

* **Munchkin-Protokoll-Agnostik-Link-Tracking**: Erweitern der Unterstützung für das Tracking von `tel` und `mailto` Links mit Munchkin , um erweiterte Web-Verhaltensweisen zu verfolgen.

* **Zusätzliche HTTP-Methoden für Webhooks**: Geben Sie PUT, PATCH und DELETE als Anfragetypen an, um mit Webdiensten zu interagieren.

## Sales Insight {#sales-insight}

![(Stern)](assets/yellow-star.png)

* **Zugriffsberechtigungen für Sales Insight in Salesforce**: Administratoren können über den Berechtigungssatz der Marketo App, der Teil des Sales Insight Salesforce-Pakets ist, Sales Insight-Zugriff für eine begrenzte Anzahl von Personen auf Benutzerebene und nicht auf Profilebene bereitstellen.

* **My Marketo Tile Update - Sales Insight-Aktionen**: Marketo-Administratoren (und Benutzer, die sie bestimmen) können jetzt über die neue Kachel &quot;Sales Insight-Aktionen&quot;auf der Seite &quot;My Marketo&quot;schnell zu ihrer Instanz mit Sales Insight-Aktionen navigieren.

## SalesConnect {#sales-connect}

![(Stern)](assets/yellow-star.png)

* **Salesforce-API-Update**: Mit der Salesforce Summer Version 22 werden ältere API-Versionen 21-30 von Salesforce nicht mehr unterstützt. Mit dieser Marketo Engage-Version wurden alle Sales Connect-Anfragen, die ältere API-Versionen verwenden, aktualisiert, damit sie auf eine unterstützte Version passen. Ausführliche Informationen zu Salesforce API-Pensionsplänen finden Sie unter [here](https://help.salesforce.com/s/articleView?language=en_US&amp;type=1&amp;id=000354473){target="_blank"}.

## API-Verbesserungen {#api-enhancements}

* **Neue Filterfunktionen für die Bulk Program Member Extract API**: Filtern Sie nach Status der Programmmitgliedschaft, updatedAt, Cadence oder erschöpftem Inhalt, um den extrahierten Datensatz zu verfeinern.

* **Verbesserung der Bulk Program Member Extract API**: Geben Sie bis zu 10 Programme während der Schaffung von Arbeitsplätzen an, um den Durchsatz zu erhöhen.

## Ankündigungen {#announcements}

* **Veraltete Forms-Version - Forms 1.0, Lead-Capture-/Speicherendpunkt und Skriptversionen von Formularen**: Die Unterstützung für Forms 1.0-Assets wird ab Oktober 2022 vollständig aus Marketo Engage entfernt. Alle vorhandenen Forms 1.0-Assets funktionieren nicht mehr. Für Marketo Engage-Formulare ist JavaScript erforderlich, damit sie auf Landingpages und Websites geladen werden können.

**_Webinar zur Produktversion_**

[Webinar zur Marketo Engage-Version vom Juni und August 2022](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}
