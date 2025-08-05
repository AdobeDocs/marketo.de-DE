---
description: August 2021 - Marketo-Dokumentation - Produktdokumentation
title: August 2021 - Versionshinweise
exl-id: 4aec4e0b-520e-4786-a110-8e68f1bf9950
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '903'
ht-degree: 0%

---

# August 2021 - Versionshinweise {#release-notes-aug-21}

Die folgenden Funktionen sind in der Version vom 21. August enthalten. Überprüfen Sie Ihre Marketo Engage Edition auf die Verfügbarkeit der Funktionen.

>[!AVAILABILITY]
>
>Mit einem Stern (![](assets/yellow-star.png)) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie vom Adobe Marketo Engage-Support.

**_Quartalsveröffentlichungen_**

Die folgenden Funktionen werden am (**. August 2021)**.

## Experience Automation {#experience-automation}

* **Marketo Engage-Benutzerauthentifizierung über Adobe Identity**: In Kürze werden neue Marketo Engage-Benutzende mit Enterprise-Paketen mit Adobe ID-Benutzeranmeldeinformationen integriert. Die Migration aktueller Nutzer zum integrierten Identitätssystem wird erst Mitte 2022 erfolgen und bis auf Weiteres sind keine Maßnahmen erforderlich. Mit der Benutzerauthentifizierung für Adobe-Identitäten können IT-/Sicherheitsadministratoren mehrere Marketo Engage-Produktinstanzen zusammen mit anderen Experience Cloud-Lösungen verwalten und SSO über eine gemeinsame Konsole konfigurieren. Administratoren können Benutzergruppen und Benutzerberechtigungen bequem an einem Ort verwalten.

* **Schachtelung ausführbarer Kampagnen**: Ausführbare Kampagnen können jetzt auch andere ausführbare Kampagnen aufrufen, sodass Sie sie bis zu drei Ebenen tief verschachteln können. Dies ermöglicht eine weitere Konsolidierung gängiger Betriebsabläufe und verbessert das Management intelligenter Kampagnen.

* **Einzelne Flussaktion auf der Seite „Personendetails“** (verfügbar ab 9. September): Führen Sie Flussaktionen wie das Senden von E-Mail, das Ändern des Personenbesitzers oder andere intelligente Kampagnenaktionen für einzelne Personen auf der Seite „Personendetails“ mithilfe des Menüs „Flussaktion“ aus, ohne zur Datenbankrasteransicht zu wechseln.

* **[Export benutzerdefinierter Aktivitäten](/help/marketo/product-docs/administration/marketo-custom-activities/custom-activity-metadata-export.md)**: Der Metadatenexport unterstützt jetzt alle Objekte und entsprechenden Metadaten, die zum Freigeben, Analysieren und Entwerfen Ihres Abonnementdatenmodells verwendet werden können.

## API-Verbesserungen {#api-enhancements}

* **Formular-API übermitteln**: Wenn eine E-Mail-Adresse in zwei oder mehr Lead-Datensätzen dupliziert ist, aktualisieren wir den Datensatz „Zuletzt aktualisiert“, anstatt ihn vollständig zu überspringen. Parität mit der Forms 2.0-API.

* **E-Mail-API**: Abrufen von E-Mail-Assets von Champions oder Challengern. Abrufen von E-Mail-Assets mit dem Datumsbereichsfilter.

**_Veröffentlichung im gesamten Quartal_**

Die folgenden Funktionen befinden sich in einem nicht vierteljährlichen Zyklus und werden in den kommenden Monaten veröffentlicht.

## [!DNL Sales Insight] {#sales-insight}

![(Stern)](assets/yellow-star.png)

* **Verbesserte Transparenz der Lead-, Kontakt-, Account- und Opportunity-Aktivitäten für Salesforce CRM-**: Die Interaktion mit potenziellen Kunden während langer Verkaufszyklen ist aufgrund der gestiegenen Anzahl von Interaktionsdatensätzen in [!DNL Sales Insight] besser informiert. Die Registerkarten „Interessante Momente“, „Web-Aktivität“, „E-Mail“ und „Bewertung“ zeigen bis zu 400 Aktivitäten für Lead-, Kontakt-, Konto- und Opportunity-Objekte.

## [!DNL Sales Connect] {#sales-connect}

![(Stern)](assets/yellow-star.png)

* **Drosselung der E-Mail-Verbindung (Beta)**: Verbessern Sie die E-Mail-Zustellbarkeit und skalieren Sie die personalisierte Verkaufskommunikation mit der Drosselung der E-Mail-Verbindung für Sales Connect. Diese neue Technologie verwaltet automatisch das Timing des E-Mail-Versands, um [!DNL Exchange] und Gmail-Benutzern nahtlose Erlebnisse zu bieten. Verringern oder beseitigen Sie die Verwendung von Massenversand-Anwendungen von Drittanbietern und senden Sie alle Ihre E-Mails aus [!DNL Sales Connect] mit Sicherheit.

>[!NOTE]
>
>E-Mail-Einschränkungen sind jetzt in Beta verfügbar. [Weitere Informationen](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

* **Enhanced Sales Activity Insights**: Erfassen und aktivieren Sie personalisierte Interaktionen basierend auf den vorherigen Aktivitäten Ihres Sales-Teams. Neue Attribute wie „Link zur Aufzeichnung von Verkaufsanrufen“, „Name der Verkaufskampagne“ und „E-Mail-Betreff des Verkaufs“ können in Smart Lists von Marketo Engage verwendet werden.  Diese Aktivitäten können über die Marketo Engage-REST-API oder den Massenexport exportiert und gemeldet werden und stehen als zusätzliche Einschränkung für Smart Lists für Filter und Trigger zur Verfügung.

## [!DNL Bizible] {#bizible}

![](assets/yellow-star.png)

* **[!DNL Bizible][!DNL LinkedIn] Integration von Lead Gen-Forms**: Marketing-Experten können jetzt Umsatzzuordnungen für Konversionen durchführen, die auftreten, wenn [!DNL LinkedIn] Formularausfüllungen über ihre Lead Gen-Forms-Werbeeinheiten erfasst. Diese Erkenntnisse können dann zur Optimierung der Formularleistung und der Investitionen in bezahlte Medien verwendet werden. [!DNL LinkedIn] Lead Gen Forms sind eines der am schnellsten wachsenden Paid-Media-Angebote von [!DNL LinkedIn] und diese neue Funktion ist Teil unserer bestehenden [!DNL LinkedIn] Ads-Integration mit [!DNL Bizible].

* **Verbessertes Geschwindigkeits-Dashboard**: Wir haben eine neue Geschwindigkeitsmetrik und einen Dashboard-Filter für tiefere Einblicke hinzugefügt. Dieses Dashboard wird von Marketing-Experten verwendet, um die Lead- und Opportunity-Geschwindigkeit und die Effizienz verschiedener Formen der Marketing- und Vertriebsinteraktion Schritt für Schritt zu verstehen.

* **Neues Journey-Dashboard für Kohorten-Wasserfälle**: Auf diese Weise können Marketing-Fachleute den Fortschritt einer ausgewählten Kohorte anhand eines klassischen Sets aus „Demand Waterfall“-Stadien anzeigen und so ein schnelles Verständnis der Konversionsraten und der impliziten Kausalität der Staging-Konversion auf Staging-Basis erhalten.

## Integration von [!DNL Bizible] mit Adobe Experience Cloud {#bizible-integration-with-adobe-experience-cloud}

Dieser Abschnitt enthält neue Funktionen für Bizible-Benutzer, die die Migration zum Adobe Identity Management System (IMS) abgeschlossen haben. Wenn Sie migriert wurden, sehen Sie Ihre neue Adobe ID in [!DNL Bizible] Einstellungen auf der Registerkarte Adobe ID . Alle Konten sollten bis Ende 2021 migriert werden.

* **[!DNL Bizible]Integration mit Adobe Privacy Service** (verfügbar ab September 2021): Durch die Integration von [!DNL Bizible] mit Adobe Privacy Service wird die Einhaltung wichtiger Datenschutzbestimmungen (wie der DSGVO) in allen Adobe Experience Cloud-Anwendungen zentralisiert. Sie können jetzt diesen Service nutzen und alle Datenschutzanfragen zentral verwalten, sodass Änderungsanfragen, die in [!DNL Bizible] und andere Adobe-Produkte eingehen, programmübergreifend berücksichtigt werden.

* **[!DNL Bizible]auf Adobe Unified Shell**: Die Einführung von Adobe Unified Shell in [!DNL Bizible] bietet Benutzenden neue Funktionen, die in der Kopfzeilenleiste der [!DNL Bizible] Anwendung angezeigt werden, und besseren Zugriff auf Support-Ressourcen und Programmwechsel. Mit Adobe Unified Shell können Sie ein konsistentes Erlebnis zwischen [!DNL Bizible] und anderen Adobe Experience Cloud-Programmen schaffen.

* **[!DNL Bizible]Domain-Eigentümerschaft und Selbstverwaltung**: [!DNL Bizible] können Adobe Admin Console nutzen, um die Domains zu verwalten, die verfolgt werden [!DNL Bizible]. Dies bringt den Self-Service in einen zuvor manuellen Prozess und bietet ein konsistentes Erlebnis bei der Verwaltung von Domain-Eigentümerschaft und -Tracking in allen Adobe Experience Cloud-Programmen.

## Ankündigungen {#announcements}

* **Aktualisierung der Einstellungen für universelle Abonnement-ID**: Um die bevorstehende Integration von Marketo Engage und Adobe Identity für bestehende Benutzende zu unterstützen, werden alle Marketo Engage-Abonnements durch die Aktivierung der universellen ID-Unterstützung vereinheitlicht. Weitere Informationen [finden Sie hier](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md).

**_Webinar zur Produktversion_**

[Webinar zur Marketo Engage-Version August 2021](https://engage.marketo.com/August21_Release_Webinar.html)
