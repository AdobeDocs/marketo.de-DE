---
description: Aktuelle Versionshinweise – Marketo-Dokumente – Produktdokumentation
title: Aktuelle Versionshinweise
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 978bbe4de06a0e269b60108e5a91edc5499dc9c1
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 7%

---

# März 2025 - Versionshinweise {#release-notes-mar-25}

Nachstehend finden Sie alle Funktionen, die in der Version vom 25. März enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage Edition auf die Verfügbarkeit der Funktionen.

Die Versionshinweise speziell für Adobe Dynamic Chat [finden Sie hier](/help/marketo/release-notes/dynamic-chat.md).

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie vom Marketo Engage-Support.

## Standardfunktionen des Veröffentlichungszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Veröffentlichungszyklus und werden ab dem 28. **2025 veröffentlicht** wobei die verbleibenden Funktionen in den folgenden Wochen schrittweise bereitgestellt werden. Veröffentlichungsfunktionen und -daten können sich ändern. Überprüfen Sie neben jeder Funktion auf ihren Status.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Funktion</th> 
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
    <tr> 
   <td><strong>E-Mail-Designer in allen Programmen verfügbar</strong>: Die neuen E-Mails von E-Mail-Designer sind jetzt für alle Interaktions-, Standard- und Veranstaltungsprogramme verfügbar (mit Ausnahme interaktiver Webinar-Programme). Zuvor waren sie nur in E-Mail-Programmen verfügbar. Mit diesem Update wird auch das Klonen verfügbar.</td>
   <td>Versendet</td>
   <td>k. A.</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>GenAI-Funktionen in interaktiven Webinaren</strong>: Sie können jetzt Kapitel sowie eine Zusammenfassung für On-Demand-Webinare erstellen. Bearbeiten und exportieren Sie eine HTML-Datei Ihrer Daten.</td>
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Meine Token für Global und Workspace</strong>: Konfigurieren Sie meine Token sowohl auf Arbeitsbereich- als auch auf globaler Ebene, um eine verbesserte Produktivität und Kontrolle über Marken- und Marketingmaterialien in Marketo Engage-Arbeitsbereichen und sogar ganzen Instanzen zu ermöglichen.</td> 
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Token für ein beliebiges Trigger-Attribut</strong>: Erweitert die Liste der verfügbaren Trigger-Token von nur dem Liste in <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments" target="_blank">diesem Dokument</a> , um die Verwendung von Daten aus einem beliebigen auslösenden Aktivität-Attribut in Kampagne Flow-Feldern zu unterstützen. Druck Daten aus einem Aktivität Attribut in einen interessanten Moment oder legen Sie die letzte Transaktions-ID eines Lead aus einer benutzerdefinierten Aktivität in ein Lead Feld fest.</td> 
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Ankündigungen {#announcements}

* **Einstellung von Social**: Am Mittwoch, 31. Juli 2024, begann Marketo Engage mit der Einstellung der folgenden Social-Media-Funktionen innerhalb des Produkts:

   * Umfragen
   * Social-Schaltfläche
   * Empfehlungsangebot
   * Videofreigabe
   * Gewinnspiele

Bis dahin konnten Benutzer keine dieser Social Funktionen in Marketo Engage erstellen, klonen oder einbetten. Bestehende Social Assets funktionieren weiterhin bis zum 31. Januar 2025. Am 1. Februar 2025 stellten Social Vermögenswerte ihre Funktion ein. Alle in Landingpages eingebetteten Social-Media-Funktionen müssen entfernt werden. [Weitere Informationen](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977)

* **Einstellung von REST-API-„access_token“-**: Der `access_token` Abfrageparameter, der zum Authentifizieren von Marketo REST-API-Aufrufen verwendet wird, wird nicht mehr unterstützt und ist nach dem 30. Juni 2025 nicht mehr verfügbar. Alle neuen und vorhandenen Integrationen sollten REST-API-Aufrufe mit dem Header „Authorization“ authentifizieren [wie hier beschrieben](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication).

* **SOAP-API-veraltet**: Die Unterstützung für die Marketo-SOAP-API endet am 31. Oktober 2025. Services, die SOAP-API-Funktionen verwenden, sollten zur [REST-API“ migriert ](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api).

* **Neu Analytics Feature – Public Beta**: [Erweitert BI Analytics](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md) (früher bekannt als Revenue Explorer und Erweitert Report Builder) beginnt Mitte April mit dem Rollout für alle aktuellen Revenue Cycle Explorer-Benutzer. Dieses neue Tool bietet eine flexible Berichte- und Visualisierungsoberfläche für Marketo Engage Daten und liefert granulare Details zu Fortschritt, Leistung und mehr. Er bietet mehr Interaktivität und Visualisierung, schnellere Leistung und ein nahtloseres und intuitiveres Benutzererlebnis.

Um auf diese Funktion zugreifen zu können, müssen Sie das Add-on „Advanced BI Analytics“ erworben haben. Weitere Informationen erhalten Sie beim Adobe Account Team (Ihrem Account Manager).
