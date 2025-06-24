---
description: Versionshinweise - Januar 2021 - Marketo-Dokumentation - Produktdokumentation
title: Versionshinweise - Januar 2021
exl-id: 24a5f955-ef4b-4adf-9478-2653db6f9d79
feature: Release Information
source-git-commit: ecd225af3ecfd7cb9159faf5a9d384d47ee6312c
workflow-type: tm+mt
source-wordcount: '1236'
ht-degree: 0%

---

# Versionshinweise: Januar 2021 {#release-notes-jan-21}

Die folgenden Funktionen sind in der Version vom Januar 2021 enthalten. Überprüfen Sie Ihre Marketo Edition auf die Verfügbarkeit der Funktionen.

>[!AVAILABILITY]
>
>Mit einem Stern (![(Stern)](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie vom Marketo Engage-Support.

**_Quartalsveröffentlichungen_**

Die folgenden Funktionen werden am (**. Januar 2021)**.

## Benutzererlebnis der nächsten Generation {#next-generation-user-experience}

* Unterstützung für Arbeitsbereiche: Das Benutzererlebnis der nächsten Generation von Marketo Engage vereint das Erscheinungsbild von Adobe Experience Cloud mit Produktivitätsinnovationen, damit Marketing-Experten schneller und intelligenter arbeiten können. In der neuesten Version fügen wir vollständige Unterstützung für Arbeitsbereiche und Partitionen hinzu, einschließlich der Möglichkeit, Ordner über Arbeitsbereiche hinweg freizugeben. Die rechte Arbeitsfläche bietet einen Umschalter, mit dem Sie nahtlos zwischen alten und neuen Erlebnissen pro Funktion wechseln können, ohne den Kontext zu verlieren. [Erfahren Sie mehr](https://nation.marketo.com/t5/The-modern-ux/modern-ux-FAQ/ba-p/307124) aus den häufig gestellten Fragen zur nächsten Generation zu Marketing Nation.

## Multi-Channel Personalization {#multi-channel-personalization}

* **[Adobe Experience Cloud-Zielgruppensynchronisierungsphase 3](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**: Die bestehende Zielgruppensynchronisierungsfunktion von Adobe Experience Cloud (AEC) unterstützt jetzt die kontinuierliche, bidirektionale B2B-Zielgruppensynchronisierung von Marketo Engage mit anderen AEC-Anwendungen, einschließlich Adobe Experience Platform (AEP)-Angeboten wie Real-time Customer Data Platform und Adobe Experience Platform Activation.  Wenn Leads hinzugefügt und aus Ihren Zielgruppensegmenten entfernt werden, synchronisiert Marketo Engage die aktualisierte Zielgruppe automatisch über Ihre verbundenen AEC-Mobile-Apps. Nutzen Sie die Vorteile der Multi-Channel-Orchestrierung, des Re-Targeting, der Unterdrückung von Zielgruppen, der Personalisierung und des Reportings von Adobe in Ihrem gesamten AEC-Technologie-Stack.
* **[Kontinuierliche Zielgruppensynchronisierung mit Google,  [!DNL Facebook] und [!DNL LinkedIn]](/help/marketo/product-docs/demand-generation/ad-network-integrations/send-a-list-to-an-ad-network.md)**: Die kontinuierlich automatisierte Synchronisierung mit einem Werbenetzwerk kann in einer statischen Liste aktiviert werden, wobei das Werbenetzwerk aktualisiert wird, wenn sich die Listenmitgliedschaft ändert, ohne dass ein Benutzereingriff erforderlich ist.
* **[Token für benutzerdefinierte Felder für Programmteilnehmer](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/program-member-custom-field-tokens.md)**: Wir haben die benutzerdefinierten Feldfunktionen für Programmteilnehmer erweitert, um das Token-Framework zu unterstützen. Marketing-Experten können benutzerdefinierte Felder für Programmteilnehmer in E-Mails, Landingpages, SMS-Nachrichten, Push-Benachrichtigungen und Webhooks einfügen. Verwenden Sie neue Token in Kampagnen-Flussaktionen, um Datenwerte zu ändern, eine Aufgabe zu erstellen oder einen interessanten Moment zu erleben.

## Landing Pages und Formulare {#landing-pages-and-forms}

* **Formular-API**: Holen Sie Lead-Informationen oder Trigger-Pflegekampagnen ein, während Sie Daten aus Nicht-Marketo-Formularen abrufen. Nicht-Marketo-Formulare können über die REST-API in Marketo Engage integriert werden. Die neue API bietet die Möglichkeit, die Übermittlung von Marketo Engage-Formularen mit allen zugehörigen Funktionen zu imitieren.
* **Landingpages-API**: Optimieren Sie die Bearbeitungs- und Übersetzungs-Workflows in integrierten Anwendungen mit der neuen Landingpage-Vorschau-API. Drittanbieter können jetzt vollständig personalisierte Vorschauen von Landingpages rendern, ohne sich bei Marketo Engage anzumelden.  Die Landingpage-Vorschau-API ermöglicht End-to-End-Bearbeitungs- und Lokalisierungs-Workflows in integrierten Anwendungen von Drittanbietern.

## E-Mail-Marketing {#email-marketing}

* **[Abrufbeschränkungen für benutzerdefinierte Objekte erhöht](/help/marketo/product-docs/administration/email-setup/change-custom-object-retrieval-limits-in-velocity-scripting.md)**: Entwickler von E-Mail-Velocity-Skripten können die Anzahl der benutzerdefinierten Objekte durch Selbstüberschreibungen schnell auf 100 erhöhen. Marketing-Experten können die Effektivität von Smart-Kampagnen steigern, indem sie auf eine größere Anzahl benutzerdefinierter Objekte der ersten und zweiten Ebene zugreifen.

## [!DNL Salesforce] CRM-Integration {#salesforce-crm-integration}

* [[!DNL Salesforce] CRM-Authentifizierung](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md): Das OAuth 2.0-Protokoll ist für Synchronisierungsvorgänge zwischen Marketo Engage und [!DNL Salesforce] CRM verfügbar. Für neue Abonnenten ist diese Option standardmäßig aktiviert. Aktuelle Abonnentinnen und Abonnenten können diese Funktion anfordern, indem sie sich an den Marketo Support wenden.
* [[!DNL Salesforce] CRM-Synchronisierungs-Dashboard](/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.md): Administratoren können [!DNL Salesforce] CRM-Synchronisierungsstatus schnell über das Dashboard überprüfen. Die Zeitspanne für das Synchronisieren von Leistungsberichten wurde von 2 Stunden auf 5 Tage erhöht.
* **Metadatenexport**: wurde verbessert, um Opportunity-Objektattribute, benannte Konten, Standard- und benutzerdefinierte Felder des Programmmitglieds zu unterstützen.

## Administration {#administration}

* **Seite Mein Konto wurde aktualisiert**: Überprüfen Sie wichtige Abonnementinformationen auf der Seite Mein Konto. Benutzer mit beliebiger Zugriffsebene können den Abonnementnamen, die Datenzentrum-Kennung und die [!DNL Munchkin]-ID anzeigen.

**_Veröffentlichung im gesamten Quartal_**

Die folgenden Funktionen befinden sich in einem nicht vierteljährlichen Zyklus und werden in den kommenden Monaten veröffentlicht.

## [!DNL Sales Insight] {#sales-insight}

![(Stern)](assets/yellow-star.png)

* **[Verbesserte Test-E-Mail-Workflows ([!DNL Salesforce] CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/actions-in-the-msi-panel/send-marketo-email/send-a-test-email.md)**: Erhöhen Sie die Effizienz Ihres Vertriebsteams durch verbesserte [!DNL Sales Insight] Test-E-Mail-Workflows. Verkäufer können Test-E-Mails an ausgewählte E-Mail-Adressen senden, bevor sie Massen-E-Mails an bis zu 200 Empfänger senden.
* **[Einblicke in den E-Mail-Status ([!DNL Salesforce] CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/email-tab.md)**: Benutzende sehen eine Warnmeldung, wenn sie versuchen, eine E-Mail an eine ungültige E-Mail-ID oder eine abgemeldete E-Mail-Adresse zu senden, bevor sie eine E-Mail senden.  Der Status des E-Mail-Versands kann auf der Registerkarte E-Mail von [!DNL Sales Insight] eingesehen werden.
* **Massen-E-Mails über [Konto](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#account-layout) und [Opportunity](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#opportunity-layout)-Bedienfelder ([!DNL Salesforce] CRM) senden**: Verbessern Sie die Effizienz des Workflows des Verkäufers und interagieren Sie mit einer ganzen Konto- oder Opportunity-Kontaktliste durch die Verwendung neuer Massenaktionsfunktionen. Senden Sie E-Mails oder fügen Sie Kontakte zu Marketo Engage-Kampagnen hinzu, indem Sie die neue Dropdown-Option auf den Registerkarten Konto oder Opportunity verwenden, anstatt mit einzelnen Kontakten zu arbeiten. Fügen Sie Account-Kontakte zu einer Watchlist hinzu, um benachrichtigt zu werden, wenn Leads heiß werden.
* **[[!DNL Sales Insight] Für Nicht-Native- [!DNL Salesforce] -CRM-Integrationen](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)**: GA-Abonnements mit benutzerdefinierten Salesforce CRM-Integrationen können das [!DNL Sales Insight] installieren und Vertriebsteams dabei helfen, Prioritäten zu setzen und mit den viel versprechendsten Leads und Chancen zu interagieren.
* **[Best-Bets-Verbesserungen](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/marketo-tab/best-bets.md)**: Kontaktieren Sie schnell die besten Leads auf der Registerkarte Best-Bets , indem Sie sie per E-Mail versenden oder zu einer Marketo Engage-Kampagne hinzufügen. Zeigen Sie einen Lead in Marketo Engage an oder fügen Sie ihn Ihrer Watchlist hinzu. Massenaktionen und Sortieroptionen auf der Registerkarte [!UICONTROL Best ]&quot; sparen Zeit und verbessern die Effizienz des Vertriebsteams.

## [!DNL Sales Connect] {#sales-connect}

![(Stern)](assets/yellow-star.png)

* **Drosselung der E-Mail-Verbindung (BETA)**: Verbessern Sie die Zustellbarkeit Ihrer E-Mails und skalieren Sie Ihre 1:1-Vertriebskommunikation mit Drosselung der E-Mail-Verbindung für [!DNL Sales Connect]. Unsere neue Drosselungstechnologie verwaltet automatisch die Versandzeit von E-Mails, um [!DNL Exchange]- und Gmail-Benutzern nahtlose Erlebnisse zu bieten. Verringern oder beseitigen Sie die Verwendung von Massenversand-Programmen von Drittanbietern.
* **Tracking von E-Mail** Verbindungs-Bounces: Gewinnen Sie mit dem neuen E-Mail-Bounce-Bericht insight in die Lead-Qualität und die Leistung Ihrer E-Mail-Vorlage. Benutzer von [!DNL Exchange] und Gmail können Bounce-Benachrichtigungen auswählen, die für den Live-Feed, die E-Mail-Ordner, die Vorlagenanalyse und Campaign Analytics gelten.
* **Profilseitenkonfiguration**: Benutzereinstellungen auf der neuen Profilseite problemlos verwalten. Ändern Sie Ihr Passwort, bearbeiten Sie Geolokalisierungs- und Spracheinstellungen und überprüfen Sie die Integrationsstatus an einer Stelle.
* **Vorlagenverwaltung**: Organisieren Sie Verkaufs-E-Mail-Vorlagen mithilfe einer neuen Drag-and-Drop-Funktion in Kategorien, um den schnellen Zugriff auf relevante Vorlagen zu gewährleisten und die Suchzeit zu verkürzen.
* **[!DNL Sales Connect]Aktualisierungen des Benutzererlebnisses**: Passen Sie [!DNL Sales Connect] Rasterlayout an, indem Sie die Größe der Spalten ändern und sie neu anordnen. Ihre Anzeigeeinstellungen werden automatisch gespeichert.

**_Ankündigungen und Veraltungen_**

* Alle Benutzer müssen ein Upgrade auf die neueste Version von Sales Insight **vor dem 15. Januar 2021** durchführen. Wenn Sie das Upgrade nicht abgeschlossen haben, werden Sie beim Anmelden bei der Anwendung dazu aufgefordert. Befolgen Sie die Anweisungen [in diesem Handbuch](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md). Die aktualisierte Version enthält einen Patch für eine erkannte Sicherheitslücke. Der Patch wurde ursprünglich am 6. April 2016 veröffentlicht. Hinweis: **Versionen 1.4363 oder höher** müssen kein Upgrade durchführen.
* Die Einstellung des Form 1.0-Service tritt in der Version **Mai 2021** in Kraft. Der Forms 1.0-Service wird vollständig veraltet sein, was zum Verlust der Funktionalität aller verbleibenden Forms 1.0-Assets führt, die noch in Verwendung sind. Formularübermittlungen, die über nicht unterstützte Methoden wie programmgesteuerte Formular-POSTs an die Endpunkte „leadCapture/save“ und „leadCapture/save2“ erfolgen, werden ebenfalls abgelehnt. Weitere Informationen und Fehlerbehebungen finden Sie unter [Unser Beitrag in Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-the-Marketo-Engage-Form-Platform/ta-p/306631).
* Im Jahr 2021 wird Marketo Engage Änderungen an der URL-Struktur für Landingpages, Formulare sowie Bild- und Dateielemente vornehmen. Für bestehende Marketo Engage-Abonnements beginnt der schrittweise Rollout am 1. April 2021. Weitere Informationen zur Rollout-Zeitleiste werden im März 2021 veröffentlicht. Einzelheiten dazu, wie sich die einzelnen betroffenen Asset-Typen ändern, finden Sie in [unserem Beitrag in Marketing Nation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-Design-Studio-URLs/ta-p/306632).

**_Webinar zur Produktversion_**

Möchten Sie mehr über diese Funktionen und Verbesserungen erfahren? Melden Sie [ jetzt an](https://engage.marketo.com/January_21_Release_Webinar_Registration.html) um am 21. Januar um 13:00 Uhr PT / 16:00 Uhr ET an einem Live-Webinar mit unserem Produkt-Team teilzunehmen, um einen tieferen Einblick in diese Innovationen zu erhalten.
