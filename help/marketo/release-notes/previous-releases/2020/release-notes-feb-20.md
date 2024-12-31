---
unique-page-id: 37355826
description: Versionshinweise - Februar '20 - Marketo-Dokumente - Produktdokumentation
title: Versionshinweise - Feb '20
exl-id: 6216b405-69c6-422b-a78c-7df0e8d271e9
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 1%

---

# Versionshinweise: Feb &#39;20 {#release-notes-feb}

Die folgenden Funktionen sind in der Version vom Februar 2020 enthalten. Überprüfen Sie Ihre Marketo Edition auf die Verfügbarkeit der Funktionen.

>[!AVAILABILITY]
>
>Mit einem Stern ( ![(Stern)](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie von Ihrem Marketo Engage-Support-Mitarbeiter.

**_Vierteljährliche Versionen_** Die folgenden Funktionen wurden am **21. Februar 2020)**.

## Kern-Marketo-Einbindung {#core-marketo-engage}

* **Flussaktion „Inhaber in Microsoft ändern“ in Microsoft Dynamics**: Behalten Sie die Kontrolle über Ihre Microsoft Dynamics CRM-Daten bei und können Sie den Inhaber eines Leads/Kontakts direkt vom Marketo Engage aus ändern. Dies ist eine Erweiterung unserer nativen CRM-Integrationsfunktion.
* **User Management-APIs**: Automatisieren Sie die Benutzer- und Rollenverwaltung über externe Identitäts- und Organisationsverwaltungssysteme. Dies ist eine Erweiterung unserer API-Aufruffunktion.
* **APIs für benutzerdefinierte Objektschemata**: Automatisches Verwalten und Bereitstellen von benutzerdefinierten Objektschemata über Instanzen hinweg in Marketo Engage, um Datenmodelle in Ihren Verkaufs- und Marketing-Tools konsistent zu halten. Mit dieser API können Sie benutzerdefinierte Objekte in einer Sandbox oder einem Kompetenzzentrum definieren und testen und für beliebig viele Instanzen bereitstellen. Dies ist eine Erweiterung unserer API-Aufruffunktion. Wenden Sie sich an Ihren Marketo Engage-Support-Mitarbeiter, um zu erfahren, wie Sie Zugriff auf diese Verbesserung erhalten.
* **APIs für Landingpage-Umleitungsregeln**: Automatisieren Sie die Verwaltung von Umleitungsregeln für Landingpages. Dies ist eine Erweiterung unserer API-Aufruffunktion.
* **Zwischenspeichern von Formulardeskriptoren**: Durch Zwischenspeichern von Formularen als Ressourcen reduzieren wir die Ladezeit von eingebetteten Formularen und verbessern die allgemeine Anwendungsstabilität. Bitte beachten Sie, dass es bei Genehmigungen von eingebetteten Formularen bis zu vier Minuten dauern kann, bis sie im Internet widergespiegelt werden. Dies ist eine Erweiterung unserer Funktionen für Landingpages und Forms.

<br> 

**_Veröffentlichung im gesamten Quartal_**

Die folgenden Funktionen befinden sich in einem nicht vierteljährlichen Zyklus und werden in den kommenden Monaten veröffentlicht.

## Bizible {#bizible}

![(Stern)](assets/yellow-star.png)

* **Account-basierte Segmentierung** Analysieren Sie die Attribution auf Kontoebene mit der Möglichkeit, Segmente und Filter für Discover-Dashboards auf der Grundlage von Kontoattributen zu erstellen. Verwenden Sie diese Segmente, um eine Aufschlüsselung nach Ihrer Account-basierten Marketing-Leistung durchzuführen.
* **Filter speichern**: Speichern Sie Dashboard-spezifische Filter, die für jeden Benutzer eindeutig sind, um Ihre Dashboards schnell und konsistent zu analysieren.
* **Auf PDF exportieren**: Teilen Sie wertvolle Erkenntnisse in Ihrem Unternehmen, indem Sie Bizible Dashboards als PDF exportieren.

## Sales Connect {#sales-connect}

* **Fenster-Updates erstellen**: Der Prozess zur Auswahl von Vorlagen und zum Versand von E-Mails über Sales Connect wurde optimiert. Verwenden Sie das Fenster Erstellen in unserem Webclient und Salesforce als zentrale Anlaufstelle für Verkäufer, mit der Möglichkeit, Vorlagenkategorien zu speichern, E-Mails zu planen, E-Mails massenweise zu senden und E-Mails mit Ansicht- und Klick-Tracking zu senden.
* **Aktualisierungen des Command Centers**: Wir bauen das Sales Connect Command Center neu auf, um Verkäufern Einblicke in all ihre E-Mails, Anrufe und Aufgaben zu geben, die von Sales Connect initiiert wurden. Sie können auch Informationen wie E-Mail-Interaktion und Zustellbarkeit über das Command Center anzeigen.

<br> 

## Ankündigungen {#announcements}

* **Marketo Engage Success Center**: Im Februar 2020 starten wir das Marketo Success Center. Das Success Center ist ein produktinternes Hilfesystem, mit dem Sie Produktdokumente und die Community durchsuchen, Anleitungen aufrufen, auf Annahmeinhalte wie die Marketo University und Best Practice-Videos von Kollegen zugreifen und vieles mehr - direkt von Ihrer Marketo Engage-Instanz aus. **Hinweis**: Diese Funktion wird als Beta-Version in ANZ gestartet und später in diesem Quartal in Nordamerika eingeführt.

## Einstellungen {#deprecations}

* **Asset-API „_method“-**: Nach September 2020 akzeptieren Asset-API-Endpunkte keine „_method“ mehr zum Übergeben von Abfrageparametern in einem POST-Hauptteil, um URI-Längenbeschränkungen zu umgehen. Um Anfragen zu berücksichtigen, die diesen Parameter erfordern, wird die URI-Beschränkung für Asset-APIs von 6 KB auf 65 KB erhöht, sodass lange Anfrage-URIs gesendet werden können.
* **Einstellung der Unterstützung für Internet Explorer**: Ab unserer Version vom 31. Juli 2020 wird die Marketo Engage-Benutzeroberfläche in Internet Explorer nicht mehr unterstützt.

**_Webinar zur Produktversion_** [Nehmen Sie ](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) 3. März um 11:00 Uhr PT/14:00 Uhr ET an einem Live-Webinar teil, das von unserem Produktteam gehostet wird, und erfahren Sie mehr über die in dieser Version enthaltenen Funktionen.
