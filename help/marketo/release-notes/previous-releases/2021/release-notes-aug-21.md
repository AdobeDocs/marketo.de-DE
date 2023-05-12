---
description: Versionshinweise - August 2021 - Marketo-Dokumente - Produktdokumentation
title: August 2021 - Versionshinweise
exl-id: 4aec4e0b-520e-4786-a110-8e68f1bf9950
source-git-commit: 7a062683a3c38d8765eb966041bf7ee3db665f5a
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 0%

---

# Versionshinweise: August 2021 {#release-notes-aug-21}

Die folgenden Funktionen sind in der Version vom 21. August enthalten. Überprüfen Sie Ihre Marketo Engage-Edition auf Funktionsverfügbarkeit.

>[!AVAILABILITY]
>
>Mit einem Stern gekennzeichnete Funktionen (![](assets/yellow-star.png)) sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie von Ihrem Adobe Marketo Engage-Support-Mitarbeiter.

**_Vierteljährliche Versionen_**

Die folgenden Funktionen werden veröffentlicht auf **20. August 2021**.

## Erlebnisautomatisierung {#experience-automation}

* **Marketo Engage-Benutzerauthentifizierung über Adobe Identity**: Bald werden neue Marketo Engage-Benutzer mit Enterprise-Paketen mit Adobe ID-Benutzeranmeldeinformationen integriert. Die Migration der aktuellen Benutzer zum integrierten Identitätssystem erfolgt erst Mitte 2022 und es sind keine Maßnahmen erforderlich, bis weitere Informationen verfügbar sind. Die Authentifizierung von Identitätsbenutzern ermöglicht es IT-/Sicherheitsadministratoren, mehrere Marketo Engage-Produktinstanzen zusammen mit anderen Experience Cloud-Lösungen zu verwalten und SSO über eine gemeinsame Konsole zu konfigurieren. Administratoren können Benutzergruppen und Benutzerberechtigungen bequem an einem Ort verwalten.

* **Ausführbare Kampagnenerfassung**: Ausführbare Kampagnen können jetzt auch andere ausführbare Kampagnen aufrufen, sodass Sie sie bis zu drei Ebenen tief verschachteln können. Dies ermöglicht die weitere Konsolidierung gemeinsamer Betriebsabläufe und verbessert die Verwaltung intelligenter Kampagnen.

* **EinzelFluss-Aktion auf der Seite &quot;Personendetails&quot;** (Bis 9. September verfügbar): Führen Sie über das Flussaktionsmenü auf der Detailseite der Person Flüsse aus, z. B. E-Mails senden, den Inhaber einer Person ändern oder andere Aktionen mit intelligenter Kampagne für einzelne Personen, ohne zur Datenbankraster-Ansicht zu wechseln.

* **[Export benutzerspezifischer Aktivitäten](/help/marketo/product-docs/administration/marketo-custom-activities/custom-activity-metadata-export.md)**: Der Metadatenexport unterstützt jetzt alle Objekte und entsprechenden Metadaten, die zum Freigeben, Analysieren und Entwerfen Ihres Abonnementdatenmodells verwendet werden können.

## API-Verbesserungen {#api-enhancements}

* **Submit Form API**: Wenn eine E-Mail-Adresse in zwei oder mehr Lead-Datensätze dupliziert wird, wird der Eintrag &quot;Zuletzt aktualisiert&quot;aktualisiert, anstatt dass er vollständig übersprungen wird. Entspricht der Forms 2.0-API.

* **Email-API**: Rufen Sie Meister- oder Herausforderer-E-Mail-Assets ab. Abrufen von E-Mail-Assets mithilfe des Datumsbereichfilters.

**_Veröffentlichung im gesamten Quartal_**

Die folgenden Funktionen befinden sich in einem nicht vierteljährlichen Zyklus und werden in den kommenden Monaten veröffentlicht.

## Sales Insight {#sales-insight}

![(Stern)](assets/yellow-star.png)

* **Verbesserte Sichtbarkeit von Lead-, Kontakt-, Konto- und Opportunity-Aktivitäten für Salesforce CRM-Benutzer**: Die Interaktion mit Interessenten während langer Verkaufszyklen ist aufgrund einer erhöhten Anzahl von Interaktionseinträgen in Sales Insight besser informiert. Interessante Momente, Web-Aktivitäten, E-Mails und Punktzahlen zeigen bis zu 400 Aktivitäten in Lead-, Kontakt-, Konto- und Opportunity-Objekten.

## SalesConnect {#sales-connect}

![(Stern)](assets/yellow-star.png)

* **Einschränken der E-Mail-Verbindung (Beta)**: Verbessern Sie die Zustellbarkeit von E-Mails und skalieren Sie die personalisierte Verkaufskommunikation mit der E-Mail-Verbindungsbegrenzung für Sales Connect. Diese neue Technologie verwaltet automatisch den Zeitpunkt des E-Mail-Versands, um nahtlose Erlebnisse für Exchange- und Gmail-Benutzer zu erstellen. Verringern oder eliminieren Sie die Verwendung von Massen-E-Mail-Sendeanwendungen von Drittanbietern und senden Sie alle E-Mails von Sales Connect sicher.

>[!NOTE]
>
>E-Mail-Einschränkungen sind jetzt in der Beta-Version verfügbar. [Weitere Informationen](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

* **Verbesserte Einblicke in die Verkaufsaktivität**: Erfassen und aktivieren Sie die personalisierte Interaktion basierend auf den früheren Aktivitäten Ihres Verkaufsteams. In Marketo Engage-Smart-Listen können neue Attribute wie &quot;Link zur Aufzeichnung von Verkaufsaufrufen&quot;, &quot;Name der Verkaufskampagne&quot;und &quot;E-Mail-Betreff&quot;verwendet werden.  Diese Aktivitäten können über die Marketo Engage-REST-API oder den Massenexport exportiert werden und sind in Filtern und Triggern als zusätzliche Einschränkungen für Smart-Listen verfügbar.

## Bizible {#bizible}

![](assets/yellow-star.png)

* **Bizible LinkedIn Lead Gen Forms Integration**: Marketingexperten können jetzt Umsätze für Konversionen zuordnen, die auftreten, wenn LinkedIn Formulare über die Lead Gen Forms-Anzeigeneinheiten erfasst. Diese Einblicke können dann zur Optimierung der Formularleistung und der Investitionen in gebührenpflichtige Medien verwendet werden. linkedIn Lead Gen Forms gehört zu den am schnellsten wachsenden Paid Media-Angeboten von LinkedIn. Diese neue Funktion ist Bestandteil unserer bestehenden LinkedIn Ads-Integration mit Bizible.

* **Verbessertes Velocity-Dashboard**: Wir haben eine neue Geschwindigkeitsmetrik und einen Dashboard-Filter hinzugefügt, um tiefere Einblicke zu erhalten. Dieses Dashboard wird von Marketingexperten verwendet, um die Lead- und Opportunitätsgeschwindigkeit einzelner Phasen sowie die Effizienz verschiedener Formen der Marketing- und Verkaufsinteraktion zu verstehen.

* **Neues Journey-Dashboard für Kohortenwasserfälle**: Auf diese Weise können Marketing-Experten den Fortschritt einer ausgewählten Kohorte anhand eines klassischen &quot;Demand-Wasserfall&quot;-Sets aus Phasen anzeigen, um ein schnelles Verständnis der Konversionsraten und der impliziten Staging-Konversionskausalität auf einer Staging-Ebene zu ermöglichen.

## Bizible-Integration mit Adobe Experience Cloud {#bizible-integration-with-adobe-experience-cloud}

Dieser Abschnitt enthält neue Funktionen für Bizible-Benutzer, die die Migration des Identity Management-Systems (IMS) für die Adobe abgeschlossen haben. Wenn Sie migriert wurden, finden Sie Ihre neue Adobe ID in den Bizible-Einstellungen auf der Registerkarte Adobe ID . Alle Konten sollten bis Ende 2021 migriert werden.

* **Bizible-Integration mit Adobe Privacy Service** (verfügbar im September 2021): Durch die Integration von Bizible in den Adobe Privacy Service wird die Einhaltung wichtiger Datenschutzbestimmungen (wie DSGVO) in allen Adobe Experience Cloud-Applikationen zentralisiert. Sie können diesen Dienst jetzt nutzen und alle Datenschutzanfragen zentral verwalten, sodass sich Änderungsanfragen, die in Bizible und andere Adobe-Produkte eingehen, in allen Anwendungen widerspiegeln.

* **Bizible auf der Adobe Experience Cloud-Benutzeroberfläche**: Durch die Übernahme der Adobe Experience Cloud-Benutzeroberfläche durch Bizible erhalten Benutzer neue Funktionen, die in der Bizible-Anwendungs-Kopfzeilenleiste angezeigt werden. Dazu gehört auch ein besserer Zugriff auf Supportressourcen und das Wechseln von Anwendungen. Die Experience Cloud-Oberfläche hilft bei der Erstellung eines konsistenten Erlebnisses zwischen Bizible und anderen Adobe Experience Cloud-Anwendungen.

* **Bizible Domain Ownership und Self-Management**: Bizible-Benutzer können Adobe Admin Console nutzen, um die Domänen zu verwalten, die Bizible verfolgen soll. Dadurch wird der Self-Service zu einem zuvor manuellen Prozess und die Verwaltung von Domain-Besitz und -Tracking in allen Adobe Experience Cloud-Anwendungen einheitlich gestaltet.

## Ankündigungen {#announcements}

* **Aktualisierung der Einstellungen für die universelle ID eines Abonnements**: Um die bevorstehende Integration von Marketo Engage- und Adobe-Identitäten für bestehende Benutzer zu unterstützen, werden alle Marketo Engage-Abonnements bei der Aktivierung der Universellen ID-Unterstützung vereinheitlicht. Weitere Informationen [finden Sie hier .](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md).

**_Webinar zur Produktversion_**

[Webinar zur Marketo Engage-Version August 2021](https://engage.marketo.com/August21_Release_Webinar.html)
