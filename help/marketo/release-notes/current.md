---
description: Aktuelle Versionshinweise - Marketo-Dokumente - Produktdokumentation
title: Aktuelle Versionshinweise
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
source-git-commit: 46aff8058cb97743bee1bd5ff5ddf0ddbbb663a5
workflow-type: tm+mt
source-wordcount: '647'
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

* **Verbesserte Verwendung von Stream Designer für dynamischen Chat**: Fügen Sie Karten direkt aus der Arbeitsfläche von Stream Designer hinzu, ohne sie per Drag-and-Drop verschieben zu müssen. Die Benutzeroberfläche des dynamischen Chat wurde ebenfalls verbessert, um eine bessere Sichtbarkeit des Inhalts auf einzelnen Karten zu ermöglichen.

* **Erweiterte Regeln für die Zuweisung von Routing für dynamischen Chat**: Dynamischer Chat bietet mehr Optionen für zielgerichtetes Termin-Routing. Geben Sie an, welche Agentenbestellungen auf der Grundlage von Marketo Engage-Attributen weitergeleitet werden sollen, und stellen Sie sicher, dass die Leads an die entsprechenden Agenten weitergeleitet werden.

* **Fortschrittliche Dialogberichte für dynamischen Chat**: Zeigen Sie die Leistung Ihrer Dynamic Chat-Kampagnen mithilfe der neuen Datenvisualisierungen für Interaktions- und Konversionsmetriken detaillierter an.

* **Nicht verwendete Marketo Engage-Attribute für dynamischen Chat nicht synchronisieren**: Heben Sie die Synchronisierung von Marketo Engage-Attributen aus Ihrem Dynamic Chat-Abonnement auf, die nicht verwendet werden. Dies erleichtert Ihnen die Datenbereinigung und ermöglicht die Synchronisierung alternativer Attribute nach Bedarf.

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

* **Salesforce-API-Update**: Mit der Salesforce Summer Version 22 werden ältere API-Versionen 21-30 von Salesforce nicht mehr unterstützt. Mit dieser Marketo Engage-Version wurden alle Sales Connect-Anfragen, die ältere API-Versionen verwenden, aktualisiert, damit sie auf eine unterstützte Version passen. Ausführliche Informationen zu Salesforce API-Pensionsplänen finden Sie unter [here](https://help.salesforce.com/s/articleView?language=en_US&amp;type=1&amp;id=000354473){target=&quot;_blank&quot;}.

## API-Verbesserungen {#api-enhancements}

* **Neue Filterfunktionen für die Bulk Program Member Extract API**: Filtern Sie nach Status der Programmmitgliedschaft, updatedAt, Cadence oder erschöpftem Inhalt, um den extrahierten Datensatz zu verfeinern.

* **Verbesserung der Bulk Program Member Extract API**: Geben Sie bis zu 10 Programme während der Schaffung von Arbeitsplätzen an, um den Durchsatz zu erhöhen.

## Ankündigungen {#announcements}

* **Veraltete Forms-Version - Forms 1.0, Lead-Capture-/Speicherendpunkt und Skriptversionen von Formularen**: Die Unterstützung für Forms 1.0-Assets wird ab Oktober 2022 vollständig aus Marketo Engage entfernt. Alle vorhandenen Forms 1.0-Assets funktionieren nicht mehr. Für Marketo Engage-Formulare ist JavaScript erforderlich, damit sie auf Landingpages und Websites geladen werden können.

**_Webinar zur Produktversion_**

Nehmen Sie am 24. August 2022 um 9:00 Uhr PT / 23:00 Uhr ET teil, um eine [Live-Webinar](https://engage.marketo.com/2022_June_August_Release_Webinar_RegistrationPage.html){target=&quot;_blank&quot;} wird von unserem Produktteam gehostet, wo Sie erfahren können, wie Sie alle neuesten Produktinnovationen verwenden.
