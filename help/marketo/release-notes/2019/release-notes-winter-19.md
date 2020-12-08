---
unique-page-id: 17727823
description: Versionshinweise - Winter 19 - Marketing Docs - Produktdokumentation
title: Versionshinweise - Winter 19
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '1112'
ht-degree: 0%

---


# Versionshinweise: Winter &#39;19 {#release-notes-winter}

Die folgenden Funktionen sind in der Version Winter &#39;19 enthalten. Überprüfen Sie Ihre Marketo-Edition auf Funktionsverfügbarkeit.

Bitte klicken Sie auf die Titellink-Links, um detaillierte Ansichten zu den einzelnen Funktionen anzuzeigen, falls verfügbar.

>[!NOTE]
>
>Für Facebook ist jetzt ein Business Manager-Konto erforderlich, um die Integration Ihrer benutzerspezifischen Audience nutzen zu können. Ihr Facebook LaunchPoint-Dienst *muss* mit einem Business Manager-Konto verknüpft sein, sonst funktioniert **Ihre Integration nach dem 14. Januar 2019** nicht mehr. Informationen zum Einrichten eines Business Manager-Kontos finden Sie in der [Facebook-Hilfe](https://www.facebook.com/business/help/1710077379203657).

>[!NOTE]
>
>Microsoft drängt alle Online-Kunden, auf die neueste Version von Microsoft Dynamics zu aktualisieren. Wenn Sie Ihre Marketo-Instanz mit Dynamics Online integrieren, müssen Sie vor dem 31. [Januar 2019](../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution/upgrade-the-marketo-solution-for-microsoft-dynamics.md) auf die neueste Version der Marketing Solution **** aktualisieren, um sicherzustellen, dass Ihre Integration weiterhin funktioniert.

>[!NOTE]
>
>Marketo aktualisiert die OAuth Version für GoToWebinar von 1.0 auf 2.0. Die Unterstützung für OAuth 1.0 wird im Januar 2019 eingestellt. Wenn Sie GoToWebinar-Kunde sind, müssen Sie Ihre Anmeldungen bis zum 31. **Januar 2019** über LaunchPoint (im Admin-Bereich) erneut authentifizieren, um sicherzustellen, dass Ihre Integration weiterhin funktioniert. Weitere Informationen finden Sie auf unserer [Community-Seite](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019).

## Verbesserungen der Hauptplattform {#core-platform-enhancements}

** [E-Mail-Adresse für Marketing-E-Mails](../../product-docs/email-marketing/general/email-cc.md)**

Binden Sie bis zu fünf CC-Adressen pro Empfänger in E-Mails ein, die über Marketing gesendet werden.

**API**

* **Unterstützung für mehrere Branding-Domänen für die Asset-API:** Das Genehmigen und Klonen von Assets führt innerhalb der API und Benutzeroberfläche zu denselben Ergebnissen.
* **E-Mail-CC-Unterstützung für Asset-API**: Benutzer, die E-Mails über die API klonen, genehmigen und verarbeiten, bleiben mit den Benutzeroberflächeneinstellungen identisch.

** [Munchkin v155 (Beta)](http://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **Nur-API-Modus**: Benutzer können nun festlegen, wann und wie Mitglieder ihrer Datenbank verfolgt werden, indem sie einseitige Web-Apps explizit aufrufen können, wenn sie einen Webseitenbesuch aufzeichnen möchten, anstatt sich auf die automatische Verfolgung von Marketo zu verlassen.
* **Abmeldeverwaltung**: Sie können die Ausschluss-Cookie-Domäne problemlos verwalten, indem Sie die Ausschluss-Cookie-Domäne mit der Munchkin-Tracking-Cookie-Domäne abgleichen.
* **Domänendef-Parameter**: Zweibuchstaben-Domänen (d. h. &quot; [website.io](http://website.io)&quot;) wird in Marketo automatisch verfolgt, ohne dass zusätzliche Setup-Anforderungen erforderlich sind.

## Marketo Sales Engage {#marketo-sales-engage}

* **Salesforce-benutzerdefiniertes Profil**: Sales Engage unterstützt jetzt unbegrenzte benutzerspezifische Profil.

* **Salesforce-Anpassung**: Indem Sie nicht kritische Felder für die benutzerdefinierte Aktivität entfernen, können Sie Sales Engage effizienter in der CRM-Plattform einrichten.
* **E-Mail-Dienst**: Profitieren Sie von einer besseren Auslieferbarkeit und verbesserten Funktionen für die Rückverfolgung von Antworten, geplante E-Mails und Massen-E-Mails, indem Sie eine Verbindung zu Microsoft Outlook herstellen (über die Registerkarte &quot;E-Mail-Verbindung&quot;über Office 365 oder On-Prem).
* **Neue Admin-Einstellungen**: Zur Optimierung Ihrer Sales Engage-Instanz wurden zwei Admin-Seiten hinzugefügt:

   * *Team Management* unterstützt einen nahtlosen Kontoeinrichtungsprozess, indem Administratoren Abonnements und Teams bearbeiten können.
   * *Salesforce Admin Settings* hilft Teams, ihre SFDC-Synchronisierung schneller und einfacher einzurichten als je zuvor.

* **OWA-Plugin für Windows**: Mit einem einzigen Add-In werden alle Windows Office365-Clients in Sales Engage unterstützt, sodass Live Feed in Outlook verwendet werden kann. Das neue Plugin wird im Microsoft Store verfügbar sein.
* **Aktivitäten Pusher**: Synchronisieren Sie Sales Engage mit der zentralen Marketo-Plattform, um Echtzeit-Marketing-Erkenntnisse zu nutzen.

## Marketo Sky {#marketo-sky}

>[!NOTE]
>
>Marketo Sky-Releases treten häufiger auf. Die folgenden Funktionen und Erweiterungen werden voraussichtlich Ende des 4. Quartals/Anfang des 1. Weitere Informationen und Aktualisierungen finden Sie in unserer [Sky-Dokumentation](https://help.marketo.com/hc/en-us/articles/360012858573).

* **Optionales Standarderlebnis**: Marketo-Benutzer können Marketo Sky als Standarderlebnis festlegen, wenn ihnen der Zugriff durch einen Administrator gewährt wurde.

* **Mein Marketer** wurde neu gestaltet: Passen Sie Ihr Erlebnis an, indem Sie Widgets hinzufügen, die wichtige Informationen, Benachrichtigungen und Links zu den am häufigsten besuchten Bereichen enthalten.

* **Ansichten und Detailseiten für die Design Studio-Liste**: Mit den Ansichten von E-Mails, Landingpages und Formularen, die Sie filtern und durchsuchen können, erzielen Sie eine höhere Organisations- und Genauigkeitsstufe. Asset-Detailseiten enthalten wichtige Informationen zu den einzelnen Assets, einschließlich der Programm, die das Asset verwendet, der Anzahl der verwendeten Snippets und mehr.

* **Globale Suche**: Marketo Angebot jetzt eine schnellere und robustere globale Suchfunktion. Die Abfragen der Suche werden jetzt auf allen verfügbaren Arbeitsbereichen ausgeführt und können Assets (aktiv und archiviert), Beschriftungen, Kampagnen und Programm suchen. Die Suchergebnisse werden über eine Überlagerung bereitgestellt. Jedes Ergebnis enthält den Dateispeicherort-Pfad, um anzugeben, wo sich das Asset befindet.

* **Verbesserte Benutzeroberfläche**: Neue Symbole, Modale und Schaltflächen sowie eine neue Farbpalette, die unsere Markenaktualisierung widerspiegelt und die Marketo Sky noch beeindruckender und funktioneller macht.

* **Verbesserungen** der Benutzerfreundlichkeit von E-Mail-Programmen: Wir gehen weiter in Richtung Parität bei der E-Mail-Programm-Funktionalität zwischen unserer klassischen Marketing-Lead-Management-Plattform und dem neuen Marketo Sky-Erlebnis.
* **Ereignis-mit-Webinar-Programme**: Ereignis-mit-Webinar-Programme sind jetzt auf Marketo Sky verfügbar (Hinweis: Nur GoToWebinar wird in dieser Version unterstützt, mit weiteren Integrationen im Laufe der Zeit).

## Kundenbasiertes Marketing {#account-based-marketing}

** [ABM Personale Segmentierung und Filterung](../../product-docs/account-based-marketing/using-personas.md)**

Personalisieren Sie Ihre ABM-Kampagnen für bestimmte Personen in benannten Konten. Die ABM-Persona-Funktion erstellt einen Standardauftragstitel basierend auf der Interessentensegmentierung und ermöglicht die Konfiguration zusätzlicher Personensegmente.

## Analytics {#analytics}

**Bizibel**

* **Benutzerdefinierte berechnete Felder**: Verwenden Sie ein beliebiges Bizible-Attribut, um benutzerdefinierte Felder zu erstellen, die für den Berichte und die Segmentierung von Dashboards verwendet werden können.

* **SOC-II-Zertifizierung**: Die neue Sicherheits- und Datenschutzzertifizierung baut auf der Typzulassung von Anfang des Jahres auf.

## Web-Personalisierung {#web-personalization}

**[hinzufügen Subdomänen in den Kontoeinstellungen](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

Zur effizienteren Verwaltung von Domänen und Subdomänen können Benutzer nun Subdomänen zu ihren RTP-Kontoeinstellungen hinzufügen.

## Marketing-Mobile-Interaktion (MME) {#marketo-mobile-engagement-mme}

**Aktualisiertes MME Software Development Kit (SDK) für Android**

Wir haben unser SDK für Android auf ein moderneres, stabileres und skalierbares Framework aktualisiert, das mehr Flexibilität und neue technische Funktionen enthält. Entwickler von Android-Apps können jetzt mit diesem neuen SDK direkt die [Firebase Cloud Messaging](http://firebase.google.com/docs/cloud-messaging/) (FCM) von Google verwenden.

* [Entwicklerhandbücher](http://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [Häufig gestellte Fragen zu Entwicklern](http://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>App-Entwickler **müssen** vor dem 31. März 2019 auf die neue Version aktualisieren. Wenn Sie Ihr SDK nicht bis zum 31. März 2019 aktualisieren, können neue Benutzer, die Ihre App nach diesem Datum herunterladen, erst Push-Benachrichtigungen erhalten, wenn Sie auf die neueste Version des SDK aktualisieren. Für das SDK-Update ist es nicht erforderlich, dass Ihre aktuellen Benutzer der mobilen App eine neue Version Ihrer App erneut herunterladen.

## Zusätzliche Aktualisierungen {#additional-updates}

**Erweiterte Webinar-Plattform**

Neben der Produktversion arbeitet unser Partnerteam an einem neuen Framework, das Webinar-Anbietern die Möglichkeit gibt, eigene Integrationen mit Marketo zu entwickeln und zu pflegen. Dadurch erhalten sie mehr Flexibilität bei der Aktualisierung und Verbesserung ihrer Lösungen und können Marketingexperten die von ihnen gewählten Integrationen optimal nutzen.

Wir planen, unsere neue Plattform mit Anbietern von Fall zu Fall zu entwickeln. Weitere Informationen finden Sie in unseren [Programm-Details](https://www.marketo.com/why-marketo/partners/technology/) oder wenden Sie sich an Ihren Ansprechpartner bei Marketing.
