---
unique-page-id: 17727823
description: Versionshinweise - Winter '19 - Marketo-Dokumentation - Produktdokumentation
title: Versionshinweise - Winter '19
exl-id: 0cb3b3a1-472e-41d4-84f4-47f06e65017c
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '1050'
ht-degree: 3%

---

# Versionshinweise – Winter 2019 {#release-notes-winter}

Die folgenden Funktionen sind in der Version Winter &#39;19 enthalten. Überprüfen Sie Ihre Marketo Edition auf die Verfügbarkeit der Funktionen.

Bitte klicken Sie auf die Titel-Links, um detaillierte Artikel für jede Funktion anzuzeigen, falls verfügbar.

>[!NOTE]
>
>[!DNL Facebook] benötigt jetzt ein Business Manager-Konto, um Ihre benutzerdefinierte Audience-Integration nutzen zu können. Ihr [!DNL Facebook] LaunchPoint *Service muss* einem Business Manager-Konto zugeordnet sein oder **Ihre Integration funktioniert nach dem 14. Januar 2019 nicht mehr**. Informationen zum Einrichten eines Business Manager-Kontos finden Sie unter [[!DNL Facebook] Hilfe](https://www.facebook.com/business/help/1710077379203657).

>[!NOTE]
>
>Microsoft drängt alle Online-Kunden, auf die neueste Version von [!DNL Microsoft Dynamics] zu aktualisieren. Wenn Sie Ihre Marketo-Instanz mit [!DNL Dynamics Online] integrieren, müssen Sie vor dem 31. [&#x200B; 2019 ein Upgrade auf &#x200B;](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md) neueste Version der Marketo-**durchführen** um sicherzustellen, dass Ihre Integration weiterhin funktioniert.

>[!NOTE]
>
>Marketo aktualisiert die OAuth-Version für GoToWebinar von 1.0 auf 2.0. Die Unterstützung für OAuth 1.0 wird im Januar 2019 eingestellt. Wenn Sie GoToWebinar-Kunde sind, müssen Sie Ihre Anmeldedaten bis zum 31. **2019 über LaunchPoint (im Admin-Bereich) erneut authentifizieren** um sicherzustellen, dass Ihre Integration weiterhin funktioniert. Weitere Informationen finden Sie auf unserer [Community-Seite](https://nation.marketo.com/docs/DOC-6739-gotowebinar-authentication-change-take-action-before-1312019).

## Verbesserungen der Kernplattform {#core-platform-enhancements}

**[E-Mail-CC für Marketo-E-Mails](/help/marketo/product-docs/email-marketing/general/email-cc.md)**

Fügen Sie E-Mails, die über Marketo gesendet werden, bis zu fünf CC-Adressen pro Empfänger hinzu.

**API**

* **Unterstützung von Multi-Branding-Domains für die Asset-API:** Das Genehmigen und Klonen von Assets führt innerhalb der API und Benutzeroberfläche zu denselben Ergebnissen.
* **E-Mail-CC-Unterstützung für Asset**-API: Benutzer, die E-Mails über die API klonen, genehmigen und verarbeiten, bleiben mit den Benutzeroberflächeneinstellungen paritätisch.

**[[!DNL Munchkin] v155 (Beta)](https://developers.marketo.com/javascript-api/lead-tracking/configuration/)**

* **Nur-API-Modus**: Benutzerinnen und Benutzer können jetzt bestimmen, wann und wie Mitglieder ihrer Datenbank verfolgt werden, indem sie zulassen, dass Single Page Web Apps explizit aufrufen, wenn sie einen Web-Seitenbesuch aufzeichnen möchten, anstatt sich auf das automatische Tracking von Marketo zu verlassen.
* **Opt-out-Verwaltung**: Einfaches Verwalten von Opt-outs durch Abgleich der Opt-out-Cookie-Domain mit der [!DNL Munchkin] Tracking-Cookie-Domain.
* **Entscheidungsparameter auf Domain-Ebene**: Zwei-Buchstaben-Domains (d. h. &quot;[website.io](https://website.io)„) werden in Marketo automatisch ohne zusätzliche Setup-Anforderungen verfolgt.

## Marketo Sales Engage {#marketo-sales-engage}

* **[!DNL Salesforce]Benutzerdefiniertes Profil**: Sales Engage unterstützt jetzt unbegrenzt benutzerdefinierte Profile.

* **[!DNL Salesforce]Anpassung**: Durch das Entfernen nicht kritischer benutzerdefinierter Aktivitätsfelder können Benutzer Sales Engage effizienter in der CRM-Plattform einrichten.
* **E-Mail-**: Bessere Zustellbarkeit sowie verbessertes Antwort-Tracking, Funktionen für geplante E-Mails und Funktionen für Massen-E-Mails durch Herstellen einer Verbindung zu [!DNL Microsoft Outlook] (entweder über Office365 oder On-Premise über die Registerkarte E-Mail-Verbindung ).
* **Neue Admin-**: Es wurden zwei Admin-Seiten hinzugefügt, um Ihre Sales Engage-Instanz zu optimieren

   * *Team-Management* unterstützt einen nahtlosen Prozess zur Kontoeinrichtung, indem es Administratoren ermöglicht, Abonnements und Teams zu bearbeiten.
   * *Salesforce-Admin-*: Hilft Teams beim schnelleren und einfacheren Einrichten der SFDC-Synchronisierung als je zuvor.

* **OWA-Plug-in für[!DNL Windows]**: Mit einem einzigen Add-in werden alle [!DNL Windows Office365]-Clients in Sales Engage unterstützt, sodass Live-Feed in Outlook verwendet werden kann. Das neue Plug-in wird im Microsoft Store verfügbar sein.
* **Pusher-Aktivitäten**: Synchronisieren Sie Sales Engage mit der Marketo-Kernplattform, um Echtzeit-Marketing-Erkenntnisse zu nutzen.

## [!DNL Marketo Sky] {#marketo-sky}

>[!NOTE]
>
>[!DNL Marketo Sky] Versionen erfolgen häufiger. Die folgenden Funktionen und Verbesserungen werden voraussichtlich im späten 4. und frühen 1. Quartal veröffentlicht. Weitere Informationen und Updates finden Sie in unserer [Sky-Dokumentation](https://help.marketo.com/).

* **Optionales Standarderlebnis**: Marketo-Benutzende können [!DNL Marketo Sky] als Standarderlebnis festlegen, wenn ihnen der Zugriff durch einen Administrator gewährt wurde.

* **Neu gestaltete meine Marketo**: Passen Sie Ihr Erlebnis an, indem Sie Widgets hinzufügen, die wichtige Informationen, Benachrichtigungen und Links zu Ihren am häufigsten besuchten Bereichen bereitstellen.

* **Design Studio-Listenansichten und -Detailseiten**: Mit filterbaren und durchsuchbaren Listenansichten von E-Mails, Landingpages und Formularen erhalten Sie ein höheres Maß an Organisation und Genauigkeit. Asset-Detailseiten enthalten wichtige Informationen zu jedem Asset, einschließlich der Programme, von denen das Asset verwendet wird, der Anzahl der verwendeten Snippets und mehr.

* **Globale Suche**: Marketo bietet jetzt eine schnellere und robustere globale Suchfunktion für die gesamte Plattform. Suchanfragen erstrecken sich jetzt auf alle barrierefreien Arbeitsbereiche und können nach Assets (aktiv und archiviert), Kennzeichnungen, Kampagnen und Programmen suchen. Suchergebnisse werden über eine Überlagerung bereitgestellt und jedes Ergebnis enthält sein Dateispeicherort-Protokoll, um anzugeben, wo sich das Asset befindet.

* **Verbesserte Benutzeroberfläche**: Neue Symbole, Modale und Schaltflächen sowie eine neue Farbpalette, die unsere Markenerneuerung widerspiegelt und [!DNL Marketo Sky] noch beeindruckender und funktioneller macht.

* **Verbesserungen der Benutzerfreundlichkeit des E-Mail** Programms: Wir arbeiten kontinuierlich an der Parität der E-Mail-Programmfunktionen zwischen unserer klassischen Marketo-Lead-Management-Plattform und dem neuen [!DNL Marketo Sky].
* **Event-With-Webinar Programme**: Event-With-Webinar Programme sind jetzt in [!DNL Marketo Sky] verfügbar (Hinweis: Nur GoToWebinar wird in dieser Version unterstützt, wobei im Laufe der Zeit weitere Integrationen etabliert werden).

## Kundenbezogenes Marketing {#account-based-marketing}

**[ABM - Personabasierte Segmentierung und Filterung](/help/marketo/product-docs/target-account-management/using-personas.md)**

Personalisieren Sie Ihre ABM-Kampagnen für bestimmte Personas in benannten Konten. Die ABM-Persona-Funktion erstellt einen standardmäßigen Auftragstitel basierend auf der Lead-Segmentierung und ermöglicht die Konfiguration zusätzlicher Personensegmente.

## Analytics {#analytics}

**[!DNL Bizible]**

* **Benutzerdefinierte berechnete Felder**: Verwenden Sie ein beliebiges [!DNL Bizible]-Attribut, um benutzerdefinierte Felder zu erstellen, die für die Dashboard-Berichterstellung und -Segmentierung verwendet werden können.

* **SOC II Typ II Zertifizierung**: Die neue Sicherheits- und Datenschutzzertifizierung baut auf der Akkreditierung Typ I von Anfang dieses Jahres auf.

## [!DNL Web Personalization] {#web-personalization}

**[In den Kontoeinstellungen Subdomänen hinzufügen](/help/marketo/product-docs/web-personalization/getting-started/workspaces-in-web-personalization.md)**

Um Domains und Subdomains effizienter zu verwalten, können Benutzer jetzt Subdomains zu ihren RTP-Kontoeinstellungen hinzufügen.

## Marketo Mobile Engagement (MME) {#marketo-mobile-engagement-mme}

**Aktualisiertes MME Software Development Kit (SDK) für Android**

Wir haben unser SDK für Android auf ein moderneres, stabileres und skalierbareres Framework aktualisiert, das mehr Flexibilität und neue technische Funktionen bietet. Entwickler von Android-Apps können jetzt mit diesem neuen SDK direkt [Firebase Cloud Messaging](https://firebase.google.com/docs/cloud-messaging/) (FCM) von Google verwenden.

* [Entwickleranweisungen](https://developers.marketo.com/mobile/installation/#android_adding_fcm_to_your_application)
* [Häufig gestellte Fragen für Entwickler](https://developers.marketo.com/mobile/installation/#android_fcm_faq)

>[!NOTE]
>
>App-Entwickler **müssen** vor dem 31. März 2019 auf die neue Version aktualisieren. Wenn Sie Ihre SDK bis zum 31. März 2019 nicht aktualisieren, können neue Benutzende, die Ihre App nach diesem Datum herunterladen, erst dann Push-Benachrichtigungen erhalten, wenn Sie auf die neueste Version der SDK aktualisiert haben. Für das SDK-Update müssen die aktuellen Benutzenden Ihrer mobilen App keine neue Version Ihrer App herunterladen.

## Zusätzliche Updates {#additional-updates}

**Erweiterbare Webinar-Plattform**

Zusätzlich zu unserer Produktversion arbeitet unser Partnerteam an einem neuen Framework, das es Webinar-Anbietern ermöglicht, ihre eigenen Integrationen mit Marketo zu erstellen und zu pflegen, um mehr Flexibilität bei der Aktualisierung und Verbesserung ihrer Lösungen zu bieten und es Marketing-Experten zu ermöglichen, die ausgewählten Integrationen optimal zu nutzen.

Wir planen, unsere neue Plattform von Fall zu Fall mit den Anbietern auszubauen. Weitere Informationen finden Sie in unseren [Programmdetails](https://www.marketo.com/why-marketo/partners/technology/) oder wenden Sie sich an Ihren Ansprechpartner bei Marketo.
