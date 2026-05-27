---
title: 2019
description: 2019 - Marketo-Dokumente - Produktdokumentation
feature: Release Information
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45id: c5f60233-d5ea-4453-a799-0ad258b4d399id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: d65b4a73-87a3-4d56-b638-74e74d9939ceid: e2290edd-b061-4880-9d79-dee306cf5aa9id: e64968b2-4ee5-47f9-8cae-0588f184b9ebid: ea90ebee-5c84-42d9-8b21-006bdabc95a3id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bccid: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2: id: a1d50dda-6d94-4e16-8c30-5eb7181c4650id: d5c7388a-594e-4d15-9b39-98d6ce479e8bid: de9e3aa9-f002-4fe1-897b-09ee3c55114bid: df8eb12b-4f82-491f-acbb-d74012ca5654id: ffdd6159-0e10-4a57-8021-94e93bab8183
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: bbbea26f-9621-49eb-9ab8-e06fb3bbce8cid: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: d095671a-1355-40aa-8b5f-06c33c68080bid: e0eb8757-182f-49f3-94a4-1587d16f5094id: e1e0219c-f879-479f-8427-888ed2a6e9c2id: eddd9b14-83bd-4ff4-9072-54a4a484abb7id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: 4d4669f3239b43afbcbd660644c8d1a35734a556
workflow-type: tm+mt
source-wordcount: 2528
ht-degree: 3%

---

# 2019

## Winter 2019 {#winter}

Die folgenden Funktionen sind in der Version Winter &#39;19 enthalten. Überprüfen Sie Ihre Marketo Edition auf die Verfügbarkeit der Funktionen.

Bitte klicken Sie auf die Titel-Links, um detaillierte Artikel für jede Funktion anzuzeigen, falls verfügbar.

>[!NOTE]
>
>[!DNL Facebook] benötigt jetzt ein Business Manager-Konto, um Ihre benutzerdefinierte Audience-Integration nutzen zu können. Ihr [!DNL Facebook] LaunchPoint *Service muss* einem Business Manager-Konto zugeordnet sein oder **Ihre Integration funktioniert nach dem 14. Januar 2019 nicht mehr**. Informationen zum Einrichten eines Business Manager-Kontos finden Sie unter [[!DNL Facebook] Hilfe](https://www.facebook.com/business/help/1710077379203657).

>[!NOTE]
>
>Microsoft drängt alle Online-Kunden, auf die neueste Version von [!DNL Microsoft Dynamics] zu aktualisieren. Wenn Sie Ihre Marketo-Instanz mit [!DNL Dynamics Online] integrieren, müssen Sie vor dem 31. [ 2019 ein Upgrade auf ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md) neueste Version der Marketo-**durchführen** um sicherzustellen, dass Ihre Integration weiterhin funktioniert.

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

## Frühjahr 2019 {#spring}

Die folgenden Funktionen sind in der Version vom Frühjahr 1919 enthalten. Überprüfen Sie Ihre Marketo Edition auf die Verfügbarkeit der Funktionen.

Bitte klicken Sie auf die Titel-Links, um detaillierte Artikel für jede Funktion anzuzeigen, falls verfügbar.

***Quartalsveröffentlichungen_**

Die folgenden Funktionen wurden am 15. März 2019 veröffentlicht.

## Verbesserungen der Kernplattform {#core-platform-enhancements}

* **Warteliste:** Neuer Programm-/Ereignisstatus für die Warteliste für ein Mitglied, wenn Sie es [ „zurückstellen“ möchten](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md) bis eine freie Stelle geöffnet wird. Dies gilt für Kanäle, die mit Veranstaltungsprogrammen in Marketo Classic verknüpft sind, und sowohl für Ereignis- als auch für Ereignis-mit-Webinar-Programmen in [!DNL Marketo Sky]. Standardmäßig hat die Warteliste denselben Schrittwert wie „Registriert“.
* **[Benutzerdefiniertes Kommunikationslimit](/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md)**: Administratoren können jetzt benutzerdefinierte tägliche oder wöchentliche Kommunikationslimits festlegen.
* **[Smart Campaign Asset-APIs](https://developers.marketo.com/rest-api/assets/smart-campaigns/)**: Reichern Sie Ihre Analysen außerhalb von Marketo mit dem Abruf von intelligenten Kampagnendatensätzen nach aktualisiertem Datum und aktualisierter ID an.
* **HTTPS-Tracking-Links für E-Mail**: Kunden, die „Sichere Domains für Tracking-Links“ erworben haben, können jetzt Marken-Tracking-Links in Ihren E-Mails als HTTPS anzeigen.
* **Aktualisierungen des E-Mail-Zustellbarkeits-Powerpacks**: Möglichkeit, bestimmte Testergebnisse zu kennzeichnen und zu kommentieren, Ergebnisse über eine URL für Interessengruppen freizugeben und Änderungen zu verfolgen, um die Entwicklung einer E-Mail zu verfolgen, während Interessengruppen Inhalte bearbeiten.

Kundenbezogenes Marketing

**[AccountAI](/help/marketo/product-docs/target-account-management/account-profiling/account-profiling-ranking-and-tuning.md)** Jetzt allgemein verfügbar. AccountAI arbeitet mit künstlicher Intelligenz und zeigt die Kunden an, auf die Sie mit Ihrer ABM-Strategie abzielen sollten.

<br> 

**_Nicht-vierteljährliche Versionen_**

Die folgenden Funktionen werden voraussichtlich im ersten Kalenderquartal und bis zum Beginn des zweiten Quartals 2019 veröffentlicht.

## [!DNL Marketo Sky] {#marketo-sky}

* **Vollständige E-Mail** Programmfunktionalität: Senden Sie E-Mails, erstellen Sie A/B-Tests und verfolgen Sie die Ergebnisse in einem benutzerfreundlichen Erlebnis.
* **Smart Campaign-Funktionalität**: Eine neue Benutzeroberfläche bietet verbesserte Stabilität, da die Funktion für intelligente Kampagnen auch in Sky weiter eingeführt wird.
* **Design Studio Assets verwalten**: Es wurde die Möglichkeit hinzugefügt, Vorlagen, Bilder, Forms, Snippets, Dateien, E-Mails und Landingpages stapelweise aus den Listenansichten von Design Studio zu verwalten.
* **Dashboard für Empfänger-Zeitzonen**: Verstehen Sie das Kundenverhalten mit Berichten für E-Mails, die mit der Zeitzonenfunktion „Versand in Empfänger“ in Sky gesendet werden.

## Marketo Sales Engage {#marketo-sales-engage}

* **Verbesserte Prüfung**: Neue Sichtbarkeit aller Personen, E-Mails und [Inhalte](/help/marketo/product-docs/marketo-sales-connect/templates/view-template-list-as-another-user.md) in einer Instanz mit zusätzlicher Möglichkeit, [ von anderen Benutzern ](/help/marketo/product-docs/marketo-sales-connect/campaigns/view-campaigns-list-as-another-user.md) Kampagnen zu beenden.
* **[Abmeldeverwaltung](/help/marketo/product-docs/marketo-sales-connect/email/unsubscribes/marketo-unsubscribe-check.md)**: Maximieren Sie die Zustellbarkeit und Einhaltung der Möglichkeit, E[Mail-Domains ](/help/marketo/product-docs/marketo-sales-connect/admin/blocked-domains.md) blockieren. Marketo wird vor dem Senden einer E-Mail auch einen Querverweis auf die Lead-Datenbank für Abmeldungen durchführen.

## [!DNL Bizible] von Marketo {#bizible-by-marketo}

* **[!DNL Bizible]Funktionsverbesserungen entdecken**: Neue Dashboard-Segmentierungsfunktionen ermöglichen es Marketing-Experten, die Leistung besser zu verstehen.
* **Unterstützung mehrerer Währungen**: Wechseln Sie zwischen Ihrer Unternehmenswährung und einer beliebigen lokalen Währung mit der neuen automatischen Währungsumrechnungsfunktion von [!DNL Bizible], die auf CRM-Währungstabellen basiert.
* **CRM-Kampagnenkosten**: Messen Sie die Ausgaben und den ROI von Offline-Marketing-Aktivitäten mit der Möglichkeit, automatisch Kostendaten aus dem CRM-Kampagnenobjekt abzurufen.

## Juni 2019 {#june}

Die folgenden Funktionen sind in der Version vom Juni 19 enthalten. Überprüfen Sie Ihre Marketo Edition auf die Verfügbarkeit der Funktionen.

**_Quartalsveröffentlichungen_**

Die folgenden Funktionen wurden am 14. Juni 2019 veröffentlicht.

## Marketo Kernservices {#marketo-core-services}

* **Prüfsumme für Massenextraktionsdatei**: Stellen Sie sicher, dass eine vollständige Datei abgerufen wurde, indem Sie Ihren Datei-Hash mit der Prüfsummenzeichenfolge Ihrer abgeschlossenen Extraktionsaufträge vergleichen.
* **Automatisierte Migration von E-Mail 1.0 zu E-Mail 2.0**: E-Mail 2.0 ist vollständig mit E-Mail 1.0-E-Mails und -Vorlagen kompatibel. Neue Funktionen, z. B. die Möglichkeit, Inhaltselemente (Bilder, Text usw.) zu gruppieren in -Modulen zu erstellen, Variablen wie Zeichenfolge, Farbe, Bild usw. in Vorlagen zu definieren und vollständig responsive Starter-Vorlagen zu nutzen. umfasst außerdem eine visuelle Auswahl für E-Mail-Vorlagen.

>[!CAUTION]
>
>Seit dem 18. Juni 2019 ist E-Mail 1.0 nicht mehr verfügbar. Weitere Informationen zu E-Mail 2.0 und zur Einstellung von E-Mail 1.0 finden [hier](https://nation.marketo.com/docs/DOC-7038).

## Kundenbezogenes Marketing {#account-based-marketing}

* **[!DNL LinkedIn]Account Matching (BETA)** : Eine neue ABM-Funktion ist jetzt in der Beta-Phase verfügbar und bietet Ihnen die Möglichkeit, Listen bekannter und Leerraum-Konten direkt von Marketo an LinkedIn zu senden. Diese Funktion ist automatisch für alle Marketo ABM-Kunden enthalten.

<br> 

**_Veröffentlichung im gesamten Quartal_**

Die folgenden Funktionen werden voraussichtlich im zweiten Kalenderquartal und bis zum Beginn des dritten Quartals 2019 veröffentlicht.

## [!DNL Marketo Sky] {#marketo-sky}

* **Ereignisbegrenzungen** und **Ereignisziele** sind im Allgemeinen in [!DNL Marketo Sky] unter dem Premium-Ereignis-Add-on verfügbar.

   * Event-Caps: Optimieren Sie das Kundenerlebnis für Ihre Veranstaltungen und Webinare mit Registrierungs-Caps, Seitenumleitungen und Wartelistenfunktionen.
   * Veranstaltungsziele: Legen Sie Veranstaltungsregistrierungs- und -teilnahmeziele fest und verfolgen Sie den Fortschritt in Echtzeit.

* **Links zur Vollnavigation**: Wir haben die Navigation für alle zulässigen Anwendungen aktiviert, z. B. Hootsuite, Kalender und mehr.
* **E-Mail-, Landingpage-, Snippet-, Formular-, Bild- und Dateilistenansichten**: Anzeigen, Suchen und Ausführen von Massenaktionen für beliebige Assets in Design Studio.
* **Seite mit Bild-, Datei- und Snippet-Details**: Hier erhalten Sie schnelle Details zu Ihren Assets mit Metadaten wie _erstellt um/_ und Aktionen wie _Löschen_ und _Genehmigen_.
* **Widget „Community-Blogposts**: Greifen Sie auf aktuelle Beiträge aus der Community in My Marketo zu.
* **Bald ablaufendes Widget**: Fügen Sie das Widget „Bald ablaufend“ zu Ihrem Dashboard My Marketo hinzu, um zu sehen, welche Kampagnen und Landingpages als Nächstes ablaufen werden.
* **Weitere Smart List Cards**: Segmentieren und ansprechen Sie sie entsprechend mit zusätzlichen Smart List Cards, einschließlich des Flussschritts „Aufgabe erstellen“, CRM-Smart List-Regeln und mehr.
* **E-Mail-Champion/Challenger-Detailseite**: Sehen Sie Daten wie Gewinnkriterien, Erstellt in usw. von Ihren E-Mail-Champion/Challenger-Tests.

## Marketo [!DNL Sales Connect] {#marketo-sales-connect}

* **Massenaktionen bei der [!DNL Salesforce]-Anpassung**: Maximieren Sie die Produktivität, indem Sie E-Mails senden und Kontakte per [!DNL Salesforce]-Anpassung stapelweise zu Kampagnen hinzufügen.
* **Einstellungen - [!DNL Salesforce] für Administratoren und Nicht-Administratoren**: Verwalten Sie Ihre [!DNL Sales Connect]-Instanz mit einer klaren Ansicht der mit [!DNL Sales Connect] verbundenen [!DNL Salesforce]-Instanz sowie Meine E-Mail, um Aktualisierungen zu [!DNL Salesforce]. Die erweiterten Synchronisierungseinstellungen für Admins, Nicht-Admins und Team Wide Sync werden in den kommenden Monaten veröffentlicht.
* **Einstellungen - Integrationsseite**: Eine zentrale Anlaufstelle für all Ihre Integrationen, damit Sie unser offenes Ökosystem optimal nutzen können.
* **Einstellungen - Profilseite**: Zeigen Sie Ihre Kontodetails an, aktualisieren Sie sie, ändern Sie Ihr Passwort und überprüfen Sie den Status der Implementierung Ihrer Instanz auf dieser neuen Profilseite.

* **System-E-**: Aktualisiertes Design, verbesserte Reaktionsfähigkeit und Internationalisierungsfunktionen.

## [!DNL Bizible] von Marketo {#bizible-by-marketo}

* **Unterstützung mehrerer Währungen für[!DNL Dynamics]**: [!DNL Bizible] passt sich jetzt [!DNL Microsoft Dynamics] Währungstabellen an, sodass Sie einfach zwischen Unternehmens- und lokalen Währungen wechseln können. (Hinweis: Die Unterstützung für SFDC wurde im 1. Quartal 2019 veröffentlicht.)
* **Drift-Integration**: Erfahren Sie, wie sich Drift-Unterhaltungen auf den Journey Ihres Kunden auswirken. [!DNL Bizible] werden auch E-Mail-Adressen aus Konversationen abrufen, um entweder einen neuen Lead zu erstellen oder den Touchpoint mit einem vorhandenen Lead zu verbinden.
* **Lokalisierung**: [!DNL Bizible] ist jetzt in allen von Marketo unterstützten Sprachen verfügbar (Englisch, Japanisch, Deutsch, Spanisch, Französisch und Portugiesisch).

_**Webinar zur Produktversion**_ Sehen Sie sich die Aufzeichnung unseres Webinars mit den Versionsinnovationen vom 19. Juni [hier](https://engage.marketo.com/Marketo-June-Product-Release-2019-On-Demand.html) an.

## August 2019 {#august}

Die folgenden Funktionen sind in der Version vom 19. August enthalten. Überprüfen Sie Ihre Marketo Edition auf die Verfügbarkeit der Funktionen.

**_Quartalsveröffentlichungen_**

Die folgenden Funktionen wurden am 16. August 2019 veröffentlicht.

## Kern-Marketo-Einbindung {#core-marketo-engage}

* **Erweiterbares Webinar-Framework**: Sparen Sie Zeit mit dem neuen vorkonfigurierten Webinar-Framework von Marketo (eingeführt in den Versionshinweisen zum Winter 19), das Daten von Webinar-Anbietern nahtlos an Marketo weiterleitet und umgekehrt. Cvent und Zoom sind jetzt in diesem neuen Framework verfügbar.
* **Aktualisierung der Smart Campaign-API**: Verwalten Sie die Lebenszyklusfunktionen von Smart Campaign, während wir die CRUD-Schnittstelle (Erstellen, Lesen, Aktualisieren, Löschen) abrunden.
* **API-Änderung für E-Mail-Header aktualisieren**: Für die API zum Aktualisieren von E-Mail-Headern ist keine E-Mail mehr mit einer angehängten Vorlage erforderlich, um Header-Felder wie die Betreffzeile zu aktualisieren.

**Account-Based Marketing** ![(Stern)](assets/yellow-star.png)

* **[!DNL LinkedIn]Account Matching**, das sich zuvor in der Beta-Phase befand, ist jetzt allgemein verfügbar.
* **AccountAI** wird offiziell in &quot;**Profiling“**.

<br> 

**_Veröffentlichung im gesamten Quartal_**

Die folgenden Funktionen befinden sich in einem nicht-vierteljährlichen Zyklus und werden im dritten Kalenderquartal und Anfang des 4. Quartals 2019 veröffentlicht.

**[!DNL Marketo Sales Connect]** ![(Stern)](assets/yellow-star.png)

* **Verbesserung des Seiten-Layouts für Personen** Verwalten Sie Personen und Gruppen durch Listenimporte und Massenaktionen im neuen Seiten-Layout für Personen.

>[!AVAILABILITY]
>
>Mit einem Stern ( ![(Stern)](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie vom Marketo-Support.

>[!NOTE]
>
>**Einstellung von TLS 1.0 und 1.1**: Um die Anpassung an den erstklassigen Sicherheitsstandard von Adobe zu gewährleisten, wird die Unterstützung für Transport Layer Security (TLS) 1.0 und 1.1 ab dem 13. Dezember 2019 eingestellt. Bei Systemen, die mit Marketo integriert werden und nicht dem 1.2-Protokoll entsprechen, kann der Zugriff auf Marketo Engage-Services verloren gehen.
>
>**Um Ihren Marketo Engage-Zugriff beizubehalten, stellen Sie sicher, dass alle Client-Systeme vor dem 13. Dezember 2019 TLS 1.2-kompatibel**. Weitere Informationen finden Sie [hier](https://nation.marketo.com/docs/DOC-7059-tls-10-11-deprecation-faq).

**_Webinar zur Produktversion_** [Nehmen Sie ](https://engage.marketo.com/August_19_Release_Webinar.html) 28. August um 1:00PM PT / 4 :00PM ET an einem Live-Webinar teil, das von unserem Produkt-Team veranstaltet wird, und erfahren Sie mehr über die Funktionen dieser Version.
