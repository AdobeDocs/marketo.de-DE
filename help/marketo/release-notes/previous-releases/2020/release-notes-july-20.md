---
unique-page-id: 45416698
description: Versionshinweise - 20. Juli - Marketo-Dokumente - Produktdokumentation
title: Versionshinweise - Juli '20
exl-id: 3c9b1f1d-961c-4bf8-8b99-37b483230506
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 2%

---

# Versionshinweise – Juli 2020 {#release-notes-july}

Die folgenden Funktionen sind in der Version vom Juli 2020 enthalten. Überprüfen Sie Ihre Marketo Edition auf die Verfügbarkeit der Funktionen.

>[!AVAILABILITY]
>
>Bitte beachten Sie, dass je nach aktuellem Paket für Artikel mit einem Stern ( ![(Stern)](assets/yellow-star.png) der Kauf eines Mehrwert-Add-ons erforderlich sein kann. Weitere Informationen erhalten Sie vom Marketo Engage-Support.

**_Vierteljährliche Versionen_** Die folgenden Funktionen werden am 31. **2020 veröffentlicht**.

## Administration {#administration}

* **[Export „Verwendet von“ in der](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)**: Administratoren können jetzt alle Asset-Links „Verwendet von“ für ein ausgewähltes Feld in eine CSV-Datei exportieren. Diese Verbesserung kann sowohl Admins als auch Nicht-Admins beim Bereinigen nicht verwendeter Felder unterstützen. Darüber hinaus können Assets jetzt in einer neuen Browser-Registerkarte oder in einem neuen Fenster geöffnet werden.

## Kundenbezogenes Marketing {#account-based-marketing}

![(Stern)](assets/yellow-star.png)

* **Aktualisierte Benutzeroberfläche für die Kontoprofilerstellung**: Vereinfachen Sie die Erstellung Ihrer Zielkontenliste in der Kontoprofilerstellung mit optimierten Schritten, die alle in einem einzigen Bildschirm angezeigt werden.

<br> 

**_Veröffentlichung im gesamten Quartal_**

Die folgenden Funktionen befinden sich in einem nicht vierteljährlichen Zyklus und werden in den kommenden Monaten veröffentlicht.

* **Forms-Service**: Wir führen eine strengere Validierung der Formularfeldsyntax ein und die Möglichkeit, gängige Bot-Muster mit neuen Funktionen für gesicherte Domains für Landingpages zu blockieren. Das Blockieren von Bot-Mustern kann die Übermittlung von Spam-Formularen reduzieren und die Qualität Ihrer Datenbank verbessern.

>[!NOTE]
>
>Der vollständige Rollout der erweiterten Validierung der Formularfeldsyntax wurde auf die Zeit nach unserer Version vom Januar 2021 verschoben.

* **Erhöhte Größenbeschränkung für Asset-API-URI**: Die Größenbeschränkung für den Uniform Resource Identifier (URI) wird von 8 KB auf 65 KB erhöht, bevor der Parameter „_method“ entfernt wird. Bei der Durchführung langer Abfragezeichenfolgen ermöglicht diese Größenbeschränkung eine einfachere Weitergabe der Daten. Das Entfernen des Parameters „_method“ ist Teil eines bevorstehenden Sicherheits-Upgrades.

## [!DNL Sales Insight] {#sales-insight}

![(Stern)](assets/yellow-star.png)

* **[[!DNL Sales Insight] Für Kunden mit nicht-nativer CRM [!DNL Salesforce] Integration](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md) (Beta)**: Marketo Engage-Kunden mit nicht-nativen [!DNL Salesforce] CRM-Integrationen können jetzt [!DNL Sales Insight] verwenden, um ihren Vertriebsteams zu helfen, die aktivsten Leads und Chancen zu verstehen, zu priorisieren und mit ihnen zu interagieren, um intelligentes Verkaufen und schnellere Angebote zu ermöglichen.

## [!DNL Sales Connect] {#sales-connect}

![(Stern)](assets/yellow-star.png)

* **[Verbessertes Einverständnis von zwei Parteien für Verkaufsanrufe:](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)** Administratoren haben jetzt mehr Kontrolle über Konfigurationen zur Anrufaufzeichnung. [Anrufaufzeichnungen aktivieren](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md) mit der Gewissheit, dass Sie das Einverständnisgesetz von zwei Parteien einhalten. Automatisieren Sie die Benachrichtigung über den aufgezeichneten Anruf und aktivieren Sie Audioclips, die vor dem Anruf abgespielt werden sollen.

<br> 

## Ankündigungen und Veraltungen {#announcements-deprecations}

* **Entfernen von Asset-API-Parametern „_method“**: Nach September 2020 akzeptieren Asset-API-Endpunkte keine „_method“ mehr zum Übergeben von Abfrageparametern in einem POST-Text, um URI-Längenbeschränkungen zu umgehen. Um Anfragen nachzukommen, für die dieser Parameter erforderlich ist, werden die URI-Beschränkungen für Asset-APIs von 8 KB auf 65 KB erhöht.
* **[[!DNL Munchkin] Lead verknüpfen](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**: Mit dieser Version des Munchkin JavaScript-Clients, Version 159, werden wir die [!DNL Munchkin] Associate-Lead-Methode einstellen. Wenn aufgerufen wird, erhalten Sie einen Warnhinweis, dass die Methode in einer zukünftigen Version entfernt wird. Nach dem Entfernen ist die Methode nicht mehr funktionsfähig und Versuche, sie zu verwenden, schlagen fehl. Marketo Engage-Kunden, die diese Methode kürzlich verwendet haben, werden einzeln über ihre Verwendung benachrichtigt.
* **Unterstützung für Internet Explorer**: Wie bereits angekündigt, endet die Marketo Engage-Unterstützung für Internet Explorer 11 am **. Juli 2020**. Wir werden [!DNL Google Chrome], [!DNL Mozilla Firefox], [!DNL  Apple Safari] und [!DNL Microsoft Edge] weiterhin unterstützen.
* **Sky Default Experience**: Die Option für Administratoren oder Benutzer, [!DNL Marketo Sky] als Standarderlebnis festzulegen, wird in dieser Version entfernt, um eine Aktualisierung des primären Benutzererlebnisses vorzubereiten. Weitere Informationen zur Aktualisierung des primären Erlebnisses, die für später in diesem Jahr geplant ist, werden im Juli verfügbar sein. Benutzer, die [!DNL Marketo Sky] als Standarderlebnis festgelegt haben oder Zugriff auf [!DNL Marketo Sky] erhalten haben, können weiterhin über eine Kachel auf der Startseite von My Marketo auf [!DNL Marketo Sky] zugreifen.
* **EdgeHTML (nicht-Chromium) [!DNL Microsoft Edge] Unterstützung**: Marketo Engage wird Ende 2020 keine EdgeHTML-Versionen von Microsoft Edge mehr unterstützen. Ab dem 1. Januar 2021 unterstützen wir nur die neueste Chromium-Version von Microsoft Edge.
