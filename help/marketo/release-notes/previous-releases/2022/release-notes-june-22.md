---
description: Juni 2022 - Versionshinweise - Marketo-Dokumente - Produktdokumentation
title: Juni 2022 - Versionshinweise
exl-id: f4438ea8-1657-4955-9f9f-640b3ecf5caa
feature: Release Information
source-git-commit: cf4dcb6a316eba631ccb73a991c09e83c80b82ca
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# Juni 2022 - Versionshinweise {#release-notes-june-22}

Unten finden Sie alle Funktionen der Version vom 22. Juni. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf Funktionsverfügbarkeit.

>[!AVAILABILITY]
>
>Mit einem Stern (![Stern](assets/yellow-star.png)) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Wenden Sie sich an Ihren Marketo Engage-Support-Mitarbeiter, um mehr zu erfahren.

Die folgenden Funktionen werden am 24. Juni 2022 veröffentlicht. Der Rollout der verbleibenden Funktionen erfolgt schrittweise über die folgenden Wochen (sofern nicht anders angegeben).****

## Marketing-Datenumgebung {#marketing-data-environment}

* **ErstellteAt/UpdatedAt-Felder für benutzerdefinierte Objekte verfügbar machen**: Ermöglicht Ihnen die Überprüfung dieser Felder auf dem Bildschirm &quot;Personendetails&quot;, um weitere Einblicke zu erhalten.

## Kanalübergreifende Orchestrierung {#cross-channel-orchestration}

* **Verbesserte Nutzung der Stream-Designer für Dynamic Chat**: Fügen Sie Karten direkt aus der Stream-Designer-Arbeitsfläche hinzu, ohne sie per Drag-and-Drop verschieben zu müssen. Die Dynamic Chat-Oberfläche wurde ebenfalls verbessert, um eine bessere Sichtbarkeit des Inhalts auf einzelnen Karten zu ermöglichen.

* **Erweiterte Einstellungsregeln für Dynamic Chat**: Dynamic Chat bietet mehr Optionen für zielgerichtetes Terminierungsrouting. Geben Sie an, welche Agententermine auf der Grundlage von Marketo Engage-Attributen weitergeleitet werden sollen, und stellen Sie sicher, dass Leads an die entsprechenden Agenten weitergeleitet werden.

* **Fortschrittliche Dialogberichte für Dynamic Chat**: Zeigen Sie die Leistung Ihrer Dynamic Chat-Kampagnen mithilfe der neuen Datenvisualisierungen für Interaktions- und Konversionsmetriken detaillierter an.

* **Nicht verwendete Marketo Engage-Attribute für Dynamic Chat aufheben**: Synchronisieren Sie Marketo Engage-Attribute aus Ihrem Dynamic Chat-Abonnement, die nicht verwendet werden, und erleichtern Sie die Datenbereinigung und ermöglichen Sie die Synchronisierung alternativer Attribute nach Bedarf.

## Erlebnis der nächsten Generation

**Neue Umschalter-Ansichten**: Die folgenden Ansichten sind jetzt im Erlebnis der nächsten Generation verfügbar:

* [Ansicht &quot;E-Mail-Details&quot;](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [E-Mail-Listenansicht](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## Erlebnisautomatisierung {#experience-automation}

* **Ausschlüsse von globalen Formularfeldvalidierungsregeln**: Schließen Sie bestimmte Formulare aus globalen Formularvalidierungsregeln aus, damit Abonnementzentren und andere geschäftskritische Workflows alle Werte akzeptieren können.

* **Schritte zum Selbstbedienungsfluss**: Erweitern Sie die Konnektivität zwischen Marketo Engage und dem Rest Ihres Stapels mit der Möglichkeit, benutzerdefinierte Flussschritte zur Verwendung in Smart-Kampagnen zu erstellen. Sowohl Marketo Engage-Benutzer als auch -Partner können diese Funktion nutzen, um die Verwendung externer Webdienste in Trigger-, Batch- und ausführbaren Kampagnen im Gegensatz zu Webhooks zu ermöglichen, die nur in Trigger-Kampagnen verwendet werden können.

* **Munchkin Protocol Agnostic Link Tracking**: Erweitern Sie die Unterstützung für das Tracking von `tel` - und `mailto` -Links mit Munchkin, um erweiterte Web-Verhaltensweisen zu verfolgen.

* **Zusätzliche HTTP-Methoden für Webhooks**: Geben Sie PUT, PATCH und DELETE als Anfragetypen an, um mit Webdiensten zu interagieren.

## Sales Insight {#sales-insight}

![(star)](assets/yellow-star.png)

* **Zugriffsberechtigungen für Sales Insight in Salesforce**: Administratoren können über den Berechtigungssatz der Marketo-App, der Teil des Salesforce-Pakets von Sales Insight ist, Sales Insight-Zugriff auf eine begrenzte Anzahl von Personen auf Benutzerebene und nicht auf Profilebene gewähren.

* **Meine Marketo-Kachelaktualisierung - Sales Insight-Aktionen**: Marketo-Administratoren (und die von ihnen benannten Benutzer) können jetzt über eine neue Kachel &quot;Sales Insight-Aktionen&quot;auf der Seite &quot;My Marketo&quot;schnell zu ihrer Sales Insight-Aktionsinstanz navigieren.

## Sales Connect {#sales-connect}

![(star)](assets/yellow-star.png)

* **Salesforce-API-Update**: Mit der Salesforce Summer 22-Version werden API-ältere Versionen 21-30 von Salesforce nicht mehr unterstützt. Mit dieser Marketo Engage-Version wurden alle Sales Connect-Anfragen, die ältere API-Versionen verwenden, aktualisiert, damit sie auf eine unterstützte Version passen. Klicken Sie für ausführliche Informationen zu den Salesforce API-Pensionsplänen auf [hier](https://help.salesforce.com/s/articleView?language=en_US&amp;type=1&amp;id=000354473){target="_blank"}.

## API-Verbesserungen {#api-enhancements}

* **Neue Filterfunktionen für die Bulk Program Member Extract API**: Filtern Sie nach Status der Programmmitgliedschaft, updatedAt, Cadence oder erschöpftem Inhalt, um den extrahierten Datensatz zu verfeinern.

* **Verbesserung der Bulk Program Member Extract API**: Geben Sie bis zu 10 Programme während der Auftragserstellung an, um den Durchsatz zu verbessern.

## Ankündigungen {#announcements}

* **Forms-Einstellung - Forms 1.0, Lead-Capture-/Speicherendpunkt und Nicht-Skriptversionen von Formularen**: Die Unterstützung für Forms 1.0-Assets wird bis Oktober 2022 vollständig aus dem Marketo Engage entfernt. Alle vorhandenen Forms 1.0-Assets funktionieren nicht mehr. Für Marketo Engage-Formulare muss JavaScript auf Landingpages und Websites geladen werden.

**_Webinar zur Produktversion_**

[Marketo Engage-Release-Webinar vom Juni und August 2022](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}
