---
unique-page-id: 45416698
description: Versionshinweise - 20. Juli - Marketo Docs - Produktdokumentation
title: Versionshinweise - Juli 20
exl-id: 3c9b1f1d-961c-4bf8-8b99-37b483230506
translation-type: tm+mt
source-git-commit: d44f5e6f3fb24a25678e4d15ee4c6361b658556b
workflow-type: tm+mt
source-wordcount: '653'
ht-degree: 1%

---

# Versionshinweise: Juli &#39;20 {#release-notes-july}

Die folgenden Funktionen sind in der Version vom 20. Juli enthalten. Überprüfen Sie Ihre Marketo Edition auf Funktionsverfügbarkeit.

>[!AVAILABILITY]
>
>Beachten Sie, dass je nach aktuellem Paket Artikel mit einem Stern ( ![(star)](assets/yellow-star.png)) möglicherweise den Kauf eines Wertzusatzes erfordern. Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zu erhalten.

**_Vierteljährliche_** ReleasesDie folgenden Funktionen werden am 31.  **Juli 2020** veröffentlicht.

## Administration {#administration}

* **[&quot;Verwendet von&quot;-Export in Feldverwaltung](/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md)**: Administratoren können jetzt alle Asset-Links &quot;Verwendet von&quot;für ein ausgewähltes Feld in eine CSV-Datei exportieren. Diese Verbesserung kann sowohl Administratoren als auch Nichtadministratoren bei der Bereinigung nicht verwendeter Felder unterstützen. Außerdem können Assets jetzt in einer neuen Browserregisterkarte oder einem neuen Browserfenster geöffnet werden.

## Kundenbezogenes Marketing {#account-based-marketing}

![(Stern)](assets/yellow-star.png)

* **Aktualisierte Benutzeroberfläche für die Kontoprofilerstellung**: Vereinfachen Sie die Erstellung Ihrer Zielgruppe-Konto-Liste im Kontoprofil mit optimierten Schritten in einem einzigen Bildschirm.

<br> 

**_Veröffentlichung im gesamten Quartal_**

Die folgenden Funktionen befinden sich in einem nicht vierteljährlichen Zyklus und werden in den kommenden Monaten veröffentlicht.

* **Forms-Dienst**: Wir führen eine stärkere Formularfeldsyntax-Überprüfung und die Möglichkeit ein, gängige Bot-Muster mit neuen Funktionen für sichere Domänen für Landingpages zu blockieren. Durch das Blockieren von Bot-Mustern können Sie die Übermittlung von Spam-Formularen reduzieren und die Qualität Ihrer Datenbank verbessern.

>[!NOTE]
>
>Die vollständige Einführung der erweiterten Formularfeldsyntax-Überprüfung wurde nach unserer Version vom Januar 2021 verschoben.

* **Maximale URI-Größe** für Asset-API: Die Größenbeschränkung der einheitlichen Ressourcenkennung (URI) wird von 8 KB auf 65 KB erhöht, bevor der Parameter &quot;_method&quot;entfernt wird. Bei Zeichenfolgen mit langer Abfrage können die Daten aufgrund dieser Größenbeschränkung leichter übergeben werden. Die Entfernung des Parameters &quot;_method&quot;ist Teil einer bevorstehenden Sicherheitsaktualisierung.

## Sales Insight {#sales-insight}

![(Stern)](assets/yellow-star.png)

* **[Sales Insight aktiviert für Kunden mit nicht nativer Salesforce CRM-Integration](/help/marketo/product-docs/marketo-sales-insight/sales-insight-for-non-native-salesforce-integrations.md)  (Beta)**: Marketo Engage-Kunden mit nicht-nativen Salesforce CRM-Integrationen können nun Sales Insight verwenden, um ihren Vertriebsteams zu helfen, die am meisten engagierten Interessenten und Chancen zu verstehen, zu priorisieren und mit ihnen zu interagieren, um intelligentes Verkaufen und schnellere Geschäfte zu ermöglichen.

## SalesConnect {#sales-connect}

![(Stern)](assets/yellow-star.png)

* **[Verbesserte Zweiparteizustimmungen für Verkaufsaufrufe:](/help/marketo/product-docs/marketo-sales-connect/phone/two-party-consent-settings.md)** Administratoren haben jetzt eine größere Kontrolle über die Konfigurationen für die Aufzeichnung von Aufrufen. [Aktivieren Sie ](/help/marketo/product-docs/marketo-sales-connect/phone/enable-call-recording.md) Aufrufe mit der Gewissheit, dass Sie das Zweitanbieter-Einwilligungsgesetz einhalten. Automatisieren Sie die Benachrichtigung über den aufgezeichneten Aufruf und aktivieren Sie Audioclips, die vor dem Aufruf wiedergegeben werden sollen.

<br> 

## Mitteilungen und Veraltungen {#announcements-deprecations}

* **Asset-API &quot;_method&quot;-Parameterentfernung**: Ab September 2020 akzeptieren die Asset-API-Endpunkte &quot;_method&quot;nicht mehr, um Abfragen-Parameter in einem POST-Textkörper zu übergeben, um die Längenbeschränkungen des URI zu umgehen. Um Anforderungen, die diesen Parameter erfordern, anzupassen, werden die URI-Beschränkungen für Asset-APIs von 8 KB auf 65 KB erhöht.
* **[Munchkin Associate Lead](https://developers.marketo.com/blog/deprecation-of-munchkin-associate-lead-method/)**: Mit dieser Version des Munchkin JavaScript-Client, Version 159, beginnen wir mit der Einstellung der Munchkin Associate Lead-Methode. Wenn sie aufgerufen wird, erhalten Sie eine Warnung, dass die Methode in einer zukünftigen Version entfernt wird. Nach dem Entfernen ist die Methode nicht mehr funktionsfähig, und Versuche, sie zu verwenden, schlagen fehl. Marketo Engage-Kunden, die diese Methode vor kurzem verwendet haben, werden einzeln über ihre Verwendung informiert.
* **Unterstützung für Internet Explorer**: Wie bereits angekündigt, endet die Marketo Engage-Unterstützung für Internet Explorer 11 am 31.  **Juli 2020**. Google Chrome, Mozilla Firefox, Apple Safari und Microsoft Edge werden weiterhin unterstützt.
* **Sky-Standarderlebnis**: Die Option, mit der Administratoren oder Benutzer Marketo Sky als Standarderlebnis festlegen können, wird in dieser Version entfernt, um eine Aktualisierung der primären Benutzererfahrung vorzubereiten. Weitere Informationen über die für Ende des Jahres geplante Aktualisierung der primären Erfahrung werden im Juli verfügbar sein. Benutzer, die Marketo Sky als Standard-Erlebnis festgelegt haben oder Zugriff auf Marketo Sky erhalten haben, können weiterhin von einer Kachel auf der Startseite My Marketo auf Marketo Sky zugreifen.
* **Unterstützung** von EdgeHTML (nicht Chromium) Microsoft Edge: Marketo Engage unterstützt Ende 2020 keine EdgeHTML-Versionen von Microsoft Edge mehr. Ab dem 1. Januar 2021 wird nur die neueste Chromium-Version von Microsoft Edge unterstützt.
