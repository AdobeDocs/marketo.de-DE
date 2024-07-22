---
description: Versionshinweise - Mai 2021 - Marketo-Dokumente - Produktdokumentation
title: Mai 2021 - Versionshinweise
exl-id: e3de60a2-17bd-4760-848e-6e931ad85b3c
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1450'
ht-degree: 0%

---

# Mai 2021 - Versionshinweise {#release-notes-may-21}

Die folgenden Funktionen sind in der Version vom 21. Mai enthalten. Überprüfen Sie Ihre Marketo-Edition auf Funktionsverfügbarkeit.

>[!AVAILABILITY]
>
>Mit einem Stern (![](assets/yellow-star.png)) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Wenden Sie sich an Ihren Marketo Engage-Support-Mitarbeiter, um mehr zu erfahren.

**_Vierteljährliche Versionen_**

Die folgenden Funktionen werden am **7. Mai 2021** veröffentlicht.

## Kontobasierte Erlebnisse {#Account-based-eaperiences}

* **Konto-Smart-Listen (allgemeine Verfügbarkeit)** ![](assets/yellow-star.png): Identifizieren und qualifizieren Sie Konten mit gewünschten Konto- und Personalattributen dynamisch, um Targeting in kanalübergreifenden Marketing-Kampagnen durchzuführen und rechtzeitige Warnungen an den Vertrieb zu senden, damit Geschäfte schneller geschlossen werden. Diese neue Funktion ermöglicht eine robuste Automatisierung kontobasierter Marketingstrategien. Smart-Listen für Konten sind für Kunden mit Target-Kontoverwaltung verfügbar, die sich auf dem Benutzererlebnis der nächsten Generation befinden.

## Benutzererlebnis der nächsten Generation {#next-generation-user-experience}

Mit der globalen Suchvorschau können Marketingexperten schnell erkennen, wo sich ein freigegebenes Asset in ihrer Instanz befindet. Browser-Registerkarten zeigen den Speicherort an, um die Navigation in Marketing Activities oder Design Studio zu verbessern. Zusätzliche Baumstruktur und globale Suchfilter helfen bei der Feinabstimmung Ihrer Suchkriterien. Die Drag-and-Drop-Funktion innerhalb des Baums wurde neu aktiviert, sodass Sie Ordner und Assets schnell und effizient in die wichtigsten App-Bereiche verschieben können. Dank neu aktualisierter Symbole (die den Barrierefreiheitsstandards von Adobe entsprechen) und Statusabzeichen können Marketingexperten schnell und einfach im Baum zwischen Ordnern und Assets unterscheiden und den Status von Programmen und Assets ermitteln.

## Erlebnisautomatisierung {#experience-automation}

* **Kampagnenflussschritte ausführen**: Optimieren Sie die Arbeitsabläufe zur Kampagnenerstellung und verbessern Sie die Kampagnenleistung mit einem neuen Flussschritt für Smart-Kampagnen. Erstellen und speichern Sie zentralisierte Vorlagenkampagnen für sich wiederholende Aufgaben in Ihrem Arbeitsbereich, wie z. B. die Normalisierung des Ländercodes, die über den neuen Workflow &quot;Kampagne ausführen&quot;von jeder Smart-Kampagne aus aufgerufen und ausgeführt werden können. Verknüpfte Kampagnen werden in der angegebenen Reihenfolge ausgeführt und stellen sicher, dass die Aufgaben abgeschlossen sind, bevor zum nächsten Flussschritt gewechselt wird. Bearbeiten Sie den Fluss schnell in nur einer zentralisierten Kampagne, um jede Smart-Kampagne zu aktualisieren, die sie verwendet, um die Datenverwaltung, die Lead-Scoring- und Routing-Workflows zu optimieren.

## Kanalübergreifende Orchestrierung {#cross-channel-orchestration}

* **Vertrauliche Datenfelder in Forms**: Die personenbezogenen Daten des Protect-Kunden können nicht in Adobe Marketo Engage-Formularen angezeigt werden, indem Datenfelder als vertraulich definiert und die Formularvorbelegung für diese Felder eingeschränkt wird. Wenn ein Besucher ein Formular auf der Landingpage anzeigt, zeigen die als vertraulich definierten Felder keine vorausgefüllten Daten an.

* **Spam Form Submissions**: Protect Ihre Adobe Marketo Engage-Datenbank anhand von Junk-Daten, die zu ungültigen Warnhinweisen für den Vertrieb, Trigger-Kampagnen-Rückläufen und unerwünschten Aktivitäten führen können. Der neue Validierungsmechanismus lehnt ungültige Formularübermittlungen ab und stoppt Bot-Angriffe. Ihre Daten sind sauberer, und Ihre Marketing-Kampagnen werden wie gewünscht ausgeführt, wodurch das Risiko minimiert wird, unqualifizierte Leads zum Verkauf zu senden.

* **Warnung zur E-Mail-Programmgenehmigung**: Verhindern Sie den Versand fehlerhafter E-Mails, wenn die neuen Änderungen an einem zuvor genehmigten Programm vorgenommen wurden.  Die Warnung dient als Schutz, wenn ein Marketing-Experte Änderungen an einer bereits genehmigten E-Mail vornimmt, dann aber vergisst, die neuesten Änderungen zu genehmigen, und die E-Mail an eine große Zielgruppe ohne Inhalt, ungültigen Inhalt oder alten Inhalt sendet.

* **Aktivität &quot;E-Mail-Bots filtern&quot;**: Verhindern Sie unbeabsichtigte Verkaufswarnungen und falsche E-Mail-Berichte über die neue Funktion zum Filtern von E-Mail-Bot-Aktivitäten. Ermitteln und filtern Sie Öffnungen und Klicks, die E-Mail-Bots zugeordnet werden können, indem Sie Links überprüfen, die zu falschen Triggern und Verkaufswarnungen oder falschen Berichten führen.

## API-Verbesserungen {#api-enhancements}

Mehrere wichtige Aktualisierungen an Bulk- und Lead-APIs, darunter die Möglichkeit, benutzerdefinierte Objektdaten stapelweise zu exportieren, Unternehmen mit Lead in Batches zu verknüpfen, die Möglichkeit, die Massenextraktion von Aktivitäten anhand eines Primärattributs zu filtern und die Möglichkeit, Programmmitgliedschaften zu erstellen und zu aktualisieren.

* **Ereignisprogramme verschachteln**: In Adobe Marketo Engage können Sie Ereignisprogramme unter anderen Programmtypen erstellen, klonen oder verschieben. Diese Funktion ist jetzt in der Assets-API zulässig.

* **Verbesserte Löschprogramm-API**: Ermöglicht integrierten Anwendungen das Löschen von Programmen, die zusätzliche Asset-Typen enthalten, ohne dass Benutzer dies manuell über Adobe Marketo Engage tun müssen.

* **Programmmitgliedschaft**: Marketingexperten können alle Einträge von Programmmitgliedern für ein ausgewähltes Programm abfragen, sofern unterschiedliche Kriterien wie z. B. der Status von Programmmitgliedern erfüllt sind. Geben Sie diese Informationen für eine externe Anwendung, ein Business Intelligence-Tool oder Adobe Experience Cloud frei, um die Segmentierung zu verbessern und gezieltere Interaktionen zu erstellen.

* **Massenextraktion benutzerdefinierter Objekte**: Der Massendatenexport ergänzt die Importfunktionen, die Datenanalysten bereits in Adobe Marketo Engage nutzen. Jetzt können sie in Adobe Marketo Engage benutzerdefinierte Objekte der ersten Ebene gespeicherte Daten stapelweise extrahieren und diese Daten in eine andere Anwendung, Data Warehouse oder ein BI-Tool (Business Intelligence) laden, um bessere Einblicke in die Daten in der Adobe Marketo Engage-Instanz zu erhalten.  Die Massenbewegung benutzerdefinierter Objekte erfolgt bidirektional und kann zu einem bequemen Zeitpunkt geplant werden.

* **Benutzerdefinierte Felder-Metadaten-API**: Sparen Sie Zeit, indem Sie die Erstellung benutzerdefinierter Felder automatisieren, während Sie Ihre Adobe Marketo Engage-Integrationen mit einer Drittanbieteranwendung einrichten. Diese Automatisierung kommt insbesondere Kunden mit mehreren Adobe Marketo Engage-Instanzen zugute, die jetzt in der Lage sind, die Erstellung benutzerdefinierter Felder zu optimieren, für die in jeder Instanz manuelle Arbeit erforderlich war. Optimieren Sie die Erstellung benutzerdefinierter Felder und sparen Sie Zeit für diese ressourcenintensive Aktivität.

* **Bulk Activity Extract API**: Gewinnen Sie Kontrolle über die Menge und den Typ der Daten bei der Durchführung von Massenextraktionen. Filtern Sie unnötige Datenpunkte und steuern Sie die Anzahl der API-Aufrufe, die erforderlich sind, um Aktivitätsdaten stapelweise zu extrahieren.  Wählen Sie beispielsweise offene E-Mails aus, besuchen Sie eine Webseite oder ändern Sie den Lead-Punktstand und lassen Sie andere Wertänderungen, die Sie nicht analysieren möchten, zurück. Optimieren Sie den Prozess, um die Anzahl der API-Aufrufe und die Datenbereinigung zu verringern.

* **Lead-API**: Identifizieren Sie Leads in Adobe Marketo Engage, denen Adobe ECID (Experience Cloud-ID) zugeordnet ist.  Adobe Marketo Engage-Kunden können eine Liste von Leads aus einer ausgewählten Kampagne erstellen und die ECIDs (Experience Cloud-ID) verwenden, um in Adobe Analytics Berichte für diese spezifische Liste zu erstellen. Die Integration zwischen Adobe Marketo Engage und Adobe Experience Cloud eröffnet unbegrenzte Möglichkeiten für Segmentierung, Targeting und Reporting.

* **Bulk Lead Import API**: Steuern Sie den Massenimport von Leads und benötigte Ressourcen. Diese Verbesserung schafft eine Verbindung zwischen Lead und Unternehmen beim Massenimport von Leads. Erhöhen Sie die Effizienz und die Arbeit mit Daten und verringern Sie die Nutzung bei API-Aufrufen.

* **Web API-basierte Integration für die Microsoft Dynamics Online-Kunden**: Die MS Dynamics Web API wurde mit Version 8.0 REST-Protokoll eingeführt und implementiert OData (Open Data Protocol) v4. OData ist ein OASIS-Standard (Organization for the Advancement of Structured Information Standards) zum Erstellen und Verwenden von RESTful-Diensten im Vergleich zu Rich-Data. Adobe Marketo Engage-Kunden, die mithilfe dieser Methode eine Integration mit Microsoft Dynamics erfordern, werden derzeit von SOAP (Simple Object Access Protocol) zu einer Web-API-basierten Verbindung migriert.

## Marketing-Datenumgebung {#marketing-data-environment}

* **XLSX-Export**: Wir haben die Exportfunktionen im gesamten Produkt aktualisiert, um XLSX anstelle von XLS zu unterstützen. Dies bedeutet, dass diese Option an jeder Stelle im Produkt, an der der XLS-Export derzeit unterstützt wird, durch eine Option zum Exportieren nach XLSX ersetzt wird. Diese Änderung betrifft die Dateinamen aller Excel-Exporte von Berichten und anderen Daten aus Adobe Marketo Engage.

* **Suche nach Lead-ID**: Schneller Zugriff auf die Lead-Datensatz-Suche nach Adobe Marketo Engage-Lead-ID in der Lead-Datenbank oder statischen Liste. Geben Sie im Fenster Schnellsuche einfach `[id]` mit der entsprechenden Nummer ein. Daraufhin werden die Lead-Informationen angezeigt. Benutzer können schnell Lead-, Unternehmens- oder Opportunity-Details überprüfen.

## Bizible {#bizible}

![](assets/yellow-star.png)

* **Integration mit LinkedIn Lead Gen Forms (Beta)**: Verschaffen Sie sich einen umfassenden Einblick in Ihre LinkedIn-Kanalausgaben und Ihren ROI mit der Bizible Premium-Zuordnungslösung. Durch die neueste Integration mit LinkedIns Lead Gen Forms erhält Bizible Einblicke in Formulare, die auf der LinkedIn-Plattform eingereicht wurden. Diese Formularausfüllungen werden mit Leads aus Ihrer CRM-Instanz (Customer Relationship Management) oder Adobe Marketo Engage-Instanz abgeglichen, sodass sie für die Attribution infrage kommen und anhand Ihrer anderen Marketing-Interaktionen verfolgt werden können.

## Ankündigungen {#announcements}

* **Marketo Product Docs Switching Platforms**: Wir freuen uns, Ihnen mitteilen zu können, dass die Marketo Product Docs seit Freitag, dem 7. Mai, der Adobe Experience League beigetreten sind. Sie können weiterhin die URL docs.marketo.com verwenden. Wenn Sie bereits vorhandene Artikel mit einem Lesezeichen versehen haben, werden Sie umgeleitet. Alle Produktdokumente sind auf der neuen Plattform verfügbar, für Ende des Jahres sind Verbesserungen geplant.

* **Optimierte Benutzerverwaltung und Single Sign-on mit Adobe Identity System**: Ab Juli 2021 werden die neuen Adobe Marketo Engage-Kunden mit Adobe-Benutzeranmeldeinformationen integriert. Die Migration von aktuellen Kunden zum integrierten Identitätssystem erfolgt erst Mitte 2022 und es ist bis auf Weiteres keine Kundenaktion erforderlich. Single Sign-On ermöglicht IT-/Sicherheitsadministratoren die Verwaltung mehrerer Adobe Marketo Engage-Produktinstanzen zusammen mit anderen Experience Cloud-Lösungen sowie die Konfiguration von SSO (Shared Services Organization) über eine gemeinsame Konsole. Administratoren können Benutzergruppen und Benutzerberechtigungen bequem über eine gemeinsame Admin Console verwalten.

**_Webinar zur Produktversion_**

[Marketo Engage-Release-Webinar vom Mai 2021](https://engage.marketo.com/May_21_Release_webinar_RegistrationPage.html)
