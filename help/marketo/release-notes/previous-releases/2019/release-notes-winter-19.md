---
unique-page-id: 17727823
description: Versionshinweise - Winter 19 - Marketo Docs - Produktdokumentation
title: Versionshinweise - Winter '19
exl-id: 0cb3b3a1-472e-41d4-84f4-47f06e65017c
feature: Release Information
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '1079'
ht-degree: 3%

---

# Versionshinweise: Winter &#39;19 {#release-notes-winter}

Die folgenden Funktionen sind in der Version Winter 19 enthalten. Überprüfen Sie Ihre Marketo-Edition auf Funktionsverfügbarkeit.

Klicken Sie auf die Titel-Links, um detaillierte Artikel zu den einzelnen Funktionen anzuzeigen, sofern verfügbar.

>[!NOTE]
>
>Facebook benötigt jetzt ein Business Manager-Konto, um Ihre benutzerdefinierte Zielgruppenintegration nutzen zu können. Ihr Facebook LaunchPoint-Dienst *must* mit einem Business Manager-Konto verknüpft sein oder **Ihre Integration funktioniert nach dem 14. Januar 2019 nicht mehr**. Informationen zum Einrichten eines Business Manager-Kontos finden Sie unter [Hilfe zu facebook](https://www.facebook.com/business/help/1710077379203657).

>[!NOTE]
>
>Microsoft drängt alle Online-Kunden zum Upgrade auf die neueste Version von Microsoft Dynamics. Wenn Sie Ihre Marketo-Instanz mit Dynamics Online integrieren, müssen Sie [Aktualisierung auf die neueste Version der Marketo-Lösung](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md) before **31. Januar 2019** , um sicherzustellen, dass Ihre Integration weiterhin funktioniert.

>[!NOTE]
>
>Marketo aktualisiert die OAuth-Version für GoToWebinar von 1.0 auf 2.0. Die Unterstützung für OAuth 1.0 wird im Januar 2019 eingestellt. Wenn Sie GoToWebinar-Kunde sind, müssen Sie Ihre Anmeldungen über LaunchPoint (im Admin-Bereich) durch **31. Januar 2019** , um sicherzustellen, dass Ihre Integration weiterhin funktioniert. Weitere Informationen finden Sie in unserer [Community-Seite](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019).

## Verbesserungen der Kernplattform {#core-platform-enhancements}

**[E-Mails in E-Mails an Email CC für Marketo](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

Fügen Sie E-Mails, die über Marketo gesendet werden, bis zu fünf CC-Adressen pro Empfänger hinzu.

**API**

* **Unterstützung für mehrere Branding-Domänen für die Asset-API:** Das Genehmigen und Klonen von Assets führt innerhalb der API und Benutzeroberfläche zu denselben Ergebnissen.
* **E-Mail-CC-Unterstützung für Asset-API**: Benutzer, die E-Mails über die API klonen, genehmigen und verarbeiten, stimmen mit den Benutzeroberflächeneinstellungen überein.

**[Munchkin v155 (Beta)](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/lead-tracking)**

* **Nur-API-Modus**: Benutzer können jetzt bestimmen, wann und wie Mitglieder ihrer Datenbank verfolgt werden, indem sie zulassen, dass einseitige Webanwendungen explizit aufrufen, wenn sie einen Webseitenbesuch aufzeichnen möchten, anstatt sich auf die automatische Verfolgung von Marketo zu verlassen.
* **Opt-out-Verwaltung**: Einfaches Verwalten von Opt-outs durch Abgleichen der Opt-out-Cookie-Domäne mit der Munchkin-Tracking-Cookie-Domäne.
* **Entscheidungsparameter auf Domänenebene**: Domänen mit zwei Buchstaben (d. h. &quot; [website.io](https://website.io)&quot;) wird automatisch in Marketo ohne zusätzliche Einrichtungsanforderungen verfolgt.

## Marketo Sales Engage {#marketo-sales-engage}

* **Salesforce Custom Profile**: Sales Engage unterstützt jetzt unbegrenzte benutzerdefinierte Profile.

* **Salesforce-Anpassung**: Durch das Entfernen nicht kritischer benutzerdefinierter Aktivitätsfelder können Benutzer die Kundenbindung in der CRM-Plattform effizienter einrichten.
* **Email Service**: Nutzen Sie eine bessere Zustellbarkeit sowie verbesserte Antwort-Tracking, geplante E-Mail-Funktionen und Massen-E-Mail-Funktionen, indem Sie eine Verbindung zu Microsoft Outlook herstellen (entweder über Office365 oder On-Premise über die Registerkarte E-Mail-Verbindung ).
* **Neue Admin Settings**: Es wurden zwei Admin-Seiten hinzugefügt, um Ihre Sales Engage-Instanz zu optimieren.

   * _Team-Management_ unterstützt eine nahtlose Kontoeinrichtung, indem sie es Administratoren ermöglicht, Abonnements und Teams zu bearbeiten.
   * _Salesforce-Admin-Einstellungen_ hilft Teams, ihre SFDC-Synchronisation schneller und einfacher einzurichten als je zuvor.

* **OWA-Plug-in für Windows**: Mit einem einzigen Add-in werden alle Windows Office365-Clients in Sales Engage unterstützt, sodass Live Feed in Outlook verwendet werden kann. Das neue Plug-in wird im Microsoft Store verfügbar sein.
* **Activities Pusher**: Synchronisieren Sie die Vertriebsinteraktion mit der Marketo-Hauptplattform, um Echtzeit-Marketing-Einblicke zu nutzen.

## Marketo Sky {#marketo-sky}

>[!NOTE]
>
>Marketo Sky-Releases treten häufiger auf. Die folgenden Funktionen und Verbesserungen werden voraussichtlich Ende Q4/Anfang Q1 veröffentlicht. Weitere Informationen und Aktualisierungen finden Sie in der [Sky-Dokumentation](https://help.marketo.com/).

* **Optionales Standarderlebnis**: Marketo-Benutzer können Marketo Sky als Standarderlebnis festlegen, wenn ihnen Zugriff durch einen Administrator gewährt wurde.

* **Meine Marketo neu gestaltet**: Passen Sie Ihr Erlebnis an, indem Sie Widgets hinzufügen, die wichtige Informationen, Benachrichtigungen und Links zu den am häufigsten besuchten Bereichen enthalten.

* **Design Studio-Listenansichten und Detailseiten**: Mit filterbaren und durchsuchbaren Listenansichten von E-Mails, Landingpages und Formularen profitieren Sie von einer höheren Organisation und Genauigkeit. Asset-Detailseiten bieten wichtige Informationen zu jedem Asset, einschließlich der Programme, von denen das Asset verwendet wird, der Anzahl der verwendeten Snippets und mehr.

* **Globale Suche**: Marketo bietet jetzt eine schnellere und robustere globale Suchfunktion auf der gesamten Plattform. Suchabfragen werden jetzt in allen zugänglichen Arbeitsbereichen ausgeführt und können nach Assets (sowohl aktiv als auch archiviert), Bezeichnungen, Kampagnen und Programmen suchen. Suchergebnisse werden über eine Überlagerung bereitgestellt. Jedes Ergebnis enthält seinen Dateispeicherort-Pfad, um anzugeben, wo sich das Asset befindet.

* **Verbesserte Benutzeroberfläche**: Neue Symbole, Modelle und Schaltflächen sowie eine neue Farbpalette, die unsere Markenaktualisierung widerspiegelt und Marketo Sky noch beeindruckender und funktioneller macht.

* **Verbesserungen bei der Benutzerfreundlichkeit von E-Mail-Programmen**: Wir gehen weiter auf die Parität der E-Mail-Programmfunktionalität zwischen unserer klassischen Marketo-Lead-Management-Plattform und dem neuen Marketo Sky-Erlebnis zu.
* **Event-with-Webinar-Programme**: Event-With-Webinar-Programme sind jetzt unter Marketo Sky verfügbar (Hinweis: In dieser Version wird nur GoToWebinar unterstützt, wobei im Laufe der Zeit weitere Integrationen erstellt werden).

## Kundenbezogenes Marketing {#account-based-marketing}

**[ABM Persona-basierte Segmentierung und Filterung](/help/marketo/product-docs/target-account-management/using-personas.md)**

Personalisieren Sie Ihre ABM-Kampagnen für bestimmte Personas in benannten Konten. Die ABM Persona-Funktion erstellt einen standardmäßigen Auftragstitel basierend auf der Lead-Segmentierung und ermöglicht die Konfiguration zusätzlicher Personensegmentierungen.

## Analytics {#analytics}

**Bizible**

* **Benutzerdefinierte berechnete Felder**: Verwenden Sie ein beliebiges Bizible-Attribut, um benutzerdefinierte Felder zu erstellen, die für Dashboard-Berichte und -Segmentierung verwendet werden können.

* **Zertifizierung nach SOC II Typ II**: Die neue Sicherheits- und Datenschutzzertifizierung baut auf der Typakkreditierung I von Anfang dieses Jahres auf.

## Web-Personalisierung {#web-personalization}

**[In den Kontoeinstellungen Subdomänen hinzufügen](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

Um Domänen und Subdomänen effizienter zu verwalten, können Benutzer nun Subdomänen zu ihren RTP-Kontoeinstellungen hinzufügen.

## Marketo Mobile Engagement (MME) {#marketo-mobile-engagement-mme}

**Aktualisiertes MME Software Development Kit (SDK) für Android**

Wir haben unser SDK für Android auf ein moderneres, stabileres und skalierbareres Framework aktualisiert, das mehr Flexibilität und neue technische Funktionen enthält. Entwickler von Android-Apps können jetzt Google direkt verwenden [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/) (FCM) mit diesem neuen SDK.

* [Entwicklerhandbücher]https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/mobile/installation#how-to-install-marketo-sdk-on-android)

>[!NOTE]
>
>App-Entwickler **must** Aktualisierung auf die neue Version vor dem 31. März 2019. Wenn Sie Ihr SDK nicht bis zum 31. März 2019 aktualisieren, können neue Benutzer, die Ihre App nach diesem Datum herunterladen, erst Push-Benachrichtigungen erhalten, wenn Sie auf die neueste Version des SDK aktualisieren. Für das SDK-Update ist es nicht erforderlich, dass Ihre aktuellen Benutzer Ihrer mobilen App eine neue Version Ihrer App erneut herunterladen.

## Weitere Updates {#additional-updates}

**Erweiterte Webinar-Plattform**

Zusätzlich zur Produktversion arbeitet unser Partnerteam an einem neuen Framework, das Webinar-Anbietern die Erstellung und Pflege eigener Integrationen mit Marketo ermöglicht. So erhalten sie mehr Flexibilität bei der Aktualisierung und Optimierung ihrer Lösungen und können Marketingexperten ihre ausgewählten Integrationen optimal nutzen.

Wir planen, unsere neue Plattform mit Anbietern von Fall zu Fall zu erweitern. Weitere Informationen finden Sie in unserer [Programmdetails](https://www.marketo.com/why-marketo/partners/technology/) oder wenden Sie sich an Ihren Ansprechpartner bei Marketo.
