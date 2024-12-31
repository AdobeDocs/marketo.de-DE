---
description: Versionshinweise - Juni 2022 - Marketo-Dokumente - Produktdokumentation
title: Versionshinweise – Juni 2022
exl-id: f4438ea8-1657-4955-9f9f-640b3ecf5caa
feature: Release Information
source-git-commit: cf4dcb6a316eba631ccb73a991c09e83c80b82ca
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 1%

---

# Versionshinweise: Juni 2022 {#release-notes-june-22}

Im Folgenden finden Sie alle Funktionen, die in der Version vom Juni 2022 enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage Edition auf die Verfügbarkeit der Funktionen.

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie von Ihrem Marketo Engage-Support-Mitarbeiter.

Die folgenden Funktionen werden ab dem 24. **2022 veröffentlicht** wobei die verbleibenden Funktionen in den darauffolgenden Wochen schrittweise bereitgestellt werden (sofern nicht anders angegeben).

## Marketing-Datenumgebung {#marketing-data-environment}

* **Verfügbarmachen von CreatedAt/UpdatedAt-Feldern für benutzerdefinierte Objekte**: Ermöglicht es Ihnen, diese Felder im Bildschirm „Personendetails“ zu überprüfen, um zusätzliche Einblicke zu erhalten.

## Kanalübergreifende Orchestrierung {#cross-channel-orchestration}

* **Verbesserte Stream Designer-Benutzerfreundlichkeit für Dynamic Chat**: Fügen Sie Karten direkt von der Stream Designer-Arbeitsfläche hinzu, ohne dass Sie sie per Drag-and-Drop verschieben müssen. Außerdem wurde die Dynamic Chat-Oberfläche verbessert, um den Inhalt auf Einzelkarten besser sichtbar zu machen.

* **Erweiterte Terminrouting-Regeln für Dynamic Chat**: Dynamic Chat bietet mehr Optionen für zielgerichtetes Terminrouting. Geben Sie an, welche Agententermine auf der Grundlage von Marketo Engage-Attributen weitergeleitet werden sollen, um sicherzustellen, dass Leads an die entsprechenden Agenten weitergeleitet werden.

* **Erweiterte Dialogfeldberichte für Dynamic Chat**: Sehen Sie sich die Performance Ihrer Dynamic Chat-Kampagnen genauer an, indem Sie völlig neue Datenvisualisierungen für Interaktions- und Konversionsmetriken verwenden.

* **Nicht verwendete Marketo Engage-Attribute für Dynamic Chat synchronisieren**: Heben Sie die Synchronisierung von nicht verwendeten Marketo Engage-Attributen mit Ihrem Dynamic Chat-Abonnement auf. Dies erleichtert die Datenbereinigung und ermöglicht die Synchronisierung von Ersatzattributen nach Bedarf.

## Erlebnis der nächsten Generation

**Neue Umschaltansichten ein/aus**: Die folgenden Ansichten sind jetzt in der nächsten Generation verfügbar:

* [E-Mail-Detailansicht](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [E-Mail-Listenansicht](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## Experience Automation {#experience-automation}

* **Ausschlüsse für globale Formularfeldvalidierungsregeln**: Schließen Sie bestimmte Formulare von globalen Formularvalidierungsregeln aus, damit Abonnementzentren und andere geschäftskritische Workflows alle Werte akzeptieren können.

* **Self-Service-Flussschritte**: Erweitern Sie die Konnektivität zwischen Marketo Engage und dem Rest Ihres Stacks mit der Möglichkeit, benutzerdefinierte Flussschritte für die Verwendung in Smart-Kampagnen zu erstellen. Sowohl Marketo Engage-Benutzer als auch -Partner können diese Funktion nutzen, um die Verwendung externer Web-Services in Trigger-, Batch- und ausführbaren Kampagnen zu ermöglichen, im Gegensatz zu Webhooks, die nur in Trigger-Kampagnen verwendet werden können.

* **Munchkin Protocol Agnostic Link Tracking**: Erweitern Sie die Unterstützung für das Tracking von `tel`- und `mailto`-Links mit Munchkin, um erweiterte Webverhaltensweisen zu verfolgen.

* **Zusätzliche HTTP-Methoden für Webhooks**: Geben Sie PUT, PATCH und DELETE als Anfragetypen für die Interaktion mit Webservices an.

## Sales Insight {#sales-insight}

![(Stern)](assets/yellow-star.png)

* **Berechtigungssatz für Sales Insight in Salesforce**: Administratoren können über den Berechtigungssatz für Marketo-Apps, der Teil des Salesforce-Pakets für Sales Insight ist, Sales Insight einer begrenzten Gruppe von Personen auf Benutzerebene statt auf Profilebene Zugriff gewähren.

* **Mein Marketo-Kachel-Update - Sales Insight-Aktionen**: Marketo-Administratoren (und von ihnen benannte Benutzer) können jetzt über eine neue Kachel „Sales Insight-Aktionen“ auf der Seite Mein Marketo schnell zu ihrer Sales Insight-Aktionsinstanz navigieren.

## Sales Connect {#sales-connect}

![(Stern)](assets/yellow-star.png)

* **Salesforce-API-Update**: Mit der Salesforce-Version Sommer 2022 werden ältere API-Versionen 21-30 von Salesforce nicht mehr unterstützt. Mit dieser Marketo Engage-Version wurden alle Sales Connect-Anfragen, die ältere API-Versionen verwenden, so aktualisiert, dass sie innerhalb einer unterstützten Version bleiben. Ausführliche Informationen zu Salesforce-API-Pensionsplänen finden Sie [hier](https://help.salesforce.com/s/articleView?language=en_US&amp;type=1&amp;id=000354473){target="_blank"}.

## API-Verbesserungen {#api-enhancements}

* **Neue Filterfunktionen für die API zum Extrahieren von Massenprogrammmitgliedern**: Filtern nach Programmmitgliedschaftsstatus, updatedAt, Kadenz oder erschöpftem Inhalt, um den extrahierten Datensatz zu verfeinern.

* **Verbesserung der API für die Massenprogrammextraktion**: Geben Sie während der Auftragserstellung bis zu 10 Programme an, um den Durchsatz zu verbessern.

## Ankündigungen {#announcements}

* **Einstellung von Forms - Forms 1.0, Lead-Erfassungs-/Speicherendpunkt und No-Script-Versionen von Forms**: Die Unterstützung für Forms 1.0-Assets wird bis Oktober 2022 vollständig vom Marketo Engage entfernt. Alle vorhandenen Forms 1.0-Assets funktionieren nicht mehr. Beim Marketo Engage von Formularen muss JavaScript auf Landingpages und Websites geladen werden.

**_Webinar zur Produktversion_**

[Webinar zur Marketo Engage-Version vom Juni und August 2022](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}
