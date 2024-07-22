---
unique-page-id: 37355826
description: Versionshinweise - Februar 20 - Marketo-Dokumente - Produktdokumentation
title: Versionshinweise - Feb '20
exl-id: 6216b405-69c6-422b-a78c-7df0e8d271e9
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 1%

---

# Versionshinweise: Feb &#39;20 {#release-notes-feb}

Die folgenden Funktionen sind in der Version vom 20. Februar enthalten. Überprüfen Sie Ihre Marketo-Edition auf Funktionsverfügbarkeit.

>[!AVAILABILITY]
>
>Mit einem Stern ( ![(star)](assets/yellow-star.png)) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Wenden Sie sich an Ihren Marketo Engage-Support-Mitarbeiter, um mehr zu erfahren.

**_Vierteljährliche Versionen_** Die folgenden Funktionen wurden am 21. Februar 2020 veröffentlicht. ****

## Kern-Marketo-Einbindung {#core-marketo-engage}

* **Microsoft Dynamics &quot;Inhaber in Microsoft wechseln&quot;-Flussaktion**: Behalten Sie die Kontrolle über Ihre Microsoft Dynamics CRM-Daten bei, sodass Sie einen Lead-/Kontaktinhaber direkt über Marketo Engage ändern können. Dies ist eine Verbesserung unserer nativen CRM-Integrationsfunktion.
* **User Management-APIs**: Automatisieren Sie die Benutzer- und Rollenverwaltung durch externe Identitäts- und Organisationsverwaltungssysteme. Dies ist eine Verbesserung unserer API-Aufruffunktion.
* **Benutzerdefinierte Objekt-Schema-APIs**: Verwalten und stellen Sie benutzerdefinierte Objektschemata in allen Instanzen in Marketo Engage automatisch bereit, um Datenmodelle in Ihren Verkaufs- und Marketingtools konsistent zu halten. Mit dieser API können Sie benutzerdefinierte Objekte in einer Sandbox oder einem Kompetenzzentrum definieren und testen und so so viele Instanzen wie nötig bereitstellen. Dies ist eine Verbesserung unserer APIs-Aufruffunktion. Wenden Sie sich an Ihren Marketo Engage-Support-Mitarbeiter, um zu erfahren, wie Sie auf diese Verbesserung zugreifen können.
* **APIs für Umleitungsregeln für Landingpages**: Automatisches Management von Umleitungsregeln für Landingpages. Dies ist eine Verbesserung unserer API-Aufruffunktion.
* **Zwischenspeicherung des Formular-Deskriptors**: Wir reduzieren die Ladezeit eingebetteter Formulare und erhöhen die allgemeine Anwendungsstabilität durch Zwischenspeichern von Formularen als Ressourcen. Bitte beachten Sie, dass Genehmigungen, die an eingebetteten Formularen vorgenommen wurden, bis zu vier Minuten dauern können, bis sie im Internet angezeigt werden. Dies ist eine Verbesserung unserer Funktionen für Einstiegsseiten und Forms.

<br> 

**_Herausgabe während des gesamten Quartals_**

Die folgenden Funktionen befinden sich in einem nicht vierteljährlichen Zyklus und werden in den kommenden Monaten veröffentlicht.

## Bizible {#bizible}

![(star)](assets/yellow-star.png)

* **Kontobasierte Segmentierung**: Analysieren Sie die Attribution auf Kontoebene mit der Möglichkeit, Segmente und Filter für Discover-Pinnwände basierend auf Kontoattributen zu erstellen. Verwenden Sie diese Segmente, um einen Drilldown in Ihre kontobasierte Marketing-Performance durchzuführen.
* **Filter speichern**: Speichern Sie für jeden Benutzer spezifische Dashboard-Filter, um Ihre Dashboards schnell und konsistent zu analysieren.
* **Nach PDF exportieren**: Geben Sie wertvolle Einblicke in Ihr Unternehmen frei, indem Sie Bizible-Dashboards als PDF exportieren.

## Sales Connect {#sales-connect}

* **Window-Updates erstellen**: Wir haben den Prozess für die Auswahl von Vorlagen und den Versand von E-Mails über Sales Connect optimiert. Verwenden Sie das Fenster Erstellen in unserem Webclient und Salesforce als zentrale Anlaufstelle für Verkäufer, in der Sie Vorlagenkategorien speichern, E-Mails planen, in großen Mengen versenden und E-Mails mit Ansicht- und Klick-Tracking senden können.
* **Aktualisierungen des Command Centers**: Wir erstellen das Sales Connect-Befehlszentrum neu, um Verkäufern Einblicke in alle E-Mails, Aufrufe und Aufgaben zu ermöglichen, die über Sales Connect initiiert wurden. Sie können auch Informationen wie E-Mail-Interaktion und Zustellbarkeit über das Command Center anzeigen.

<br> 

## Ankündigungen {#announcements}

* **Marketo Engage Success Center**: Wir starten das Marketo Success Center im Februar 2020. Das Success Center ist ein produktinternes Hilfesystem, in dem Sie Produktdokumente und die Community durchsuchen, Anleitungen aufrufen, auf Adoptionsinhalte wie Marketo University und Best Practices-Videos von Kollegen zugreifen und vieles mehr - direkt von Ihrer Marketo Engage-Instanz aus. **Hinweis**: Diese Funktion wird als Beta-Version in ANZ gestartet und später im Quartal in Nordamerika eingeführt.

## Einstellungen {#deprecations}

* **Asset-API-Parameter &quot;_method&quot;**: Ab September 2020 akzeptieren Asset-API-Endpunkte &quot;_method&quot;nicht mehr, um Abfrageparameter in einem POST-Textkörper weiterzugeben, um URI-Längenbeschränkungen zu umgehen. Um Anforderungen aufzunehmen, die diesen Parameter erfordern, wird die URI-Beschränkung für Asset-APIs von 6 KiB auf 65 KiB erhöht, sodass lange Anfrage-URIs gesendet werden können.
* **Einstellung der Unterstützung für Internet Explorer**: Ab unserer Juli-Version vom 31. Juli 2020 wird die Marketo Engage-Benutzeroberfläche in Internet Explorer nicht mehr unterstützt.

**_Produkt-Release-Webinar_** [Nehmen Sie am 3. März um 11:00 Uhr PT/14:00 Uhr ET an, um ein Live-Webinar anzuzeigen, das von unserem Produktteam gehostet wird, und erfahren Sie mehr über die Funktionen in dieser Version.](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html)
