---
description: Versionshinweise - Januar 2021 - Marketing Docs - Produktdokumentation
title: Versionshinweise - Januar 2021
translation-type: tm+mt
source-git-commit: 073b73255d49f859c32c8b4793e6798f02f7a5c4
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Versionshinweise: Januar 2021 {#release-notes-jan-21}

Die folgenden Funktionen sind in der Version vom 21. Januar enthalten. Überprüfen Sie Ihre Marketo-Edition auf Funktionsverfügbarkeit.

>[!AVAILABILITY]
>
>Mit einem Stern gekennzeichnete Funktionen ( ![(star)](assets/star-yellow.svg)) werden als kostenpflichtige Add-ons bezeichnet. Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zu erhalten.

**_Quartalsversionen_**

Die folgenden Funktionen werden am **15. Januar 2021** veröffentlicht.

## Benutzererlebnis der nächsten Generation {#next-generation-user-experience}

* Unterstützung für Arbeitsbereiche: Das Marketo Engage der nächsten Generation bringt das Aussehen von Adobe Experience Cloud mit Produktivitätsinnovationen zusammen, um Marketingfachleuten dabei zu helfen, schneller und intelligenter zu arbeiten. In der neuesten Version werden Arbeitsbereiche und Partitionen vollständig unterstützt, einschließlich der Möglichkeit, Ordner über Arbeitsbereiche hinweg freizugeben. Auf der rechten Arbeitsfläche wird ein Umschalter Angebot, mit dem Sie eine nahtlose Transition zwischen alten und neuen Erlebnissen pro Funktion ermöglichen können, ohne den Kontext zu verlieren. [Erfahren Sie mehr ](https://nation.marketo.com/t5/The-Next-Generation-Experience/Next-Generation-Experience-FAQ/ba-p/307124) über die FAQ zur Erlebnis-Version der nächsten Generation zur Marketing Nation.

## Personalisierung mehrerer Kanal {#multi-channel-personalization}

* **[Adobe Experience Cloud Audience Sync Phase 3](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**: Die bestehende Synchronisierungsfunktion für Adobe Experience Cloud (AEC)-Audiencen unterstützt jetzt eine kontinuierliche bidirektionale B2B-Audience-Synchronisierung von Marketo Engage zu anderen AEC-Anwendungen, einschließlich Adobe Experience Platform (AEP)-Angeboten wie Echtzeit-Kundendatenplattform und Adobe Experience Platform-Aktivierung.  Da Interessenten zu Ihren Audiencen-Segmenten hinzugefügt und entfernt werden, synchronisiert Marketo Engage die aktualisierte Audience automatisch mit allen angeschlossenen AEC-Apps. Nutzen Sie die Multi-Kanal-Orchestrierung, das Remoteschalten, die Unterdrückung von Audiencen, die Personalisierung und die Verwendung von Berichten in Ihrem AEC-Tech-Stack, um die Vorteile der Adobe zu nutzen.
* **[Kontinuierliche Synchronisierung der Audience mit Google, Facebook und LinkedIn](/help/marketo/product-docs/demand-generation/ad-network-integrations/send-a-list-to-an-ad-network.md)**: Kontinuierlich automatisierte Synchronisierung mit einem Werbenetzwerk kann auf einer statischen Liste aktiviert werden. Dadurch wird das Werbenetzwerk aktualisiert, wenn sich die Mitgliedschaft in der Liste ändert, ohne dass ein Benutzereingriff erforderlich ist.
* **[Token für benutzerdefinierte Felder](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/program-member-custom-field-tokens.md)** für Programm-Member: Die Funktionen für benutzerdefinierte Programm-Mitglieder wurden erweitert, um das Token-Framework zu unterstützen. Marketingexperten können benutzerspezifische Felder in E-Mails, Landingpages, SMS-Nachrichten, Push-Benachrichtigungen und Webhooks einfügen. Verwenden Sie neue Token in Kampagnen-Flussaktionen, um Datenwerte zu ändern, eine Aufgabe oder einen interessanten Moment zu erstellen.

## Landingpages und Forms {#landing-pages-and-forms}

* **Formular-API**: Ziehen Sie Interessenteninformationen oder Trigger-Kampagnen ein, während Sie Daten von Nicht-Marketo-Formularen abrufen. Nicht-Marketo-Formulare können über die REST-API in Marketo Engage integriert werden. Die neue API bietet die Möglichkeit, die Formularübermittlung des Marketo Engages mit allen zugehörigen Funktionen zu imitieren.
* **Landingpages-API**: Mit der neuen Landingpage Vorschau API können Sie Workflows in integrierten Anwendungen optimieren. Drittanbieter können nun vollständig personalisierte Vorschauen von Landingpages wiedergeben, ohne sich bei Marketo Engage anzumelden.  Die Landingpage Vorschau API ermöglicht die durchgängige Bearbeitung und lokale Anpassung von Workflows in integrierten Anwendungen von Drittanbietern.

## Email Marketing {#email-marketing}

* **[Benutzerdefinierte Objekte - Abrufbeschränkungen erhöht](/help/marketo/product-docs/administration/email-setup/change-custom-object-retrieval-limits-in-velocity-scripting.md)**: Entwickler von E-Mail-Velocity Scripting können die Anzahl der benutzerdefinierten Objekte durch Selbstbedienungsüberschreibungen schnell auf 100 erhöhen. Marketingexperten können die Effektivität intelligenter Kampagnen erhöhen, indem sie auf eine größere Anzahl von benutzerdefinierten Objekten der ersten und zweiten Ebene zugreifen.

## Salesforce CRM-Integration {#salesforce-crm-integration}

* [Salesforce CRM-Authentifizierung](/help/marketo/product-docs/crm-sync/salesforce-sync/setting-up-oauth-2-0.md): Das OAuth 2.0-Protokoll ist für die Synchronisierung von Operationen zwischen Marketo Engage und Salesforce CRM verfügbar. Bei neuen Abonnenten ist diese Option standardmäßig aktiviert. Aktuelle Abonnenten können diese Funktion anfordern, indem sie sich an den Marketing Support wenden.
* [Salesforce CRM Syncing-Dashboard](/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.md): Administratoren können den Salesforce CRM-Synchronisierungsstatus aus dem Dashboard schnell überprüfen. Die Zeitspanne für die Synchronisierung der Leistungsberichte wurde von 2 Stunden auf 5 Tage erhöht.
* **Metadatenexport**: Erweitert zur Unterstützung von Opportunitätsobjektattributen, benannten Konten, Standardfeldern und benutzerdefinierten Feldern des Programm-Mitglieds.

## Administration {#administration}

* **Seite** &quot;Mein Konto&quot;wurde aktualisiert: Überprüfen Sie die wichtigen Abonnement-Informationen auf der Seite &quot;Mein Konto&quot;. Benutzer mit einer beliebigen Zugriffsebene können den Abonnement, die ID des Rechenzentrums und die Munchkin-ID Ansicht haben.

**_Veröffentlichung im gesamten Quartal_**

Die folgenden Funktionen befinden sich in einem nicht vierteljährlichen Zyklus und werden in den kommenden Monaten veröffentlicht.

## Sales Insight {#sales-insight}

![(Stern)](assets/star-yellow.svg)

* **[Erweiterte Test-E-Mail-Workflows (Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/actions-in-the-msi-panel/send-marketo-email/send-a-test-email.md)**: Erhöhen Sie die Effizienz Ihres Verkaufsteams durch verbesserte E-Mail-Workflows von Sales Insight. Verkäufer können Test-E-Mails an ausgewählte E-Mail-Adressen senden, bevor sie Massen-E-Mails an bis zu 200 Empfänger senden.
* **[Einblicke in den E-Mail-Status (Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/email-tab.md)**: Benutzern wird eine Warnmeldung angezeigt, wenn sie versuchen, eine E-Mail an eine ungültige E-Mail-ID oder eine nicht abonnierte E-Mail-Adresse zu senden, bevor sie eine E-Mail senden.  Die Statusangaben des E-Mail-Versands können auf der Registerkarte &quot;E-Mail&quot;von Sales Insight überprüft werden.
* **Senden von Massen-E-Mails aus  [](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#account-layout) Konten und  [](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#opportunity-layout) OpportunityPanels (Salesforce CRM)**: Verbessern Sie die Effizienz des Arbeitsablaufs des Verkäufers und arbeiten Sie mit der gesamten Liste von Kontakt- oder Gelegenheitskontakten, indem Sie neue Funktionen für Massenaktionen verwenden. Senden Sie E-Mails oder fügen Sie Marketo Engage-Kampagnen Kontakte hinzu, indem Sie die neue Dropdown-Option auf den Registern &quot;Konto&quot;oder &quot;Gelegenheit&quot;verwenden, anstatt mit einzelnen Kontakten zu arbeiten. hinzufügen Kontokontakte zu einer Überwachungsliste, die benachrichtigt werden soll, wenn Leads heiß werden.
* **[Sales Insight für nicht-native Salesforce CRM-Integrationen](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)**: GA-Abonnement mit benutzerdefinierten Salesforce CRM-Integrationen können das Sales Insight-Paket installieren und Vertriebsteams dabei unterstützen, die viel versprechendsten Interessenten und Chancen zu priorisieren und mit ihnen zu interagieren.
* **[Best-Beta-Verbesserungen](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/marketo-tab/best-bets.md)**: Kontaktieren Sie Hotspots schnell über das Register Beste Betten, indem Sie sie per E-Mail versenden oder einer Marketo Engage-Kampagne hinzufügen. Ansicht eines Interessenten in Marketo Engage oder fügen Sie ihn Ihrer Überwachungsliste hinzu. Massenaktionen und Sortieroptionen auf der Registerkarte Beste Betten sparen Zeit und verbessern die Effizienz des Verkaufsteams.

## Sales Connect {#sales-connect}

![(Stern)](assets/star-yellow.svg)

* **Einschränken der E-Mail-Verbindung (BETA)**: Verbessern Sie Ihre E-Mail-Zustellbarkeit und skalieren Sie Ihre 1:1-Verkaufskommunikation mit E-Mail-Verbindungssperre für Sales Connect. Unsere neue Drosselungstechnologie verwaltet automatisch das Timing von E-Mails, um nahtlose Erlebnisse für Exchange- und Gmail-Benutzer zu schaffen. Verringern oder beseitigen Sie die Verwendung von Massen-E-Mail-Sendeanwendungen von Drittanbietern.
* **Nachverfolgung** des Absprungs von E-Mail-Verbindungen: Erhalten Sie mit dem neuen E-Mail-Absprungbericht Einblicke in die Qualität der Interessenten und die Leistung der E-Mail-Vorlage. Exchange- und Gmail-Benutzer können Absprungbenachrichtigungen empfangen, die in den Live-Feed, E-Mail-Ordner, Vorlagenanalysen und Kampagne Analytics aggregiert werden.
* **Profil-Seitenkonfiguration**: Benutzervoreinstellungen auf der Seite &quot;Neues Profil&quot;problemlos verwalten. Ändern Sie das Kennwort, bearbeiten Sie Geolocation- und Spracheinstellungen und überprüfen Sie die Integrationsstatus an einer Stelle.
* **Vorlagen-Management**: Organisieren Sie E-Mail-Vorlagen für den Vertrieb in Kategorien mit einer neuen Drag &amp; Drop-Funktion, um schnell auf relevante Vorlagen zuzugreifen und die Suchzeit zu verkürzen.
* **Sales Connect-Benutzererfahrungsaktualisierungen**: Passen Sie das Rasterlayout von Sales Connect an, indem Sie die Größe und Anordnung der Spalten ändern. Ihre Anzeigevoreinstellungen werden automatisch gespeichert.

**_Mitteilungen und Veraltungen_**

* Alle Benutzer müssen vor dem 15. Januar 2021 auf die neueste Version von Sales Insight aktualisieren. **** Wenn Sie die Aktualisierung noch nicht abgeschlossen haben, werden Sie nach der Anmeldung bei der Anwendung dazu aufgefordert. Befolgen Sie die Anweisungen [in diesem Handbuch](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md). Die aktualisierte Version enthält einen Patch für eine identifizierte Sicherheitslücke. Der Patch wurde ursprünglich am 6. April 2016 veröffentlicht. Hinweis: **Versionen 1.4363 oder höher** müssen keine Aktualisierung durchführen.
* Der Dienst &quot;Form 1.0&quot;wird ab der Version **Mai 2021** veraltet. Der Forms 1.0-Dienst wird vollständig eingestellt, sodass alle verbleibenden Forms 1.0-Assets, die noch verwendet werden, nicht mehr funktionsfähig sind. Formularübermittlungen, die mit nicht unterstützten Methoden durchgeführt wurden, wie z. B. programmatische Formular-POSTs an die Endpunkte leadCapture/save und leadCapture/save2, werden ebenfalls abgelehnt. Weitere Informationen und Abhilfemaßnahmen finden Sie in [unserem Beitrag in Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-the-Marketo-Engage-Form-Platform/ta-p/306631).
* 2021 wird Marketo Engage die URL-Struktur für Landingpages-, Formular-, Bild- und Dateielemente ändern. Für bestehende Marketo Engage-Abonnements werden wir am 1. April 2021 mit der schrittweisen Einführung beginnen. Weitere Einzelheiten zur Zeitschiene für die Einführung werden im März 2021 veröffentlicht. Weitere Informationen zur Änderung der einzelnen betroffenen Asset-Typen finden Sie in [unserem Beitrag in Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-Design-Studio-URLs/ta-p/306632).

**_Webinar zur Produktversion_**

Möchten Sie mehr über diese Funktionen und Verbesserungen erfahren? Stellen Sie sicher, dass [registrieren Sie sich jetzt](https://engage.marketo.com/January_21_Release_Webinar_Registration.html), um am 21. Januar um 13:00 PM PT / 16:00 PM ET für ein Live-Webinar mit unserem Produktteam teilzunehmen, um einen tieferen Einstieg in diese Innovationen zu finden.
