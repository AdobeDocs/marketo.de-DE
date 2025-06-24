---
description: Versionshinweise - Juni 2022 - Marketo-Dokumente - Produktdokumentation
title: Versionshinweise – Juni 2022
exl-id: f4438ea8-1657-4955-9f9f-640b3ecf5caa
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# Versionshinweise: Juni 2022 {#release-notes-june-22}

Im Folgenden finden Sie alle Funktionen, die in der Version vom Juni 2022 enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage Edition auf die Verfügbarkeit der Funktionen.

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie vom Marketo Engage-Support.

Die folgenden Funktionen werden ab dem 24. **2022 veröffentlicht** wobei die verbleibenden Funktionen in den darauffolgenden Wochen schrittweise bereitgestellt werden (sofern nicht anders angegeben).

## Marketing-Datenumgebung {#marketing-data-environment}

* **Verfügbarmachen von CreatedAt/UpdatedAt-Feldern für benutzerdefinierte Objekte**: Ermöglicht es Ihnen, diese Felder im Bildschirm „Personendetails“ zu überprüfen, um zusätzliche insight zu erhalten.

## Kanalübergreifende Orchestrierung {#cross-channel-orchestration}

* **Verbesserte Benutzerfreundlichkeit von Stream Designer für[!DNL Dynamic Chat]**: Fügen Sie Karten direkt von der Arbeitsfläche von Stream Designer hinzu, ohne dass Sie sie per Drag-and-Drop verschieben müssen. Außerdem wurde die [!DNL Dynamic Chat] verbessert, um eine bessere Sichtbarkeit der Inhalte in einzelnen Karten zu ermöglichen.

* **Erweiterte Terminrouting-Regeln für[!DNL Dynamic Chat]**: [!DNL Dynamic Chat] bietet mehr Optionen für zielgerichtetes Terminrouting. Geben Sie an, welche Agententermine auf der Grundlage von Marketo Engage-Attributen weitergeleitet werden sollen, um sicherzustellen, dass Leads an die entsprechenden Agenten weitergeleitet werden.

* **Erweiterte Dialogfeldberichte für[!DNL Dynamic Chat]**: Sehen Sie sich die Leistung Ihrer [!DNL Dynamic Chat] Kampagnen genauer an, indem Sie völlig neue Datenvisualisierungen für Interaktions- und Konversionsmetriken verwenden.

* **Nicht verwendete Marketo Engage-Attribute für[!DNL Dynamic Chat]** synchronisieren: Heben Sie die Synchronisierung von nicht verwendeten Marketo Engage-Attributen mit Ihrem [!DNL Dynamic Chat] auf, um die Datenbereinigung zu erleichtern und alternative Attribute nach Bedarf zu synchronisieren.

## Erlebnis der nächsten Generation

**Neue Umschaltansichten ein/aus**: Die folgenden Ansichten sind jetzt in der nächsten Generation verfügbar:

* [E-Mail-Detailansicht](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-details-view){target="_blank"}
* [E-Mail-Listenansicht](/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md#email-list-view){target="_blank"}

## Experience Automation {#experience-automation}

* **Ausschlüsse für globale Formularfeldvalidierungsregeln**: Schließen Sie bestimmte Formulare von globalen Formularvalidierungsregeln aus, damit Abonnementzentren und andere geschäftskritische Workflows alle Werte akzeptieren können.

* **Self-Service-Flussschritte**: Erweitern Sie die Konnektivität zwischen Marketo Engage und dem Rest Ihres Stacks mit der Möglichkeit, benutzerdefinierte Flussschritte für die Verwendung in Smart-Kampagnen zu erstellen. Sowohl Marketo Engage-Benutzer als auch -Partner können diese Funktion nutzen, um die Verwendung externer Web-Services in Trigger-, Batch- und ausführbaren Kampagnen zu ermöglichen. Im Gegensatz zu Webhooks, die nur in Trigger-Kampagnen verwendet werden können.

* **Munchkin Protocol Agnostic Link Tracking**: Erweitern Sie die Unterstützung für das Tracking von `tel`- und `mailto`-Links mit Munchkin, um erweiterte Webverhaltensweisen zu verfolgen.

* **Zusätzliche HTTP-Methoden für Webhooks**: Geben Sie PUT, PATCH und DELETE als Anfragetypen für die Interaktion mit Webservices an.

## [!DNL Sales Insight] {#sales-insight}

![(Stern)](assets/yellow-star.png)

* **[!DNL Sales Insight]Berechtigungssatz in[!DNL Salesforce]**: Administratoren können über den Berechtigungssatz für Marketo-Apps, der Teil des [!DNL Sales Insight]-[!DNL Salesforce] ist, [!DNL Sales Insight] Zugriff für eine begrenzte Anzahl von Personen auf Benutzerebene statt auf Profilebene gewähren.

* **Mein Marketo-Kachel-Update - [!DNL Sales Insight] Aktionen**: Marketo-Administratoren (und von ihnen benannte Benutzer) können jetzt über eine neue Kachel [!DNL Sales Insight] Aktionen auf der Seite Mein Marketo schnell zu ihrer [!DNL Sales Insight]-Instanz navigieren.

## [!DNL Sales Connect] {#sales-connect}

![(Stern)](assets/yellow-star.png)

* **[!DNL Salesforce]API-Update**: Mit der [!DNL Salesforce] Summer &#39;22-Version werden die API-Legacy-Versionen 21 bis 30 von [!DNL Salesforce] nicht mehr unterstützt. Mit dieser Marketo Engage-Version wurden alle [!DNL Sales Connect], die ältere API-Versionen verwenden, so aktualisiert, dass sie innerhalb einer unterstützten Version bleiben. Ausführliche Informationen zu [!DNL Salesforce] API-Pensionsplänen finden Sie [hier](https://help.salesforce.com/s/articleView?language=en_US&type=1&id=000354473){target="_blank"}.

## API-Verbesserungen {#api-enhancements}

* **Neue Filterfunktionen für die API zum Extrahieren von Massenprogrammmitgliedern**: Filtern nach Programmmitgliedschaftsstatus, updatedAt, Kadenz oder erschöpftem Inhalt, um den extrahierten Datensatz zu verfeinern.

* **Verbesserung der API für die Massenprogrammextraktion**: Geben Sie während der Auftragserstellung bis zu 10 Programme an, um den Durchsatz zu verbessern.

## Ankündigungen {#announcements}

* **Einstellung von Forms - Forms 1.0, Lead-Erfassungs-/Speicherendpunkt und No-Script-Versionen von Forms**: Die Unterstützung für Forms 1.0-Assets wird bis Oktober 2022 vollständig aus Marketo Engage entfernt. Alle vorhandenen Forms 1.0-Assets funktionieren nicht mehr. Marketo Engage-Formulare erfordern, dass JavaScript auf Landingpages und Websites geladen wird.

**_Webinar zur Produktversion_**

[Webinar zur Marketo Engage-Version Juni und August 2022](https://engage.marketo.com/2022_June_August_Release_Webinar_OnDemandPage.html){target="_blank"}
