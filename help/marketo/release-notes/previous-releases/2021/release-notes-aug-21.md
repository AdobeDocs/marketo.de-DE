---
description: Versionshinweise - August 2021 - Marketo-Dokumente - Produktdokumentation
title: August 2021 - Versionshinweise
exl-id: 4aec4e0b-520e-4786-a110-8e68f1bf9950
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '932'
ht-degree: 0%

---

# August 2021 - Versionshinweise {#release-notes-aug-21}

Die folgenden Funktionen sind in der Version vom 21. August enthalten. Überprüfen Sie Ihre Marketo Engage-Edition auf Verfügbarkeit der Funktionen.

>[!AVAILABILITY]
>
>Mit einem Stern (![](assets/yellow-star.png)) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie von Ihrem Adobe Marketo Engage-Support-Mitarbeiter.

**_Vierteljährliche Versionen_**

Die folgenden Funktionen werden am **20. August 2021** veröffentlicht.

## Erlebnisautomatisierung {#experience-automation}

* **Marketo Engage Benutzerauthentifizierung über Adobe Identity**: Bald werden neue Marketo Engage-Benutzer mit Enterprise-Paketen mit Adobe ID-Benutzeranmeldeinformationen integriert. Die Migration der aktuellen Benutzer zum integrierten Identitätssystem erfolgt erst Mitte 2022 und es sind keine Maßnahmen erforderlich, bis weitere Informationen verfügbar sind. Die Authentifizierung von Adobe Identity-Benutzern ermöglicht IT-/Security-Administratoren die Verwaltung mehrerer Marketo Engage-Produktinstanzen zusammen mit anderen Experience Cloud-Lösungen sowie die Konfiguration von SSO über eine gemeinsame Konsole. Administratoren können Benutzergruppen und Benutzerberechtigungen bequem an einem Ort verwalten.

* **Ausführbare Kampagnennistrierung**: Ausführbare Kampagnen können jetzt auch andere ausführbare Kampagnen aufrufen, sodass Sie sie bis zu drei Ebenen tief verschachteln können. Dies ermöglicht die weitere Konsolidierung gemeinsamer Betriebsabläufe und verbessert die Verwaltung intelligenter Kampagnen.

* **EinzelFluss-Aktion auf der Seite &quot;Personendetails&quot;** (Bis zum 9. September verfügbar): Führen Sie über das Flussaktionsmenü Flüsse aus, z. B. das Senden von E-Mails, das Ändern des Eigentümers einer Person oder andere intelligente Kampagnenaktionen für einzelne Personen. Wechseln Sie dazu nicht zur Datenbankrasteransicht.

* **[Export benutzerdefinierter Aktivitäten](/help/marketo/product-docs/administration/marketo-custom-activities/custom-activity-metadata-export.md)**: Der Metadatenexport unterstützt jetzt alle Objekte und entsprechenden Metadaten, die zum Freigeben, Analysieren und Entwerfen Ihres Abonnementdatenmodells verwendet werden können.

## API-Verbesserungen {#api-enhancements}

* **Formular-API übermitteln**: Wenn eine E-Mail-Adresse in zwei oder mehr Lead-Datensätzen dupliziert wird, wird der &quot;letzte aktualisierte&quot;Datensatz aktualisiert, anstatt ihn vollständig zu überspringen. Entspricht der Forms 2.0-API.

* **E-Mail-API**: Rufen Sie die E-Mail-Assets des Gewinners oder Herausforderers ab. Abrufen von E-Mail-Assets mithilfe des Datumsbereichfilters.

**_Herausgabe während des gesamten Quartals_**

Die folgenden Funktionen befinden sich in einem nicht vierteljährlichen Zyklus und werden in den kommenden Monaten veröffentlicht.

## Sales Insight {#sales-insight}

![(star)](assets/yellow-star.png)

* **Verbesserte Sichtbarkeit der Lead-, Kontakt-, Konto- und Opportunity-Aktivitäten für Salesforce CRM-Benutzer**: Die Interaktion mit Interessenten während langer Verkaufszyklen ist aufgrund einer erhöhten Anzahl von Interaktionsdatensätzen in Sales Insight besser informiert. Interessante Momente, Web-Aktivitäten, E-Mails und Punktzahlen zeigen bis zu 400 Aktivitäten in Lead-, Kontakt-, Konto- und Opportunity-Objekten.

## Sales Connect {#sales-connect}

![(star)](assets/yellow-star.png)

* **Einschränken der E-Mail-Verbindung (Beta)**: Verbessern Sie die E-Mail-Zustellbarkeit und skalieren Sie die personalisierte Verkaufskommunikation mit der E-Mail-Verbindungsbegrenzung für Sales Connect. Diese neue Technologie verwaltet automatisch den Zeitpunkt des E-Mail-Versands, um nahtlose Erlebnisse für Exchange- und Gmail-Benutzer zu erstellen. Verringern oder eliminieren Sie die Verwendung von Massen-E-Mail-Sendeanwendungen von Drittanbietern und senden Sie alle E-Mails von Sales Connect sicher.

>[!NOTE]
>
>E-Mail-Einschränkungen sind jetzt in Beta verfügbar. [Weitere Infos](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

* **Verbesserte Einblicke in die Verkaufsaktivität**: Erfassen und aktivieren Sie personalisierte Interaktionen, die auf den vorherigen Aktivitäten Ihres Verkaufsteams basieren. Neue Attribute wie Link zur Aufzeichnung von Verkaufsaufrufen, Name der Verkaufskampagne und E-Mail-Betreff für Vertrieb können in Marketo Engage-Smart-Listen verwendet werden.  Diese Aktivitäten können über die Marketo Engage REST-API oder den Massenexport exportiert und gemeldet werden und sind in Filtern und Triggern als zusätzliche Einschränkungen für Smart-Listen verfügbar.

## Bizible {#bizible}

![](assets/yellow-star.png)

* **Bizible LinkedIn Lead Gen Forms Integration**: Marketingexperten können jetzt Umsätze für Umrechnungen zuordnen, die auftreten, wenn LinkedIn Formulare über die Lead Gen Forms-Anzeigeneinheiten erfasst. Diese Einblicke können dann zur Optimierung der Formularleistung und der Investitionen in gebührenpflichtige Medien verwendet werden. LinkedIn Lead Gen Forms gehört zu den am schnellsten wachsenden Paid Media-Angeboten von LinkedIn. Diese neue Funktion ist Bestandteil unserer bestehenden LinkedIn Ads-Integration mit Bizible.

* **Verbessertes Velocity-Dashboard**: Wir haben eine neue Velocity-Metrik und einen Dashboard-Filter hinzugefügt, um tiefere Einblicke zu erhalten. Dieses Dashboard wird von Marketingexperten verwendet, um die Lead- und Opportunitätsgeschwindigkeit einzelner Phasen sowie die Effizienz verschiedener Formen der Marketing- und Verkaufsinteraktion zu verstehen.

* **Neues Journey-Dashboard für Kohortenwasserfälle**: Marketingexperten können damit den Verlauf einer ausgewählten Kohorte anhand eines klassischen Sets von &quot;Wasserfällen nach Bedarf&quot;anzeigen, was ein schnelles Verständnis der Konversionsraten und der impliziten Staging-Konversionskausalität auf einer Staging-Ebene ermöglicht.

## Bizible-Integration mit Adobe Experience Cloud {#bizible-integration-with-adobe-experience-cloud}

Dieser Abschnitt enthält neue Funktionen für Bizible-Benutzer, die die Migration des Adobe Identity Management-Systems (IMS) abgeschlossen haben. Wenn Sie migriert wurden, finden Sie Ihre neue Adobe ID in den Bizible-Einstellungen auf der Registerkarte Adobe ID . Alle Konten sollten bis Ende 2021 migriert werden.

* **Bizible-Integration mit Adobe Privacy Service** (verfügbar im September 2021): Durch die Integration von Bizible in den Adobe-Privacy Service wird die Einhaltung wichtiger Datenschutzbestimmungen (wie DSGVO) in allen Adobe Experience Cloud-Anwendungen zentralisiert. Sie können diesen Dienst jetzt nutzen und alle Datenschutzanfragen zentral verwalten, sodass sich Änderungsanfragen, die in Bizible und andere Adobe-Produkte eingehen, in allen Anwendungen widerspiegeln.

* **Bizible on Adobe Experience Cloud Interface**: Bizible bietet durch die Übernahme der Adobe Experience Cloud-Benutzeroberfläche neue Funktionen, die in der Bizible-Anwendungs-Header-Leiste angezeigt werden. Bizible bietet besseren Zugriff auf Support-Ressourcen und den Anwendungsumschalter. Die Experience Cloud-Oberfläche hilft bei der Erstellung eines konsistenten Erlebnisses zwischen Bizible und anderen Adobe Experience Cloud-Anwendungen.

* **Bizible Domain Ownership and Self-Management**: Bizible Benutzer können Adobe Admin Console nutzen, um die Domänen zu verwalten, die von Bizible verfolgt werden sollen. Dadurch wird der Self-Service zu einem zuvor manuellen Prozess und die Verwaltung von Domain-Besitz und -Tracking in allen Adobe Experience Cloud-Anwendungen einheitlich gestaltet.

## Ankündigungen {#announcements}

* **Aktualisierung der universellen ID-Einstellungen für Abonnements**: Um die bevorstehende Marketo Engage- und Adobe-Identitätsintegration für bestehende Benutzer zu unterstützen, werden alle Marketo Engage-Abonnements bei der Aktivierung der Universellen ID-Unterstützung vereinheitlicht. Weitere Informationen [finden Sie hier](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md).

**_Webinar zur Produktversion_**

[Marketo Engage-Release-Webinar vom August 2021](https://engage.marketo.com/August21_Release_Webinar.html)
