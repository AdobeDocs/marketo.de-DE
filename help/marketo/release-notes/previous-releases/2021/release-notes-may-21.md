---
description: Mai 2021 - Versionshinweise zu Marketo - Produktdokumentation
title: Mai 2021 - Versionshinweise
exl-id: e3de60a2-17bd-4760-848e-6e931ad85b3c
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '1440'
ht-degree: 0%

---

# Mai 2021 - Versionshinweise {#release-notes-may-21}

Die folgenden Funktionen sind in der Version vom Mai 2021 enthalten. Überprüfen Sie Ihre Marketo Edition auf die Verfügbarkeit der Funktionen.

>[!AVAILABILITY]
>
>Mit einem Stern (![](assets/yellow-star.png)) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie vom Marketo Engage-Support.

**_Quartalsveröffentlichungen_**

Die folgenden Funktionen werden am (7 **Mai 2021)**.

## Account-basierte Erlebnisse {#Account-based-eaperiences}

* **Account Smart Lists (allgemeine Verfügbarkeit)** ![](assets/yellow-star.png): Dynamische Identifizierung und Qualifizierung von Accounts mit gewünschten Account- und Personenattributen, um sie in kanalübergreifenden Marketing-Kampagnen anzusprechen und zeitnahe Warnhinweise an den Vertrieb zu senden, um Angebote schneller abzuschließen. Diese neue Funktion ermöglicht eine robuste Automatisierung von Account-basierten Marketing-Strategien. Smart-Listen für Konten stehen Kunden mit Target-Kontoverwaltung zur Verfügung, die über das Benutzererlebnis der nächsten Generation verfügen.

## Benutzererlebnis der nächsten Generation {#next-generation-user-experience}

Mit der globalen Suchvorschau können Marketing-Experten schnell erkennen, wo ein freigegebenes Asset in ihrer Instanz vorhanden ist. Browser-Registerkarten zeigen den Speicherort an, um die Navigation in [!UICONTROL Marketing-Aktivitäten] oder [!UICONTROL Design Studio] zu verbessern. Zusätzliche Baumstruktur- und globale Suchfilter helfen, Ihre Suchkriterien zu verfeinern. Die Drag-and-Drop-Funktion innerhalb der Baumstruktur wurde wiederhergestellt, sodass Sie Ordner und Assets schnell und effizient in die Hauptbereiche der App verschieben können. Neu aktualisierte Symbole (die den Barrierefreiheitsstandards von Adobe entsprechen) und Statusabzeichen ermöglichen es Marketing-Experten, schnell und einfach in der Baumstruktur zwischen Ordnern und Assets zu unterscheiden und den Status von Programmen und Assets zu identifizieren.

## Experience Automation {#experience-automation}

* **Kampagnenflussschritte ausführen**: Optimieren Sie die Workflows zur Kampagnenerstellung und verbessern Sie die Kampagnenleistung mit einem neuen Flussschritt für intelligente Kampagnen. Erstellen und speichern Sie zentralisierte Vorlagenkampagnen für sich wiederholende Aufgaben in Ihrem Arbeitsbereich, z. B. die Normalisierung des Länder-Codes, die von jeder Smart-Kampagne über den neuen Flussschritt „Kampagne ausführen“ aufgerufen und ausgeführt werden. Verknüpfte Kampagnen werden in der festgelegten Reihenfolge ausgeführt und stellen die Erfüllung der Aufgabe sicher, bevor mit dem nächsten Flussschritt fortgefahren wird. Bearbeiten Sie den Fluss schnell in nur einer zentralen Kampagne, um jede Smart Campaign, die ihn verwendet, zu aktualisieren und so das Daten-Management, die Lead-Bewertung und die Routing-Workflows zu optimieren.

## Kanalübergreifende Orchestrierung {#cross-channel-orchestration}

* **Sensible Datenfelder in Forms**: Schützen Sie die personenbezogenen Daten (PII) des Kunden vor der Anzeige in Adobe Marketo Engage-Formularen, indem Sie Datenfelder als sensibel definieren und das Vorbefüllen der Formulare für diese Felder einschränken. Wenn ein Besucher ein Formular auf der Landingpage aufruft, werden in den als sensibel definierten Feldern keine vorausgefüllten Daten angezeigt.

* **Spam-Formularübermittlungen blockieren**: Schützen Sie Ihre Adobe Marketo Engage-Datenbank vor Junk-Daten, die zu ungültigen Warnhinweisen an den Vertrieb, Trigger-Kampagnenrückständen und unerwünschten Aktivitäten führen können. Der neue Validierungsmechanismus lehnt ungültige Formularübermittlungen ab und stoppt Bot-Angriffe. Ihre Daten sind sauberer, und Ihre Marketing-Kampagnen laufen wie beabsichtigt, wodurch das Risiko minimiert wird, unqualifizierte Leads an den Verkauf zu senden.

* **Warnhinweis zur Programmvalidierung per E-Mail senden**: Verhindern Sie das Senden fehlerhafter E-Mails, wenn die neuen Änderungen an einem zuvor genehmigten Programm vorgenommen wurden.  Die Warnung dient als Schutzmaßnahme, wenn ein Marketer Änderungen auf eine bereits genehmigte E-Mail anwendet, dann aber vergisst, die neuesten Änderungen zu genehmigen, und die E-Mail an eine große Audience ohne Inhalt, schlechten Inhalt oder alten Inhalt sendet.

* **E-Mail-Bot-Aktivität filtern**: Vermeiden Sie unbeabsichtigte Verkaufswarnungen und ungenaue E-Mail-Berichte durch die neue Filterfunktion für E-Mail-Bot-Aktivitäten. Identifizieren und filtern Sie Öffnungen und Klicks, die mit E-Mail-Bots verbunden sein können, die Links überprüfen, die zu falschen Triggern und Verkaufswarnungen oder falschen Berichten führen.

## API-Verbesserungen {#api-enhancements}

Mehrere wichtige Aktualisierungen der Bulk- und Lead-APIs, einschließlich der Möglichkeit, benutzerdefinierte Objektdaten stapelweise zu exportieren, Unternehmen mit Lead stapelweise zu verknüpfen, die Möglichkeit, Massenaktivitätsextraktion basierend auf einem primären Attribut zu filtern und die Programmmitgliedschaft zu erstellen und zu aktualisieren.

* **Ereignisprogramme verschachteln**: In Adobe Marketo Engage können Sie Ereignisprogramme unter anderen Programmtypen erstellen, klonen oder verschieben. Diese Funktion ist jetzt in der Assets-API zulässig.

* **Enhanced Delete Program API**: Ermöglicht integrierten Programmen das Löschen von Programmen, die zusätzliche Asset-Typen enthalten, ohne dass die Anwender dies manuell von Adobe Marketo Engage aus tun müssen.

* **Programmmitgliedschaft**: Marketing-Experten können anhand verschiedener Kriterien, wie z. B. des Status eines Programmmitglieds, alle Programmmitgliedsdatensätze nach einem ausgewählten Programm abfragen. Geben Sie diese Informationen für eine externe Anwendung, ein Business Intelligence-Tool oder Adobe Experience Cloud frei, um die Segmentierung zu verbessern und zielgerichtetere Interaktionen zu schaffen.

* **Massenextraktion benutzerdefinierter Objekte**: Der Massendatenexport ergänzt die Importfunktionen, die Datenanalysten bereits in Adobe Marketo Engage nutzen. Jetzt können sie massenweise Daten extrahieren, die im Adobe Marketo Engage Custom Objects der ersten Ebene gespeichert sind, diese Daten in ein anderes Programm, Data Warehouse oder BI-Tool (Business Intelligence) laden, um bessere Einblicke in die Daten in der Adobe Marketo Engage-Instanz zu erhalten.  Die Massendatenverschiebung von benutzerdefinierten Objekten ist bidirektional und kann zu einem geeigneten Zeitpunkt geplant werden.

* **Metadaten-API für benutzerdefinierte Felder**: Sparen Sie Zeit, indem Sie die Erstellung von benutzerdefinierten Feldern automatisieren, während Sie Ihre Adobe Marketo Engage-Integrationen mit einem Drittanbieterprogramm einrichten. Diese Automatisierung kommt insbesondere Kundinnen und Kunden mit mehreren Adobe Marketo Engage-Instanzen zugute, die jetzt in der Lage sind, die Erstellung benutzerdefinierter Felder zu optimieren, die früher in jeder Instanz manuell bearbeitet werden mussten. Optimieren Sie die Erstellung benutzerdefinierter Felder und sparen Sie Zeit bei dieser ressourcenintensiven Aktivität.

* **Bulk Activity Extract-API**: Erhalten Sie die Kontrolle über die Menge und den Typ der Daten bei der Durchführung von Massenextraktionen. Filtern Sie unnötige Datenpunkte heraus und steuern Sie die Anzahl der API-Aufrufe, die erforderlich sind, um Aktivitätsdaten stapelweise zu extrahieren.  Wählen Sie beispielsweise offene E-Mails, den Besuch einer Web-Seite oder eine Änderung der Lead-Bewertung aus und lassen Sie andere Wertänderungen zurück, die Sie nicht analysieren möchten. Optimieren Sie den Prozess, um die Anzahl der API-Aufrufe und die Datenbereinigung zu reduzieren.

* **Lead-API**: Identifizieren Sie Leads in Adobe Marketo Engage, denen eine Adobe-ECID (Experience Cloud-ID) zugeordnet ist.  Adobe Marketo Engage-Kunden können eine Liste von Leads aus einer ausgewählten Kampagne erstellen und die ECIDs (Experience Cloud-ID) verwenden, um in Adobe Analytics Berichte für diese bestimmte Liste zu erstellen. Die Integration zwischen Adobe Marketo Engage und Adobe Experience Cloud eröffnet unbegrenzte Möglichkeiten für Segmentierung, Targeting und Reporting.

* **API für den Massenimport von Leads**: Kontrollieren Sie den Massenimport von Leads und die dafür erforderlichen Ressourcen. Diese Verbesserung schafft eine Verbindung zwischen Lead und Unternehmen während des Massenimport-Prozesses des Leads. Erhöhen Sie die Effizienz und den Nutzen der Arbeit mit -Daten und verringern Sie die Nutzung von API-Aufrufen.

* **Web API-basierte Integration für die [!DNL Microsoft Dynamics Online] Kunden**: [!DNL MS Dynamics] Web API wurde mit Version 8.0 REST-Protokoll eingeführt und implementiert OData (Open Data Protocol) v4. OData ist ein OASIS-Standard (Organization for the Advancement of Structured Information Standards) zum Erstellen und Verwenden von RESTful-Services über umfangreiche Daten. Adobe Marketo Engage-Kunden, die mithilfe dieser Methode eine Integration mit [!DNL Microsoft Dynamics] benötigen, werden derzeit von SOAP (Simple Object Access Protocol) zu einer Web-API-basierten Verbindung migriert.

## Marketing-Datenumgebung {#marketing-data-environment}

* **XLSX-Export**: Wir haben die Exportfunktionen im gesamten Produkt aktualisiert, um XLSX anstelle von XLS zu unterstützen. Das bedeutet, dass diese Option an jeder Stelle im Produkt, an der der XLS-Export derzeit unterstützt wird, durch eine Option ersetzt wird, die stattdessen in XLSX exportiert wird. Diese Änderung wirkt sich auf die Dateinamen für alle Excel-Exporte von Berichten und anderen Daten aus Adobe Marketo Engage aus.

* **Suche nach Lead-ID**: Schneller Zugriff auf die Lead-Datensatzsuche anhand der Adobe Marketo Engage-Lead-ID in der Lead-Datenbank oder der statischen Liste. Geben Sie im Fenster Schnellsuche einfach `[id]` mit der entsprechenden Nummer ein. Daraufhin werden die Lead-Informationen angezeigt. Benutzer können Lead-, Unternehmens- oder Opportunity-Details schnell überprüfen.

## Bizible {#bizible}

![](assets/yellow-star.png)

* **Integration mit [!DNL LinkedIn] Lead Gen Forms (Beta)**: Mit der Premium-Attributionslösung von Bizible erhalten Sie einen tiefen Einblick in Ihre [!DNL LinkedIn] Kanalausgaben und den ROI. Durch die neueste Integration mit der Lead Gen-Forms von [!DNL LinkedIn] erhält Bizible insight in Formulare, die innerhalb der [!DNL LinkedIn]-Plattform eingereicht wurden. Diese ausgefüllten Formulare werden mit Leads aus Ihrer CRM- (Customer Relationship Management) oder Adobe Marketo Engage-Instanz abgeglichen, sodass sie für die Attribution in Frage kommen und anhand Ihrer anderen Marketing-Engagements verfolgt werden können.

## Ankündigungen {#announcements}

* **Wechselplattformen für Marketo-Produktdokumente**: Wir freuen uns, bekannt geben zu können, dass die Marketo-Produktdokumente ab Freitag, dem 7. Mai, in die Adobe Experience League aufgenommen wurden. Sie können weiterhin die URL docs.marketo.com verwenden. Wenn Sie bereits Artikel mit Lesezeichen versehen haben, werden Sie umgeleitet. Alle Produktdokumente sind auf der neuen Plattform verfügbar, mit Verbesserungen, die für später in diesem Jahr geplant sind.

* **Optimierte Benutzerverwaltung und Single Sign-on auf Basis des Adobe Identity Systems**: Ab Juli 2021 werden die neuen Adobe Marketo Engage-Kunden mit den Adobe-Benutzeranmeldeinformationen integriert. Die Migration von Bestandskunden zum integrierten Identitätssystem erfolgt erst Mitte 2022. Bis auf Weiteres ist keine Kundenaktion erforderlich. Mit Single Sign-on können IT-/Sicherheitsadministratoren mehrere Adobe Marketo Engage-Produktinstanzen zusammen mit anderen Experience Cloud-Lösungen verwalten und SSO (Shared Services Organization) über eine gemeinsame Konsole konfigurieren. Administratoren können über eine gemeinsame Admin Console Benutzergruppen und Benutzerberechtigungen bequem verwalten.

**_Webinar zur Produktversion_**

[Webinar zur Marketo Engage-Version Mai 2021](https://engage.marketo.com/May_21_Release_webinar_RegistrationPage.html)
