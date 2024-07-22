---
description: Versionshinweise - Januar 2021 - Marketo-Dokumente - Produktdokumentation
title: Januar 2021 - Versionshinweise
exl-id: 24a5f955-ef4b-4adf-9478-2653db6f9d79
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 1%

---

# Versionshinweise: Januar 2021 {#release-notes-jan-21}

Die folgenden Funktionen sind in der Version vom 21. Januar enthalten. Überprüfen Sie Ihre Marketo-Edition auf Funktionsverfügbarkeit.

>[!AVAILABILITY]
>
>Funktionen, die durch einen Stern (![(star)](assets/yellow-star.png)) gekennzeichnet werden, sind kostenpflichtige Add-ons. Wenden Sie sich an Ihren Marketo Engage-Support-Mitarbeiter, um mehr zu erfahren.

**_Vierteljährliche Versionen_**

Die folgenden Funktionen werden am **15. Januar 2021** veröffentlicht.

## Benutzererlebnis der nächsten Generation {#next-generation-user-experience}

* Unterstützung für Arbeitsbereiche: Das Anwendererlebnis der nächsten Generation von Marketo Engage kombiniert das Erscheinungsbild von Adobe Experience Cloud mit Produktivitätsinnovationen, um Marketing-Experten dabei zu unterstützen, schneller und intelligenter zu arbeiten. In der neuesten Version werden Arbeitsbereiche und Partitionen vollständig unterstützt, einschließlich der Möglichkeit, Ordner über Arbeitsbereiche hinweg freizugeben. Die rechte Arbeitsfläche bietet einen Umschalter, mit dem Sie nahtlos zwischen alten und neuen Erlebnissen pro Funktion wechseln können, ohne den Kontext zu verlieren. [Weitere Informationen](https://nation.marketo.com/t5/The-modern-ux/modern-ux-FAQ/ba-p/307124) finden Sie in den häufig gestellten Fragen zur Marketing-Nation zur nächsten Generation von Erlebnissen.

## Multi-Channel-Personalization {#multi-channel-personalization}

* **[Adobe Experience Cloud Audience Sync Phase 3](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**: Die bestehende Adobe Experience Cloud (AEC)-Funktion zur Zielgruppensynchronisierung unterstützt jetzt die kontinuierliche bidirektionale B2B-Zielsynchronisierung von Marketo Engage mit anderen AEC-Anwendungen, einschließlich Adobe Experience Platform (AEP)-Angeboten wie Real-time Customer Data Platform und Adobe Experience Platform Activation.  Da Leads zu Ihren Zielgruppensegmenten hinzugefügt und entfernt werden, synchronisiert Marketo Engage automatisch die aktualisierte Zielgruppe über Ihre verbundenen AEC-Apps hinweg. Nutzen Sie die Vorteile der kanalübergreifenden Orchestrierung, des erneuten Targetings, der Unterdrückung von Zielgruppen, der Personalisierung und der Berichterstellung von Adobe in Ihrem AEC-Technikstapel.
* **[Kontinuierliche Zielgruppensynchronisierung mit Google, Facebook und LinkedIn](/help/marketo/product-docs/demand-generation/ad-network-integrations/send-a-list-to-an-ad-network.md)**: Kontinuierliche automatisierte Synchronisierung mit einem Anzeigennetzwerk kann auf einer statischen Liste aktiviert werden, wodurch das Anzeigennetzwerk bei Änderungen der Listenmitgliedschaft aktualisiert wird, ohne dass ein Benutzereingriff erforderlich ist.
* **[Token für benutzerdefinierte Felder für Programmmitglieder](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/program-member-custom-field-tokens.md)**: Die benutzerdefinierten Feldfunktionen für Programmmitglieder wurden erweitert, um das Token-Framework zu unterstützen. Marketingexperten können Token für benutzerdefinierte Felder des Programms in E-Mails, Landingpages, SMS-Nachrichten, Push-Benachrichtigungen und Webhooks einfügen. Verwenden Sie neue Token in Kampagnenflussaktionen, um Datenwerte zu ändern, eine Aufgabe zu erstellen oder einen interessanten Moment.

## Landing Pages und Formulare {#landing-pages-and-forms}

* **Formular-API**: Rufen Sie Lead-Informationen oder Trigger-Bereitstellungskampagnen ab, während Sie Daten aus Nicht-Marketo-Formularen abrufen. Nicht-Marketo-Formulare können über die REST-API in Marketo Engage integriert werden. Die neue API bietet die Möglichkeit, die Marketo Engage-Formularübermittlung mit allen zugehörigen Funktionen zu imitieren.
* **Einstiegsseiten-API**: Optimieren Sie die Bearbeitungs- und Übersetzungs-Workflows in integrierten Anwendungen mit der neuen Einstiegsseitenvorschau-API. Drittanbieter können jetzt vollständig personalisierte Vorschauen von Landingpages rendern, ohne sich bei Marketo Engage anzumelden.  Die Landingpage-Vorschau-API ermöglicht durchgängige Bearbeitungs- und Lokalisierungs-Workflows in integrierten Anwendungen von Drittanbietern.

## E-Mail-Marketing {#email-marketing}

* **[Erhöhte benutzerspezifische Abrufgrenzen für Objekte](/help/marketo/product-docs/administration/email-setup/change-custom-object-retrieval-limits-in-velocity-scripting.md)**: Entwickler von E-Mail-Velocity-Skripten können die Anzahl der benutzerdefinierten Objekte schnell auf 100 erhöhen, indem sie die Self-Service-Überschreibung verwenden. Marketingexperten können die Effektivität intelligenter Kampagnen steigern, indem sie auf eine größere Anzahl benutzerdefinierter Objekte der ersten und zweiten Ebene zugreifen.

## Integration von Salesforce CRM {#salesforce-crm-integration}

* [Salesforce CRM-Authentifizierung](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md): Das OAuth 2.0-Protokoll ist für die Synchronisierung von Vorgängen zwischen Marketo Engage und Salesforce CRM verfügbar. Bei neuen Abonnenten ist diese Option standardmäßig aktiviert. Aktuelle Abonnenten können diese Funktion anfordern, indem sie sich an den Marketo-Support wenden.
* [Salesforce CRM-Synchronisierungs-Dashboard](/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.md): Administratoren können den Synchronisierungsstatus von Salesforce CRM schnell über das Dashboard überprüfen. Die Zeitspanne für die Synchronisierung des Leistungsberichts wurde von 2 Stunden auf 5 Tage erhöht.
* **Metadaten-Export**: Erweitert, um Opportunity-Objektattribute, benannte Konten, Standard- und benutzerdefinierte Felder des Programmmitglieds zu unterstützen.

## Administration {#administration}

* **Aktualisierte Seite &quot;Mein Konto&quot;**: Überprüfen Sie die wesentlichen Abonnementinformationen auf der Seite Mein Konto . Benutzer mit beliebigem Zugriff können den Abonnementnamen, die ID des Rechenzentrums und die Munchkin-ID anzeigen.

**_Herausgabe während des gesamten Quartals_**

Die folgenden Funktionen befinden sich in einem nicht vierteljährlichen Zyklus und werden in den kommenden Monaten veröffentlicht.

## Sales Insight {#sales-insight}

![(star)](assets/yellow-star.png)

* **[Verbesserte Test-E-Mail-Workflows (Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/actions-in-the-msi-panel/send-marketo-email/send-a-test-email.md)**: Erhöhen Sie die Effizienz Ihres Verkaufsteams durch verbesserte E-Mail-Workflows für Sales Insight-Tests. Verkäufer können Test-E-Mails an ausgewählte E-Mail-Adressen senden, bevor sie Massen-E-Mails an bis zu 200 Empfänger senden.
* **[Einblicke in den E-Mail-Status (Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/email-tab.md)**: Benutzer sehen eine Warnmeldung, wenn sie versuchen, eine E-Mail an eine ungültige E-Mail-ID oder eine abgemeldete E-Mail-Adresse zu senden, bevor sie eine E-Mail senden.  Der Status des E-Mail-Versands kann im Tab E-Mail von Sales Insight überprüft werden.
* **Massen-E-Mails aus den Bedienfeldern [Konto](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#account-layout) und [Chancen](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#opportunity-layout) senden (Salesforce CRM)**: Erhöhen Sie die Effizienz des Workflows des Verkäufers und interagieren Sie mit einer vollständigen Konto- oder Opportunity-Kontaktliste, indem Sie neue Funktionen für Massenaktionen verwenden. Senden Sie E-Mails oder fügen Sie Kontakte zu Marketo Engage-Kampagnen hinzu, indem Sie die neue Dropdown-Option in den Konto- oder Opportunities-Tabs verwenden, anstatt mit einzelnen Kontakten zu arbeiten. Fügen Sie Kontokontakte zu einer Überwachungsliste hinzu, um benachrichtigt zu werden, wenn Leads heiß werden.
* **[Sales Insight für nicht native Salesforce CRM-Integrationen](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)**: GA-Abonnements mit benutzerdefinierten Salesforce CRM-Integrationen können das Sales Insight-Paket installieren und Verkaufsteams dabei helfen, die viel versprechendsten Leads und Chancen zu priorisieren und mit ihnen zu interagieren.
* **[Best-Bets-Verbesserungen](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/marketo-tab/best-bets.md)**: Kontaktieren Sie Hot-Leads vom Tab &quot;Beste Bets&quot;, indem Sie sie per E-Mail versenden oder einer Marketo Engage-Kampagne hinzufügen. Zeigen Sie einen Lead in Marketo Engage an oder fügen Sie ihn Ihrer Beobachtungsliste hinzu. Massenaktionen und Sortieroptionen auf der Registerkarte &quot;Beste Betas&quot;sparen Zeit und verbessern die Effizienz des Verkaufsteams.

## Sales Connect {#sales-connect}

![(star)](assets/yellow-star.png)

* **Einschränken der E-Mail-Verbindung (BETA)**: Verbessern Sie Ihre E-Mail-Zustellbarkeit und skalieren Sie Ihre 1:1-Verkaufskommunikation mit der Option &quot;Einschränken der E-Mail-Verbindung für Sales Connect&quot;. Unsere neue Drosselungstechnologie verwaltet automatisch das Versandzeitlimit für E-Mails, um nahtlose Erlebnisse für Exchange- und Gmail-Benutzer zu erstellen. Verringern oder eliminieren Sie die Verwendung von Massen-E-Mail-Sendeanwendungen von Drittanbietern.
* **Bounce-Tracking der E-Mail-Verbindung**: Mit dem neuen E-Mail-Bounce-Bericht erhalten Sie Einblicke in die Lead-Qualität und die Leistung von E-Mail-Vorlagen. Exchange- und Gmail-Benutzer können sich für den Empfang von Bounce-Benachrichtigungen entscheiden, die in den Live Feed, E-Mail-Ordner, Vorlagenanalysen und Campaign Analytics aggregiert werden.
* **Profilseitenkonfiguration**: Benutzereinstellungen auf der neuen Profilseite einfach verwalten. Ändern Sie das Kennwort, bearbeiten Sie die Geolocation- und Spracheinstellungen und überprüfen Sie den Integrationsstatus an einer Stelle.
* **Vorlagenverwaltung**: Organisieren Sie E-Mail-Vorlagen für den Vertrieb mit einer neuen Drag &amp; Drop-Funktion in Kategorien, um einen schnellen Zugriff auf relevante Vorlagen zu gewährleisten und die Suchzeit zu verkürzen.
* **Sales Connect User Experience Updates**: Passen Sie das Rasterlayout für Sales Connect an, indem Sie die Größe der Spalten ändern und neu anordnen. Ihre Anzeigevoreinstellungen werden automatisch gespeichert.

**_Mitteilungen und veraltete Elemente_**

* Alle Benutzer müssen vor dem 15. Januar 2021 auf die neueste Version von Sales Insight **aktualisieren.** Wenn Sie das Upgrade nicht abgeschlossen haben, werden Sie nach der Anmeldung bei der Anwendung dazu aufgefordert. Befolgen Sie die Anweisungen [ in diesem Handbuch](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md). Die aktualisierte Version enthält einen Patch für eine identifizierte Sicherheitslücke. Der Patch wurde ursprünglich am 6. April 2016 veröffentlicht. Hinweis: **Versionen 1.4363 oder höher** müssen kein Upgrade durchführen.
* Die Einstellung des Form 1.0-Dienstes tritt in der Version vom **Mai 2021** in Kraft. Der Forms 1.0-Dienst wird vollständig eingestellt, sodass alle verbleibenden Forms 1.0-Assets, die noch verwendet werden, nicht mehr funktionsfähig sind. Darüber hinaus werden Formularübermittlungen, die über nicht unterstützte Methoden durchgeführt werden, wie z. B. programmatische Formular-POSTs an die Endpunkte leadCapture/save und leadCapture/save2, abgelehnt. Weitere Informationen und die Behebung finden Sie in [unserem Beitrag in der Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-the-Marketo-Engage-Form-Platform/ta-p/306631).
* 2021 wird Marketo Engage die URL-Struktur für Landingpages, Formulare, Bilder und Dateien ändern. Für bestehende Marketo Engage-Abonnements werden wir am 1. April 2021 mit der schrittweisen Einführung beginnen. Weitere Informationen zur Rollout-Timeline werden im März 2021 veröffentlicht. Weitere Informationen dazu, wie sich die einzelnen betroffenen Asset-Typen ändern, finden Sie in [unserem Beitrag in der Marketing-Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-Design-Studio-URLs/ta-p/306632).

**_Webinar zur Produktversion_**

Möchten Sie mehr über diese Funktionen und Verbesserungen erfahren? Stellen Sie sicher, dass Sie sich [jetzt registrieren](https://engage.marketo.com/January_21_Release_Webinar_Registration.html) , um am 21. Januar um 13:00 Uhr PT/16:00 Uhr ET für ein Live-Webinar mit unserem Produktteam teilzunehmen, um einen tieferen Einblick in diese Innovationen zu erhalten.
