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
>Mit einem Stern (![(Stern)](assets/yellow-star.png)) sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie von Ihrem Marketo Engage-Support-Mitarbeiter.

**_Vierteljährliche Versionen_**

Die folgenden Funktionen werden veröffentlicht auf **15. Januar 2021**.

## Benutzererlebnis der nächsten Generation {#next-generation-user-experience}

* Unterstützung für Arbeitsbereiche: Das Marketo Engage der nächsten Generation kombiniert das Erscheinungsbild von Adobe Experience Cloud mit Produktivitätsinnovationen, um Marketing-Experten dabei zu unterstützen, schneller und intelligenter zu arbeiten. In der neuesten Version werden Arbeitsbereiche und Partitionen vollständig unterstützt, einschließlich der Möglichkeit, Ordner über Arbeitsbereiche hinweg freizugeben. Die rechte Arbeitsfläche bietet einen Umschalter, mit dem Sie nahtlos zwischen alten und neuen Erlebnissen pro Funktion wechseln können, ohne den Kontext zu verlieren. [Weitere Infos](https://nation.marketo.com/t5/The-modern-ux/modern-ux-FAQ/ba-p/307124) aus den FAQ zur nächsten Generation von Erlebnissen in der Marketingnation.

## Multi-Channel-Personalisierung {#multi-channel-personalization}

* **[Adobe Experience Cloud Audience Sync Phase 3](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/send-a-list-to-adobe-experience-cloud.md)**: Die bestehende Funktion zur Zielgruppensynchronisierung von Adobe Experience Cloud (AEC) unterstützt jetzt die kontinuierliche bidirektionale B2B-Zielsynchronisierung von Marketo Engage mit anderen AEC-Anwendungen, einschließlich Adobe Experience Platform (AEP)-Angeboten wie Real-time Customer Data Platform und Adobe Experience Platform Activation.  Da Leads zu Ihren Zielgruppensegmenten hinzugefügt und entfernt werden, synchronisiert Marketo Engage die aktualisierte Zielgruppe automatisch über Ihre verbundenen AEC-Apps hinweg. Verwenden Sie sie, um die Anwendungsfälle für die kanalübergreifende Orchestrierung, das erneute Targeting, die Unterdrückung von Zielgruppen, die Personalisierung und die Berichterstellung von Adobe in Ihrem AEC-Technikstapel zu nutzen.
* **[Kontinuierliche Zielgruppensynchronisierung mit Google, Facebook und LinkedIn](/help/marketo/product-docs/demand-generation/ad-network-integrations/send-a-list-to-an-ad-network.md)**: Kontinuierliche automatisierte Synchronisierung mit einem Werbenetzwerk kann auf einer statischen Liste aktiviert werden, wodurch das Werbenetzwerk bei Änderungen der Listenmitgliedschaft aktualisiert wird, ohne dass ein Benutzereingriff erforderlich ist.
* **[Token für benutzerdefinierte Felder für Programmmitglieder](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/program-member-custom-field-tokens.md)**: Die benutzerdefinierten Feldfunktionen für Programmmitglieder wurden erweitert, um das Token-Framework zu unterstützen. Marketingexperten können Token für benutzerdefinierte Felder des Programms in E-Mails, Landingpages, SMS-Nachrichten, Push-Benachrichtigungen und Webhooks einfügen. Verwenden Sie neue Token in Kampagnenflussaktionen, um Datenwerte zu ändern, eine Aufgabe zu erstellen oder einen interessanten Moment.

## Landing Pages und Formulare {#landing-pages-and-forms}

* **Formular-API**: Rufen Sie Lead-Informationen oder Trigger-Pflegekampagnen ab, während Sie Daten aus Nicht-Marketo-Formularen abrufen. Nicht-Marketo-Formulare können über die REST-API in Marketo Engage integriert werden. Die neue API bietet die Möglichkeit, die Übermittlung von Marketo Engage-Formularen mit allen zugehörigen Funktionen zu imitieren.
* **Landingpage-API**: Optimieren Sie Bearbeitungs- und Übersetzungs-Workflows in integrierten Anwendungen mit der neuen Landingpage-Vorschau-API. Drittanbieter können jetzt vollständig personalisierte Vorschauen von Landingpages rendern, ohne sich bei Marketo Engage anzumelden.  Die Landingpage-Vorschau-API ermöglicht durchgängige Bearbeitungs- und Lokalisierungs-Workflows in integrierten Anwendungen von Drittanbietern.

## E-Mail-Marketing {#email-marketing}

* **[Erhöhte Rückrufgrenzen für benutzerdefinierte Objekte](/help/marketo/product-docs/administration/email-setup/change-custom-object-retrieval-limits-in-velocity-scripting.md)**: Entwickler von E-Mail-Velocity-Skripten können die Anzahl der benutzerdefinierten Objekte durch das Überschreiben der Self-Service-Funktion schnell auf 100 erhöhen. Marketingexperten können die Effektivität intelligenter Kampagnen steigern, indem sie auf eine größere Anzahl benutzerdefinierter Objekte der ersten und zweiten Ebene zugreifen.

## Integration von Salesforce CRM {#salesforce-crm-integration}

* [Salesforce CRM-Authentifizierung](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md): Das OAuth 2.0-Protokoll steht für Synchronisierungsvorgänge zwischen Marketo Engage und Salesforce CRM zur Verfügung. Bei neuen Abonnenten ist diese Option standardmäßig aktiviert. Aktuelle Abonnenten können diese Funktion anfordern, indem sie sich an den Marketo-Support wenden.
* [Salesforce CRM-Synchronisierungs-Dashboard](/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-errors.md): Administratoren können den Status der Salesforce CRM-Synchronisierung schnell über das Dashboard überprüfen. Die Zeitspanne für die Synchronisierung des Leistungsberichts wurde von 2 Stunden auf 5 Tage erhöht.
* **Metadatenexport**: Verbessert zur Unterstützung von Opportunity-Objektattributen, benannten Konten, den Standard- und benutzerdefinierten Feldern des Programmmitglieds.

## Administration {#administration}

* **Seite &quot;Mein Konto&quot;aktualisiert**: Überprüfen Sie die wesentlichen Abonnementinformationen auf der Seite Mein Konto . Benutzer mit beliebigem Zugriff können den Abonnementnamen, die ID des Rechenzentrums und die Munchkin-ID anzeigen.

**_Herausgabe im gesamten Quartal_**

Die folgenden Funktionen befinden sich in einem nicht vierteljährlichen Zyklus und werden in den kommenden Monaten veröffentlicht.

## Sales Insight {#sales-insight}

![(Stern)](assets/yellow-star.png)

* **[Verbesserte Test-E-Mail-Workflows (Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/actions-in-the-msi-panel/send-marketo-email/send-a-test-email.md)**: Erhöhen Sie die Effizienz Ihres Verkaufsteams durch verbesserte E-Mail-Workflows für Sales Insight-Tests. Verkäufer können Test-E-Mails an ausgewählte E-Mail-Adressen senden, bevor sie Massen-E-Mails an bis zu 200 Empfänger senden.
* **[Einblicke in den E-Mail-Status (Salesforce CRM)](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/email-tab.md)**: Benutzer erhalten eine Warnmeldung, wenn sie versuchen, eine E-Mail vor dem Versand einer E-Mail an eine ungültige E-Mail-ID oder eine abgemeldete E-Mail-Adresse zu senden.  Der Status des E-Mail-Versands kann im Tab E-Mail von Sales Insight überprüft werden.
* **Massen-E-Mails senden aus [Konto](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#account-layout) und [Chancen](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/msi-feature-overview.md#opportunity-layout) Bedienfelder (Salesforce CRM)**: Verbessern Sie die Effizienz des Workflows des Verkäufers und interagieren Sie mit einer vollständigen Konto- oder Opportunity-Kontaktliste, indem Sie neue Massenaktionen verwenden. Senden Sie E-Mails oder fügen Sie Marketo Engage-Kampagnen Kontakte hinzu, indem Sie die neue Dropdown-Option in den Konto- oder Opportunity-Tabs verwenden, anstatt mit einzelnen Kontakten zu arbeiten. Fügen Sie Kontokontakte zu einer Überwachungsliste hinzu, um benachrichtigt zu werden, wenn Leads heiß werden.
* **[Sales Insight für nicht native Salesforce CRM-Integrationen](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)**: GA-Abonnements mit benutzerdefinierten Salesforce CRM-Integrationen können das Sales Insight-Package installieren und Verkaufsteams dabei helfen, die viel versprechendsten Leads und Chancen zu priorisieren und mit ihnen zu interagieren.
* **[Best-Beta-Verbesserungen](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/marketo-tab/best-bets.md)**: Kontaktieren Sie im Tab Beste Betas schnell Hot Leads, indem Sie sie per E-Mail versenden oder einer Marketo Engage-Kampagne hinzufügen. Zeigen Sie einen Lead in Marketo Engage an oder fügen Sie ihn Ihrer Beobachtungsliste hinzu. Massenaktionen und Sortieroptionen auf der Registerkarte &quot;Beste Betas&quot;sparen Zeit und verbessern die Effizienz des Verkaufsteams.

## SalesConnect {#sales-connect}

![(Stern)](assets/yellow-star.png)

* **Einschränken der E-Mail-Verbindung (BETA)**: Verbessern Sie Ihre E-Mail-Zustellbarkeit und skalieren Sie Ihre 1:1-Verkaufskommunikation mit E-Mail-Verbindungsbegrenzung für Sales Connect. Unsere neue Drosselungstechnologie verwaltet automatisch das Versandzeitlimit für E-Mails, um nahtlose Erlebnisse für Exchange- und Gmail-Benutzer zu erstellen. Verringern oder eliminieren Sie die Verwendung von Massen-E-Mail-Sendeanwendungen von Drittanbietern.
* **Bounce-Tracking der E-Mail-Verbindung**: Erhalten Sie mit dem neuen E-Mail-Bounce-Bericht Einblicke in die Lead-Qualität und die Leistung von E-Mail-Vorlagen. Exchange- und Gmail-Benutzer können sich für den Empfang von Bounce-Benachrichtigungen entscheiden, die in den Live Feed, E-Mail-Ordner, Vorlagenanalysen und Campaign Analytics aggregiert werden.
* **Profilseitenkonfiguration**: Benutzereinstellungen auf der neuen Profilseite einfach verwalten. Ändern Sie das Kennwort, bearbeiten Sie die Geolocation- und Spracheinstellungen und überprüfen Sie den Integrationsstatus an einer Stelle.
* **Vorlagenverwaltung**: Organisieren Sie E-Mail-Vorlagen für Verkäufe in Kategorien mit einer neuen Drag &amp; Drop-Funktion, um einen schnellen Zugriff auf relevante Vorlagen zu gewährleisten und die Suchzeit zu verkürzen.
* **Aktualisierungen des Benutzererlebnisses für Sales Connect**: Passen Sie das Rasterlayout für Sales Connect an, indem Sie die Größe der Spalten ändern und neu anordnen. Ihre Anzeigevoreinstellungen werden automatisch gespeichert.

**_Mitteilungen und veraltete Elemente_**

* Alle Benutzer müssen auf die neueste Version von Sales Insight aktualisieren **vor dem 15. Januar 2021**. Wenn Sie das Upgrade nicht abgeschlossen haben, werden Sie nach der Anmeldung bei der Anwendung dazu aufgefordert. Befolgen Sie die Anweisungen [in diesem Handbuch](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md). Die aktualisierte Version enthält einen Patch für eine identifizierte Sicherheitslücke. Der Patch wurde ursprünglich am 6. April 2016 veröffentlicht. Hinweis: **Versionen 1.4363 oder höher** keine Aktualisierung durchführen müssen.
* Die Einstellung des Forms 1.0-Dienstes wird in Kraft treten in **Mai 2021** verfügbar. Der Forms 1.0-Dienst wird vollständig eingestellt, sodass alle verbleibenden Forms 1.0-Assets, die noch verwendet werden, nicht mehr funktionsfähig sind. Darüber hinaus werden Formularübermittlungen, die über nicht unterstützte Methoden durchgeführt werden, wie z. B. programmatische Formular-POSTs an die Endpunkte leadCapture/save und leadCapture/save2, abgelehnt. Weitere Informationen und die Sanierung finden Sie unter [unserem Beitrag in der Marketingnation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-the-Marketo-Engage-Form-Platform/ta-p/306631).
* 2021 wird Marketo Engage Änderungen an der URL-Struktur für Landingpages, Formulare, Bilder und Dateien vornehmen. Für bestehende Marketo Engage-Abonnements werden wir am 1. April 2021 mit der schrittweisen Einführung beginnen. Weitere Informationen zur Rollout-Timeline werden im März 2021 veröffentlicht. Weitere Informationen zur Änderung der betroffenen Asset-Typen finden Sie unter [unserem Beitrag in der Marketingnation](https://nation.marketo.com/t5/Product-Documents/Upcoming-Changes-to-Design-Studio-URLs/ta-p/306632).

**_Webinar zur Produktversion_**

Möchten Sie mehr über diese Funktionen und Verbesserungen erfahren? Stellen Sie sicher, [registrieren](https://engage.marketo.com/January_21_Release_Webinar_Registration.html) um am 21. Januar um 13:00 Uhr PT / 16:00 Uhr ET zu einem Live-Webinar mit unserem Produktteam zu kommen, um einen tieferen Einblick in diese Innovationen zu erhalten.
