---
description: Versionshinweise - Mai 2021 - Marketo Docs - Produktdokumentation
title: Versionshinweise - Mai 2021
translation-type: tm+mt
source-git-commit: b5d5e5895ca315976650123875777fe43854ea60
workflow-type: tm+mt
source-wordcount: '1490'
ht-degree: 0%

---

# Versionshinweise: Mai 2021 {#release-notes-may-21}

Die folgenden Funktionen sind in der Version vom 21. Mai enthalten. Überprüfen Sie Ihre Marketo Edition auf Funktionsverfügbarkeit.

>[!AVAILABILITY]
>
>Mit einem Stern gekennzeichnete Funktionen (![(star)](assets/star-yellow.svg)) werden kostenpflichtige Add-ons erstellt. Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zu erhalten.

**_Quartalsversionen_**

Die folgenden Funktionen werden am **7. Mai 2021** veröffentlicht.

## Kontobasierte Erlebnisse {#Account-based-eaperiences}

* **Intelligente Listen für Konto (allgemeine Verfügbarkeit)** (![(Stern)](assets/star-yellow.svg): Dynamische Identifizierung und Qualifizierung von Konten mit den gewünschten Konto- und Personalattributen zur Zielgruppe von Cross-Kanal-Marketing-Kampagnen und Versand von rechtzeitigen Warnungen an Vertrieb, um Transaktionen schneller abzuschließen. Diese neue Funktion ermöglicht eine robuste Automatisierung von kontobasierten Marketingstrategien. Für Kunden mit Zielgruppe-Kontoverwaltung, die über eine Benutzererfahrung der nächsten Generation verfügen, stehen Smart-Listen für Ihr Konto zur Verfügung.

## Benutzererlebnis der nächsten Generation {#next-generation-user-experience}

Mit der Vorschau der globalen Suche können Marketingexperten schnell erkennen, wo sich ein freigegebenes Asset in ihrer Instanz befindet. Die Browser-Registerkarten zeigen den Ort an, an dem Sie die Navigation in Marketing-Aktivitäten oder Design Studio verbessern können. Zusätzliche Filter für die Baumstruktur und die globale Suche helfen bei der Präzisierung Ihrer Suchkriterien. Die Drag &amp; Drop-Funktion in der Struktur wurde neu installiert, sodass Sie Ordner und Assets schnell und effizient innerhalb der Hauptanwendungsbereich verschieben können. Dank neu aktualisierter Symbole (die den Barrierefreiheitsstandards der Adobe entsprechen) und Statusmarkierungen können Marketingexperten schnell und einfach zwischen Ordnern und Assets in der Struktur unterscheiden und den Status von Programmen und Assets identifizieren.

## Erlebnisautomatisierung {#experience-automation}

* **Kampagne-Flow-Schritte** ausführen: Optimieren Sie die Erstellung Workflows Kampagnen und verbessern Sie die Leistung der Kampagne mit einem neuen Flussschritt für intelligente Kampagnen. Erstellen und speichern Sie zentralisierte Vorlagen für wiederholte Aufgaben in Ihrem Arbeitsbereich, wie z. B. die Normalisierung des Ländercodes, die über den neuen Flussschritt &quot;Kampagne ausführen&quot;von jeder Smart-Kampagne aus aufgerufen und ausgeführt werden sollen. Verknüpfte Kampagnen werden in der angegebenen Reihenfolge ausgeführt und stellen sicher, dass die Aufgabe abgeschlossen ist, bevor Sie zum nächsten Flussschritt wechseln. Bearbeiten Sie den Fluss schnell in nur einer zentralen Kampagne, um jede intelligente Kampagne zu aktualisieren, die ihn verwendet, um Data Management, Interessentenbewertung und Routing-Workflows zu optimieren.

## Kanal-Kreuzgang {#cross-channel-orchestration}

* **Sensible Datenfelder in Forms**: Die personenbezogenen Daten (PII) des Protect-Kunden können nicht in Marketo Engage-Formularen der Adobe angezeigt werden, indem Datenfelder als sensibel definiert und das Vorausfüllen der Formulare eingeschränkt wird. Wenn ein Besucher ein Formular auf der Landingpage Ansicht, zeigen die als sensibel definierten Felder keine vorausgefüllten Daten an.

* **Spam-Formularübermittlungen** blockieren: Protect Sie Ihre Adobe-Marketo Engage-Datenbank von Junk-Daten, die zu ungültigen Warnungen beim Vertrieb, Trigger-Kampagne-Rückständen und zu unerwünschten Aktivitäten führen können. Der neue Überprüfungsmechanismus lehnt ungültige Formularübermittlungen ab und stoppt Bot-Angriffe. Ihre Daten sind sauberer, und Ihre Marketing-Kampagnen laufen wie gewünscht, wodurch das Risiko, unqualifizierte Interessenten zu Verkäufen zu senden, minimiert wird.

* **Warnung zur Genehmigung** des E-Mail-Programms: Verhindern Sie das Senden fehlerhafter E-Mails, wenn die neuen Änderungen an einem zuvor genehmigten Programm vorgenommen wurden.  Die Warnung dient als Garantie, wenn ein Marketingspezialist Änderungen an einer bereits genehmigten E-Mail vornimmt, dann jedoch vergisst, die neuesten Änderungen zu genehmigen, und die E-Mail an eine große Audience ohne Inhalt, ungültigen Inhalt oder alten Inhalt sendet.

* **Einzelflussaktion auf der Interessentendetailseite**: Erlauben Sie Benutzern, über das Flussaktionen-Menü auf einzelnen Interessenten Aktionen wie das Senden von E-Mails, das Ändern des Interessenteneigentümers oder andere Aktionen zur intelligenten Kampagne auszuführen. Marketingexperten können Flussaktionen auf Interessenten ausführen, ohne zur Ansicht des Interessentendatenbankrasters wechseln zu müssen.

* **Aktivität** zum Herausfiltern von E-Mail-Bots: Mit der neuen Filterfunktion für E-Mail-Bot-Aktivitäten verhindern Sie unbeabsichtigte Verkaufswarnungen und ungenauen E-Mail-Berichte. Identifizieren und filtern Sie die angezeigten Links und Klicks, die mit E-Mail-Bots verknüpft werden können, um Links zu überprüfen, die zu falschen Triggern und Warnungen oder zu falschem Berichte führen.

## API-Verbesserungen {#api-enhancements}

Mehrere wichtige Aktualisierungen an Bulk- und Interessenten-APIs, darunter die Möglichkeit, benutzerdefinierte Objektdaten stapelweise zu exportieren, die Firma mit Interessenten in loser Schüttung zu verknüpfen, die Möglichkeit, Massenextrakte auf Basis eines Primärattributs zu filtern und die Programm-Mitgliedschaft zu erstellen und zu aktualisieren.

* **Ereignis-Programme** verschachteln: In Adobe Marketo Engage können Sie Ereignis-Programme unter anderen Programm-Typen erstellen, klonen oder verschieben. Diese Funktion ist jetzt in der Assets-API zulässig.

* **Erweiterte API zum Löschen von Programmen**: Ermöglicht integrierten Anwendungen das Löschen von Programmen mit zusätzlichen Asset-Typen, ohne dass die Benutzer dies manuell aus Adobe Marketo Engage tun müssen.

* **Mitgliedschaft** im Programm: Marketingexperten können alle Programm-Mitgliederdatensätze für ein bestimmtes Programm nach unterschiedlichen Kriterien, wie z. B. dem Status eines Programms, Abfrage werden. Geben Sie diese Informationen mit einer externen Anwendung, einem Business Intelligence-Tool oder Adobe Experience Cloud frei, um die Segmentierung zu verbessern und gezieltere Interaktionen zu erstellen.

* **Massenobjektextrahierung**: Der Massendatenexport ergänzt die Importfunktionen, die Datenanalysten bereits im Marketo Engage der Adobe nutzen. Jetzt können sie im Marketo Engage Benutzerdefinierte Objekte der 1. Adobe gespeicherte Daten stapelweise extrahieren, diese Daten in eine andere Anwendung, ein Data Warehouse oder ein BI-Tool (Business Intelligence) laden, um bessere Einblicke in die Daten in der Adobe Marketo Engage-Instanz zu erhalten.  Die Bewegung benutzerdefinierter Objektstapeldaten erfolgt bidirektional und kann zu einem günstigen Zeitpunkt geplant werden.

* **API** für benutzerdefinierte Felder-Metadaten: Sparen Sie Zeit, indem Sie die Erstellung benutzerdefinierter Marketo Engage automatisieren, während Sie Ihre Adobe-Systemintegrationen mit einer Drittanbieteranwendung einrichten. Diese Automatisierung kommt besonders Kunden mit mehreren Adoben-Marketo Engage-Instanzen zugute, die jetzt in der Lage sind, die Erstellung benutzerdefinierter Felder zu optimieren, für die in jedem Fall eine manuelle Arbeit erforderlich war. Optimieren Sie die Erstellung benutzerdefinierter Felder und sparen Sie Zeit für diese ressourcenintensive Aktivität.

* **Bulk Aktivität Extract API**: Erhalten Sie beim Durchführen von Massen-Extraktionen die Kontrolle über die Datenmenge und -art. Filtern Sie unnötige Datenpunkte und steuern Sie die Anzahl der API-Aufrufe, die erforderlich sind, um die Daten der Aktivität stapelweise zu extrahieren.  Wählen Sie beispielsweise offene E-Mails, besuchen Sie eine Webseite oder ändern Sie den Interessentenwert und lassen Sie andere Wertänderungen, die Sie nicht analysieren möchten, hinter sich. Straffen Sie den Prozess, um die Anzahl der API-Aufrufe und die Datenbereinigung zu verringern.

* **Interessenten-API**: Identifizieren Sie Interessenten im Adobe-Marketo Engage, denen Adobe-ECID (Experience Cloud-ID) zugeordnet ist.  Adobe-Marketo Engage-Kunden können eine Liste von Interessenten aus einer bestimmten Kampagne erstellen und mithilfe der ECIDs (Experience Cloud-ID) Berichte für diese bestimmte Liste in Adobe Analytics erstellen. Die Integration zwischen Adobe Marketo Engage und Adobe Experience Cloud eröffnet unbegrenzte Möglichkeiten für Segmentierung, Targeting und Berichte.

* **Bulk Lead Import API**: Kontrollieren Sie den Import und die benötigten Ressourcen. Diese Verbesserung schafft eine Verbindung zwischen Interessent und Firma während des Massenimportprozesses. Verbessern Sie die Effizienz und die Arbeit mit Daten und verringern Sie die Nutzung bei API-Aufrufen.

* **Web API-basierte Integration für Microsoft Dynamics Online-Kunden**: MS Dynamics Web API wurde mit Version 8.0 REST Protokoll eingeführt und implementiert OData (Open Data Protocol) v4. OData ist ein OASIS-Standard (Organisation zur Förderung von Strukturierten Informationsstandards) für den Aufbau und den Verbrauch von RESTful-Diensten über Rich Data. Adobe Marketo Engage-Kunden, die eine Integration mit Microsoft Dynamics mithilfe dieser Methode erfordern, werden derzeit von SOAP (Simple Object Access Protocol) zu einer Web API-basierten Verbindung migriert.

## Marketing-Daten-Umgebung {#marketing-data-environment}

* **XLSX-Export**: Wir haben die Exportfunktionen im gesamten Produkt aktualisiert, um XLSX anstelle von XLS zu unterstützen. Dies bedeutet, dass diese Option an jeder Stelle im Produkt, an der XLS-Export derzeit unterstützt wird, durch eine Option ersetzt wird, die stattdessen nach XLSX exportiert werden kann. Diese Änderung betrifft die Dateinamen für alle Excel-Exporte von Berichten und anderen Daten aus Adobe Marketo Engage.

* **Suche nach Interessenten-ID**: Greifen Sie schnell auf die Suche nach Interessentendatensätzen mit der Adobe Marketo Engage-Interessenten-ID in der Interessentendatenbank oder in der statischen Liste zu. Geben Sie im Fenster Schnellsuche einfach `[id]` mit der entsprechenden Nummer ein, dann werden die Interessenteninformationen angezeigt. Benutzer können schnell Einzelheiten zu Interessenten, Firmen oder Gelegenheiten überprüfen.

## Bizible {#bizible}

(![(star)](assets/star-yellow.svg))

* **Integration mit LinkedIn Lead Gen Forms (Beta)**: Mit der Bizible Premium Attribution Lösung erhalten Sie einen tiefen Einblick in Ihre LinkedIn Kanal-Ausgaben und Ihren ROI. Durch die neueste Integration mit LinkedIns Lead Gen Forms erhält Bizible Einblicke in Formulare, die auf der LinkedIn-Plattform eingereicht wurden. Diese Formularausfüllungen werden mit Interessenten aus Ihrer CRM- (Customer Relationship Management) oder Adobe-Marketo Engage-Instanz abgeglichen, sodass sie für eine Zuordnung infrage kommen und mit Ihren anderen Marketing-Interaktionen verfolgt werden können.

## Ankündigungen {#announcements}

* **Marketo Product Docs Switching-Plattformen**: Wir freuen uns, Ihnen mitteilen zu können, dass die Marketo Product Docs am Freitag, den 7. Mai, der Adobe Experience League beitreten werden. Sie können weiterhin die URL verwenden: docs.marketo.com und wenn bereits vorhandene Artikel mit Lesezeichen versehen sind, werden Sie umgeleitet. Alle aktuellen Produktdocs werden auf der neuen Plattform verfügbar sein, und für Ende des Jahres sind Verbesserungen geplant.

* **Optimierte Benutzerverwaltung und Single-Sign-On mit Adobe Identity System**: Ab Juli 2021 werden die neuen Adobe-Marketo Engage-Kunden mit Adobe-Benutzeranmeldeinformationen an Bord genommen. Bis Mitte 2022 erfolgt die Migration von aktuellen Kunden zum integrierten Identitätssystem. Bis auf Weiteres ist keine Kundenaktion erforderlich. Single Sign-On ermöglicht IT-/Security-Administratoren die Verwaltung mehrerer Adobe-Marketo Engage-Produktinstanzen zusammen mit anderen Experience Cloud-Lösungen sowie die Konfiguration der SSO (Shared Services Organization) über eine gemeinsame Konsole. Administratoren können Benutzergruppen und Benutzerberechtigungen bequem über eine gängige Admin Console verwalten.
