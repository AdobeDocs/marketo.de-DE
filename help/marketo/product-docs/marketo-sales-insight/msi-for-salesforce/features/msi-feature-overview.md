---
unique-page-id: 37356893
description: Übersicht über die MSI-Funktionen - Marketing-Dokumente - Produktdokumentation
title: Übersicht über die MSI-Funktionen
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '916'
ht-degree: 0%

---


# Übersicht über die MSI-Funktionen {#msi-feature-overview}

MSI verfügt über die folgenden Funktionen in Salesforce Lightning und Classic.

## Visualforce-Bedienfeld {#visualforce-panel}

MSI Visualforce Panel umfasst die folgenden Funktionen:

* Registerkarten

   * [Insight-Dashboard](http://docs.marketo.com/x/EoGMAg)
   * Interessanter Moment
   * Web-Aktivität
   * Email
   * Ergebnis

* Aktionen

   * hinzufügen zur Kampagne von Marketo
   * E-Mail an Marke senden
   * hinzufügen/Entfernen aus der überwachten Liste

* Sterne und Flammen

## Interessentenlayout {#lead-layout}

Visualforce-Seiten:

* Interessenten - Enthält die Option zum Klicken auf die Unterschrift &quot;Zur vollen Liste&quot;, werden Sie zu einer neuen Registerkarte in Salesforce gesendet, wo das MSI-Bedienfeld in einem ganzseitigen Layout angezeigt wird
* Interessentenvolle Liste - Enthält nicht die Option &quot;Gehe zu voller Liste&quot;
* Interessentenmobil - Sichtbar in Salesforce-Mobilanwendung
* InteressentenkontaktBridge - Zeigt den Bereich &quot;MSI&quot;des Kontakts an, den Sie im Feld &quot;MSI-Kontakt-ID&quot;hinzugefügt haben

Felder:

* Letzter interessanter Moment
* Datum des letzten interessanten Moments
* Letzter interessanter Moment Desc
* Letzter interessanter Moment Quelle
* Letzter interessanter Moment-Typ
* Letzte Aktivität nach Vertrieb
* Letzte Marketinginteraktion nach Vertrieb
* Relative Bewertung
* relativer Score-Wert
* Dringlichkeit
* Dringlichkeitswert
* Ansicht in Marketo - Klicken Sie auf dieses Feld, um eine nicht bearbeitbare Ansicht des Interessenten in Marketo zu öffnen. Umfasst: Interessenteninformationen, Firmen-Info, SFDC-Interessenteninformationen, benutzerdefinierte SFDC-Felder, Aktivitäten-Protokoll
* MSI-Kontakt-ID - Hinzufügen einem Salesforce-Kontakt zu diesem Feld und fügen Sie das Bedienfeld &quot;Interessenten-Kontakt-Bridge&quot;in das Interessentenlayout ein, um das MSI-Bedienfeld des Kontakts anzuzeigen

## Kontaktlayout {#contact-layout}

Visualforce-Seiten:

* Kontakt - Umfasst die Option zum Klicken auf die Hyper-Schaltfläche &quot;Zur vollen Liste gehen&quot;, werden Sie zu einer neuen Registerkarte in Salesforce gesendet, wo das MSI-Bedienfeld in einem ganzseitigen Layout angezeigt wird
* Volle Liste kontaktieren - enthält keine Option &quot;Zur vollen Liste gehen&quot;
* Contact Mobile - Sichtbar in Salesforce-Mobilanwendung
* Kontaktseite Hinzufügen zur Marketing-Kampagne - Funktion Hinzufügen zur Marketing-Kampagne ist in diesem Bereich verfügbar

Felder:

* Letzter interessanter Moment
* Datum des letzten interessanten Moments
* Letzter interessanter Moment Desc
* Letzter interessanter Moment Quelle
* Letzter interessanter Moment-Typ
* Letzte Aktivität nach Vertrieb
* Relative Bewertung
* relativer Score-Wert
* Dringlichkeit
* Dringlichkeitswert
* Ansicht in Marketo - Klicken Sie auf dieses Feld, um eine nicht bearbeitbare Ansicht des Interessenten in Marketo zu öffnen. Umfasst: Interessenteninformationen, Firmen-Info, SFDC-Interessenteninformationen, benutzerdefinierte SFDC-Felder, Aktivitäten-Protokoll
* MKTO-Interessentenbewertung
* Sales Insight - Öffnet die Seite mit der vollständigen Liste

## Kontolayout {#account-layout}

Visualforce-Seiten:

* Konto - Umfasst die Option zum Klicken auf die Hyper-Schaltfläche &quot;Zur vollen Liste gehen&quot;, werden Sie zu einem neuen Register in Salesforce gesendet, wo das MSI-Bedienfeld in einem ganzseitigen Layout angezeigt wird
* Vollständige Liste des Kontos - Option &quot;Zur vollen Liste gehen&quot;ist nicht enthalten
* Account Mobile - Sichtbar in der mobilen Anwendung Salesforce

Felder:

* Sales Insight - Öffnet die Seite mit der vollständigen Liste

Die folgenden Funktionen stehen auf der Seite &quot;Kontolayout&quot;nicht zur Verfügung:****

* Aktionen: hinzufügen zur Kampagne von Marketing, E-Mail senden von Marketing, Hinzufügen/Entfernen aus der Liste
* Sterne und Flammen

## Opportunity Layout {#opportunity-layout}

Visualforce-Seiten:

* Gelegenheit - Enthält die Option zum Klicken auf die Unterschrift &quot;Zur vollen Liste gehen&quot;, werden Sie zu einer neuen Registerkarte in Salesforce gesendet, wo das MSI-Bedienfeld in einem vollständigen Seitenlayout angezeigt wird
* Vollständige Liste der Gelegenheit - Option &quot;Zur vollen Liste gehen&quot;ist nicht enthalten
* Opportunity Mobile - Sichtbar in Salesforce-Mobilanwendung

Felder:

* Sales Insight - Öffnet die Seite mit der vollständigen Liste
* Analyse von Marketo-Chancen - eröffnet Einflussanalyse für Chancen in Marketing

Die folgenden Funktionen sind auf der Seite &quot;Opportunity Layout&quot;nicht verfügbar: **Nicht verfügbar**:

* Aktionen: hinzufügen zur Kampagne von Marketing, E-Mail senden von Marketing, Hinzufügen/Entfernen aus der Liste
* Sterne und Flammen

## Ansicht der Interessenten- und Kontaktpersonen-Liste (Massenaktionen) {#lead-and-contact-list-view-bulk-actions}

Salesforce-Blitz: hinzufügen der Aktionsschaltflächen für die Massenaktion &quot;&quot;, &quot;Hinzufügen&quot;, &quot;Marketo-Kampagne&quot;und &quot;Senden von E-Mail an E-Mail an die Kontaktanfrage&quot;in der Ansicht &quot;Interessenten- und Kontaktaufnahme&quot;der Liste.

Salesforce Classic: hinzufügen in der Ansicht &quot;Lead- und Kontaktaufnahme&quot;die Schaltflächen für Massenaktionen für-, Hinzufügen- und Marketing-Kampagne und Senden von E-Mail-Nachrichten.

## Marketo-Registerkarte {#marketo-tab}

* Beste Betas

   * Umfasst die Möglichkeit, Ansichten zu erstellen und zu bearbeiten. Möglichkeit zum Ausblenden der besten Einsätze abhängig von der Konfiguration der Option &quot;Standardausblenden&quot;auf der Seite &quot;Konfiguration von Marketing&quot;
   * Spalten - Name, Konto, letzter interessanter Moment, Statusüberschrift, Interaktion (Sterne und Flammen), Ausblenden

* Meine Watch-Liste

   * Möglichkeit zum Erstellen und Bearbeiten von Ansichten
   * Spalten - Name, Konto, letzter interessanter Moment, Statusüberschrift, Interaktion (Sterne und Flammen), Entfernen

* Web-Aktivität

   * Umfasst die Möglichkeit, Ansichten zu erstellen und zu bearbeiten, Funktionen für Zeitraumfilter
   * Spalte - Ansicht der Seite, Name, Konto, Letzter Besuch

* Anonyme Web-Aktivität

   * Umfasst die Möglichkeit, Ansichten zu erstellen und zu bearbeiten, Funktionen für Zeitraumfilter
   * Spalten - Ansicht der Seite, Firma, Letzter Besuch, Suche (öffnet die LinkedIn-Seite der Firma)

* Meine E-Mail

   * Möglichkeit zum Erstellen und Bearbeiten von Ansichten
   * Spalten - Name, Konto, Betreff, Datum, Öffnen, Klicken

* Interessentenfeed - Enthält die Möglichkeit, interessante Momente zu abonnieren, muss RSS-Feed auf der Konfigurationsseite aktiviert werden, damit diese Funktion verwendet werden kann

   * Interessanter Moment
   * Interessanter Moment (Web, E-Mail oder Meilenstein) und Beschreibung
   * Kontoname
   * Zeit, die dieser interessante Moment
   * Option &quot;Abonnieren&quot;zum Empfangen von E-Mail-Benachrichtigungen für diesen Ereignis
   * Symbol mit hoher Priorität, um diese Person zu zeigen, ist eine beste Wette

## Registerkarte &quot;Konfiguration von Marketing-Sales Insight&quot; {#marketo-sales-insight-configuration-tab}

* Betriebseinstellungen: Beinhaltet die für die Einrichtung von MSI in SFDC erforderlichen Soap- und Rest-API-Anmeldeinformationen
* MSI-Konfiguration: Umfasst die Konfiguration der Registerkarte &quot;Marketo&quot;und des MSI Visualforce-Bedienfelds
* Zurücksetzen von Marketing auf Sales Insight: Beinhaltet die Möglichkeit, alle Konfigurationen zu löschen

>[!MORELIKETHIS]
>
>[Registerkarte &quot;Konfiguration von Marketing zu Sales Insight&quot;in Salesforce](http://docs.marketo.com/x/UoCMAg)

## Sales Insight-Leistungsberichte {#sales-insight-performance-reports}

Ansicht der Leistung von E-Mails, die über Salesforce, Microsoft Dynamics oder ein Gmail- oder Outlook-Plugin gesendet werden

## MSI for Mobile {#msi-for-mobile}

MSI-Funktionen werden in der Salesforce-Mobilanwendung unterstützt

## Sprachunterstützung {#language-support}

Marketo Sales Insight wird nach Sprache gespeichert. Wenn Sie also möchten, dass es für mehr als eine Sprache funktioniert, müssen Sie die Anmeldeinformationen für jede Sprache einzeln eingeben.
