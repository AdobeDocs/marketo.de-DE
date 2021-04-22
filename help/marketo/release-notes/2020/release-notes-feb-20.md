---
unique-page-id: 37355826
description: Versionshinweise - Feb 20 - Marketo Docs - Produktdokumentation
title: Versionshinweise - Feb '20
exl-id: 6216b405-69c6-422b-a78c-7df0e8d271e9
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 1%

---

# Versionshinweise: Feb &#39;20 {#release-notes-feb}

Die folgenden Funktionen sind in der Version vom 20. Februar enthalten. Überprüfen Sie Ihre Marketo Edition auf Funktionsverfügbarkeit.

>[!AVAILABILITY]
>
>Mit einem Stern gekennzeichnete Funktionen ( ![(star)](assets/star-yellow.svg)) werden als kostenpflichtige Add-ons bezeichnet. Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zu erhalten.

**_Quartalsveröffentlichungen_** Die folgenden Funktionen wurden am 21.  **Februar 2020** veröffentlicht.

## Kern-Marketo-Einbindung {#core-marketo-engage}

* **Microsoft Dynamics &quot;Change Owner in Microsoft&quot; Flussaktion**: Behalten Sie die Kontrolle über Ihre Microsoft Dynamics CRM-Daten bei, sodass Sie einen Interessenten-/Kontaktbesitzer direkt von Marketo Engage aus ändern können. Dies ist eine Verbesserung unserer Native CRM-Integrationsfähigkeit.
* **User Management-APIs**: Automatisieren Sie die Benutzer- und Rollenverwaltung über externe Identitäts- und Organisationsverwaltungssysteme. Dies ist eine Verbesserung unserer API-Aufruffunktion.
* **Benutzerspezifische Objekt-Schema-APIs**: Automatisches Verwalten und Bereitstellen benutzerdefinierter Objekt-Schema über Instanzen in Marketo Engage hinweg, um Datenmodelle über Ihre Vertriebs- und Marketingwerkzeuge hinweg konsistent zu halten. Mit dieser API können Sie benutzerdefinierte Objekte in einer Sandbox oder einem Kompetenzzentrum definieren und testen und so viele Instanzen wie nötig bereitstellen. Dies ist eine Verbesserung unserer APIs-Aufruffunktion. Wenden Sie sich an Ihren Kundenbetreuer, um zu erfahren, wie Sie auf diese Verbesserung zugreifen können.
* **APIs** für Umleitungsregeln für Landingpages: Automatisieren Sie die Verwaltung von Umleitungsregeln für Landingpages. Dies ist eine Verbesserung unserer API-Aufruffunktion.
* **Zwischenspeicherung** des Formulardeskriptors: Wir reduzieren die Ladezeit von eingebetteten Formularen und erhöhen die allgemeine Anwendungsstabilität durch Zwischenspeichern von Formularen als Ressourcen. Bitte beachten Sie, dass die Genehmigung von eingebetteten Formularen bis zu vier Minuten dauern kann, bis sie im Internet nachgedacht ist. Dies ist eine Verbesserung unserer Landingpages- und Forms-Fähigkeiten.

<br> 

**_Veröffentlichung im gesamten Quartal_**

Die folgenden Funktionen befinden sich in einem nicht vierteljährlichen Zyklus und werden in den kommenden Monaten veröffentlicht.

## Bizible {#bizible}

![(Stern)](assets/star-yellow.svg)

* **Kontobasierte Segmentierung**: Analysieren Sie die Zuordnung auf Kontoebene mit der Möglichkeit, Segmente und Filter für Discover-Pinnwände basierend auf Kontoattributen zu erstellen. Verwenden Sie diese Segmente, um einen Drilldown in Ihrer kontobasierten Marketingleistung durchzuführen.
* **Speichern von Filtern**: Speichern Sie benutzerspezifische Filter, um Ihre Dashboard schnell und konsistent zu analysieren.
* **In PDF** exportieren: Geben Sie wertvolle Einblicke in Ihr Unternehmen, indem Sie Bizible-Dashboards als PDF-Dateien exportieren.

## SalesConnect {#sales-connect}

* **Erstellen Sie Fensteraktualisierungen**: Wir haben den Prozess zur Auswahl von Vorlagen und zum Senden von E-Mails über Sales Connect optimiert. Verwenden Sie das Fenster Erstellen in unserem Webclient und Salesforce als eine zentrale Anlaufstelle für Verkäufer, mit der Sie Vorlagendaten speichern, E-Mails planen, E-Mails stapelweise versenden und E-Mails mit Ansicht und Klick-Tracking versenden können.
* **Aktualisierungen** im Command Center: Wir bauen das Sales Connect Command Center wieder auf, um Verkäufern einen Einblick in all ihre E-Mails, Anrufe und Aufgaben zu geben, die von Sales Connect initiiert wurden. Sie können auch Informationen wie E-Mail-Interaktion und Zustellbarkeit über das Command Center Ansicht haben.

<br> 

## Ankündigungen {#announcements}

* **Erfolgszentrum** des Marketo Engages: Wir starten das Marketo Erfolgszentrum im Februar 2020. Das Success Center ist ein produktinternes Hilfecenter, mit dem Sie Produktdokumente und die Community durchsuchen, Anleitungen starten, auf Adoptionsinhalte wie die Marketo University und Videos zu Best Practices zugreifen und vieles mehr - direkt von Ihrer Marketo Engage-Instanz aus. **Hinweis**: Diese Funktion wird als Betaversion in ANZ eingeführt und wird später in Nordamerika eingeführt.

## Veraltungen {#deprecations}

* **Parameter** der Asset-API &quot;_method&quot;: Ab September 2020 akzeptieren Asset-API-Endpunkte &quot;_method&quot;nicht mehr, um Abfragen-Parameter in einem POST-Textkörper zu übergeben, um die Längenbeschränkungen des URI zu umgehen. Um Anforderungen, die diesen Parameter erfordern, anzupassen, wird die URI-Beschränkung für Asset-APIs von 6 KiB auf 65 KiB erhöht, sodass lange Anforderungs-URIs gesendet werden können.
* **Einstellung** der Unterstützung für Internet Explorer: Ab unserer Version vom 31. Juli 2020 wird die Marketo Engage-Benutzeroberfläche in Internet Explorer nicht mehr unterstützt.

**_Produktversion_** [WebinarNehmen Sie ](https://engage.marketo.com/Jan_Feb_20_Release_Webinar_Registration.html) am 3. März um 11:00 Uhr PT/2:00 Uhr ET an einem Live-Webinar teil, das von unserem Produktteam gehostet wird, und erfahren Sie mehr über die Funktionen in dieser Version.
