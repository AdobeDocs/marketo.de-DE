---
description: August 2021 - Marketo-Dokumentation - Produktdokumentation
title: August 2021 - Versionshinweise
exl-id: 4aec4e0b-520e-4786-a110-8e68f1bf9950
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '932'
ht-degree: 1%

---

# August 2021 - Versionshinweise {#release-notes-aug-21}

Die folgenden Funktionen sind in der Version vom 21. August enthalten. Überprüfen Sie Ihre Marketo Engage-Edition auf Funktionsverfügbarkeit.

>[!AVAILABILITY]
>
>Mit einem Stern (![](assets/yellow-star.png)) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie vom Adobe Marketo Engage-Support.

**_Quartalsveröffentlichungen_**

Die folgenden Funktionen werden am (**. August 2021)**.

## Experience Automation {#experience-automation}

* **Marketo Engage-Benutzerauthentifizierung über Adobe-Identität**: In Kürze werden neue Marketo Engage-Benutzer mit Enterprise-Paketen mit Adobe ID-Benutzeranmeldeinformationen integriert. Die Migration aktueller Nutzer zum integrierten Identitätssystem wird erst Mitte 2022 erfolgen und bis auf Weiteres sind keine Maßnahmen erforderlich. Die Adobe-Identitäts-Benutzerauthentifizierung ermöglicht es IT-/Sicherheitsadministratoren, mehrere Marketo Engage-Produktinstanzen zusammen mit anderen Experience Cloud-Lösungen zu verwalten und SSO über eine gemeinsame Konsole zu konfigurieren. Administratoren können Benutzergruppen und Benutzerberechtigungen bequem an einem Ort verwalten.

* **Schachtelung ausführbarer Kampagnen**: Ausführbare Kampagnen können jetzt auch andere ausführbare Kampagnen aufrufen, sodass Sie sie bis zu drei Ebenen tief verschachteln können. Dies ermöglicht eine weitere Konsolidierung gängiger Betriebsabläufe und verbessert das Management intelligenter Kampagnen.

* **Einzelne Flussaktion auf der Seite „Personendetails“** (verfügbar ab 9. September): Führen Sie Flussaktionen wie das Senden von E-Mail, das Ändern des Personenbesitzers oder andere intelligente Kampagnenaktionen für einzelne Personen auf der Seite „Personendetails“ mithilfe des Menüs „Flussaktion“ aus, ohne zur Datenbankrasteransicht zu wechseln.

* **[Export benutzerdefinierter Aktivitäten](/help/marketo/product-docs/administration/marketo-custom-activities/custom-activity-metadata-export.md)**: Der Metadatenexport unterstützt jetzt alle Objekte und entsprechenden Metadaten, die zum Freigeben, Analysieren und Entwerfen Ihres Abonnementdatenmodells verwendet werden können.

## API-Verbesserungen {#api-enhancements}

* **Formular-API übermitteln**: Wenn eine E-Mail-Adresse in zwei oder mehr Lead-Datensätzen dupliziert ist, aktualisieren wir den Datensatz „Zuletzt aktualisiert“, anstatt ihn vollständig zu überspringen. Parität mit der Forms 2.0-API.

* **E-Mail-API**: Abrufen von E-Mail-Assets von Champions oder Challengern. Abrufen von E-Mail-Assets mit dem Datumsbereichsfilter.

**_Veröffentlichung im gesamten Quartal_**

Die folgenden Funktionen befinden sich in einem nicht vierteljährlichen Zyklus und werden in den kommenden Monaten veröffentlicht.

## Sales Insight {#sales-insight}

![(Stern)](assets/yellow-star.png)

* **Verbesserte Sichtbarkeit von Lead-, Kontakt-, Account- und Opportunity-Aktivitäten für Salesforce CRM-Benutzer**: Die Interaktion mit potenziellen Kunden während langer Verkaufszyklen ist aufgrund der erhöhten Anzahl von Interaktionsdatensätzen in Sales Insight besser informiert. Die Registerkarten „Interessante Momente“, „Web-Aktivität“, „E-Mail“ und „Bewertung“ zeigen bis zu 400 Aktivitäten für Lead-, Kontakt-, Konto- und Opportunity-Objekte.

## Sales Connect {#sales-connect}

![(Stern)](assets/yellow-star.png)

* **Drosselung der E-Mail-Verbindung (Beta)**: Verbessern Sie die E-Mail-Zustellbarkeit und skalieren Sie die personalisierte Verkaufskommunikation mit der Drosselung der E-Mail-Verbindung für Sales Connect. Diese neue Technologie verwaltet automatisch das Timing des E-Mail-Versands, um Exchange- und Gmail-Benutzern nahtlose Erlebnisse zu bieten. Verringern oder beseitigen Sie die Verwendung von Massenversand-Anwendungen von Drittanbietern und senden Sie alle Ihre E-Mails vom Vertrieb Connect mit Sicherheit.

>[!NOTE]
>
>E-Mail-Einschränkungen sind jetzt in Beta verfügbar. [Weitere Informationen](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

* **Enhanced Sales Activity Insights**: Erfassen und aktivieren Sie personalisierte Interaktionen basierend auf den vorherigen Aktivitäten Ihres Vertriebsteams. Neue Attribute wie Sales Call Recording Link, Sales Campaign Name und Sales Email Subject können beim Marketo Engage von Smart Lists verwendet werden.  Diese Aktivitäten können über die Marketo Engage-REST-API oder den Massenexport exportiert und gemeldet werden und stehen als zusätzliche Einschränkung für Smart Lists für Filter und Trigger zur Verfügung.

## Bizible {#bizible}

![](assets/yellow-star.png)

* **Integration von Bizible LinkedIn Lead Gen mit Forms**: Marketing-Experten können jetzt Umsatzzuordnungen für Konversionen vornehmen, die auftreten, wenn LinkedIn Formularausfüllungen über ihre Lead Gen-Forms-Werbeeinheiten erfasst. Diese Erkenntnisse können dann zur Optimierung der Formularleistung und der Investitionen in bezahlte Medien verwendet werden. LinkedIn Lead Gen Forms ist eines der am schnellsten wachsenden Paid-Media-Angebote von LinkedIn und diese neue Funktion ist Teil unserer bestehenden LinkedIn Ads-Integration mit Bizible.

* **Verbessertes Geschwindigkeits-Dashboard**: Wir haben eine neue Geschwindigkeitsmetrik und einen Dashboard-Filter für tiefere Einblicke hinzugefügt. Dieses Dashboard wird von Marketing-Experten verwendet, um die Lead- und Opportunity-Geschwindigkeit und die Effizienz verschiedener Formen der Marketing- und Vertriebsinteraktion Schritt für Schritt zu verstehen.

* **Neues Journey-Dashboard für Kohorten-Wasserfälle**: Auf diese Weise können Marketing-Fachleute den Fortschritt einer ausgewählten Kohorte anhand eines klassischen Sets aus „Demand Waterfall“-Stadien anzeigen und so ein schnelles Verständnis der Konversionsraten und der impliziten Kausalität der Staging-Konversion auf Staging-Basis erhalten.

## Bizible-Integration mit Adobe Experience Cloud {#bizible-integration-with-adobe-experience-cloud}

Dieser Abschnitt enthält neue Funktionen für Bizible-Anwender, die ihre Migration zum Adobe Identity Management System (IMS) abgeschlossen haben. Wenn Sie migriert wurden, sehen Sie Ihre neue Adobe ID in den Bizible-Einstellungen auf der Registerkarte Adobe ID . Alle Konten sollten bis Ende 2021 migriert werden.

* **Bizible-Integration mit Adobe-Privacy Service** (verfügbar ab September 2021): Durch die Integration von Bizible mit dem Adobe-Privacy Service wird die Einhaltung wichtiger Datenschutzbestimmungen (wie der DSGVO) in allen Adobe Experience Cloud-Anwendungen zentralisiert. Sie können jetzt diesen Service nutzen und alle Datenschutzanfragen zentral verwalten, sodass Änderungsanfragen, die bei Bizible und anderen Adobe-Produkten eingehen, programmübergreifend berücksichtigt werden.

* **Bizible auf der Adobe Experience Cloud-Benutzeroberfläche**: Die Einführung der Adobe Experience Cloud-Benutzeroberfläche durch Bizible bietet Benutzenden neue Funktionen, die in der Kopfzeile der Bizible-Anwendung angezeigt werden und besseren Zugriff auf Support-Ressourcen und Programmwechsel beinhalten. Die Experience Cloud-Benutzeroberfläche hilft Ihnen, ein konsistentes Erlebnis zwischen Bizible und anderen Adobe Experience Cloud-Anwendungen zu schaffen.

* **Eigentümerschaft und Selbstverwaltung der Bizible-Domain**: Bizible-Benutzer können Adobe Admin Console nutzen, um die Domains zu verwalten, die Bizible nachverfolgen soll. Dies bringt den Self-Service in einen zuvor manuellen Prozess und bietet ein konsistentes Erlebnis bei der Verwaltung von Domain-Eigentümerschaft und -Tracking in allen Adobe Experience Cloud-Programmen.

## Ankündigungen {#announcements}

* **Aktualisierung der universellen ID-Abonnementeinstellungen**: Um die bevorstehende Marketo Engage- und Adobe-Identitätsintegration für bestehende Benutzende zu unterstützen, werden alle Marketo Engage-Abonnements durch die Aktivierung der universellen ID-Unterstützung vereinheitlicht. Weitere Informationen [finden Sie hier](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md).

**_Webinar zur Produktversion_**

[Webinar zur Marketo Engage-Version August 2021](https://engage.marketo.com/August21_Release_Webinar.html)
