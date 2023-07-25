---
unique-page-id: 45416698
description: Versionshinweise - 20. Juli - Marketo-Dokumente - Produktdokumentation
title: Juli 2020 - Versionshinweise
exl-id: 3c9b1f1d-961c-4bf8-8b99-37b483230506
feature: Release Information
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 1%

---

# Versionshinweise: Juli &#39;20 {#release-notes-july}

Die folgenden Funktionen sind in der Version vom 20. Juli enthalten. Überprüfen Sie Ihre Marketo-Edition auf Funktionsverfügbarkeit.

>[!AVAILABILITY]
>
>Beachten Sie, dass je nach aktuellem Package Elemente mit einem Stern ( ![(Stern)](assets/yellow-star.png)) kann den Kauf eines Wertzusatzes erfordern. Weitere Informationen erhalten Sie von Ihrem Marketo Engage-Support-Mitarbeiter.

**_Vierteljährliche Versionen_** Die folgenden Funktionen werden veröffentlicht auf **31. Juli 2020**.

## Administration {#administration}

* **[Export in Feldverwaltung &quot;Verwendet von&quot;](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)**: Administratoren können jetzt alle Asset-Links &quot;Verwendet von&quot;für ein ausgewähltes Feld in eine CSV-Datei exportieren. Diese Verbesserung kann sowohl Administratoren als auch Nicht-Administratoren bei der Bereinigung nicht verwendeter Felder unterstützen. Darüber hinaus können Assets jetzt in einer neuen Registerkarte oder einem neuen Browser-Fenster geöffnet werden.

## Kundenbezogenes Marketing {#account-based-marketing}

![(Stern)](assets/yellow-star.png)

* **Aktualisierte Benutzeroberfläche für Kontoprofil-Profiling**: Vereinfachen Sie die Erstellung Ihrer Zielkontoliste in der Kontoerstellung mit optimierten Schritten - alles in einem einzigen Bildschirm.

<br> 

**_Veröffentlichung im gesamten Quartal_**

Die folgenden Funktionen befinden sich in einem nicht vierteljährlichen Zyklus und werden in den kommenden Monaten veröffentlicht.

* **Forms-Dienst**: Wir führen eine strengere Validierung der Formularfeldsyntax und die Möglichkeit ein, gängige Bot-Muster mit den neuen Funktionen für sichere Domänen für Einstiegsseiten zu blockieren. Das Blockieren von Bot-Mustern kann die Übermittlung von Spam-Formularen reduzieren und die Qualität Ihrer Datenbank verbessern.

>[!NOTE]
>
>Die vollständige Einführung der erweiterten Validierung der Formularfeldsyntax wurde auf einen Zeitpunkt nach unserer Version vom Januar 2021 verschoben.

* **Maximale Asset-API-URI-Größe**: Die Größenbeschränkung für die Uniform Resource Identifier (URI) wird von 8 KB auf 65 KB erhöht, bevor der Parameter &quot;_method&quot;entfernt wird. Bei der Ausführung langer Abfragezeichenfolgen ermöglicht diese Größenbeschränkung die einfachere Übergabe der Daten. Das Entfernen des Parameters &quot;_method&quot;ist Teil eines bevorstehenden Sicherheits-Upgrades.

## Sales Insight {#sales-insight}

![(Stern)](assets/yellow-star.png)

* **[Sales Insight für Kunden mit nicht nativer Salesforce CRM-Integration aktiviert](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md) (Beta)**: Marketo Engage-Kunden mit nicht nativen Salesforce-CRM-Integrationen können jetzt Sales Insight verwenden, um ihren Vertriebsteams zu helfen, die am stärksten engagierten Leads und Chancen zu verstehen, zu priorisieren und mit ihnen zu interagieren, um intelligente Verkaufsstrategien und schnellere Angebote zu ermöglichen.

## SalesConnect {#sales-connect}

![(Stern)](assets/yellow-star.png)

* **[Verbesserte Zustimmung von zwei Parteien für Verkaufsaufrufe:](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)** Administratoren haben jetzt mehr Kontrolle über die Aufrufaufzeichnungskonfigurationen. [Aufrufaufzeichnungen aktivieren](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md) mit der Gewissheit, dass Sie das Einverständnisgesetz von zwei Parteien einhalten. Automatisieren Sie die Benachrichtigung über den aufgezeichneten Aufruf und aktivieren Sie die Audioclips, die vor dem Aufruf abgespielt werden sollen.

<br> 

## Mitteilungen und veraltete Elemente {#announcements-deprecations}

* **Asset-API &quot;_method&quot;Parameterlöschung**: Ab September 2020 akzeptieren die Asset-API-Endpunkte &quot;_method&quot;nicht mehr, um Abfrageparameter in einem POST-Textkörper weiterzugeben, um URI-Längenbeschränkungen zu umgehen. Um Anforderungen aufzunehmen, die diesen Parameter erfordern, werden die URI-Beschränkungen für Asset-APIs von 8 KB auf 65 KB erhöht.
* **[Munchkin Associate Lead](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**: Mit dieser Version des Munchkin JavaScript-Clients, Version 159, werden wir die Einstellung der Munchkin Associate Lead-Methode starten. Wenn Sie aufgerufen werden, erhalten Sie eine Warnung, die angibt, dass die Methode in einer zukünftigen Version entfernt wird. Nach dem Entfernen ist die Methode nicht mehr funktionsfähig und Versuche, sie zu verwenden, schlagen fehl. Marketo Engage-Kunden, die diese Methode vor kurzem verwendet haben, werden einzeln über ihre Verwendung informiert.
* **Unterstützung für Internet Explorer**: Wie bereits angekündigt, endet die Marketo Engage-Unterstützung für Internet Explorer 11 am **31. Juli 2020**. Google Chrome, Mozilla Firefox, Apple Safari und Microsoft Edge werden weiterhin unterstützt.
* **Sky Default Experience**: Die Option, mit der Administratoren oder Benutzer Marketo Sky als Standarderlebnis festlegen können, wird in dieser Version entfernt, um eine Aktualisierung des primären Benutzererlebnisses vorzubereiten. Weitere Informationen zur Aktualisierung des primären Erlebnisses, die für Ende dieses Jahres geplant ist, werden im Juli verfügbar sein. Benutzer, die Marketo Sky als Standarderlebnis festgelegt haben oder Zugriff auf Marketo Sky erhalten haben, können weiterhin von einer Kachel auf der My Marketo-Startseite aus auf Marketo Sky zugreifen.
* **Microsoft Edge-Unterstützung für EdgeHTML (Nicht-Chromium)**: Marketo Engage unterstützt Ende 2020 keine EdgeHTML-Versionen von Microsoft Edge mehr. Ab dem 1. Januar 2021 wird nur die neueste Chromium-Version von Microsoft Edge unterstützt.
