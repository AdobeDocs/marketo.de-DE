---
description: Aktuelle Versionshinweise – Marketo-Dokumente – Produktdokumentation
title: Aktuelle Versionshinweise
hide: true
hidefromtoc: true
feature: Release Information
source-git-commit: 44ea3d408cf460b41f3fa92c639ca089a195a4bc
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 9%

---

# Versionshinweise: April 2025 {#release-notes-apr-25}

Im Folgenden finden Sie alle Funktionen, die in der Version vom April 2025 enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage Edition auf die Verfügbarkeit der Funktionen.

Die Versionshinweise speziell für Adobe Dynamic Chat [finden Sie hier](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie vom Marketo Engage-Support.

## Standardfunktionen des Veröffentlichungszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Veröffentlichungszyklus und werden ab dem 25. **2025 veröffentlicht** wobei die verbleibenden Funktionen in den folgenden Wochen schrittweise bereitgestellt werden. Veröffentlichungsfunktionen und -daten können sich ändern. Überprüfen Sie neben jeder Funktion auf ihren Status.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Funktion</th> 
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
  <tr> 
   <td><strong>Vorlagenkompatibilität für E-Mail-Designer</strong>: E-Mail-Vorlagen aus dem klassischen E-Mail-Editor sind jetzt mit der neuen E-<a href="/help/marketo/product-docs/email-marketing/email-designer/overview.md">-Designer </a>.</td>
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>TITLE</strong>: Text.</td> 
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>TITLE</strong>: Text.</td> 
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Ankündigungen {#announcements}

* **Neue Analytics-Funktion - Öffentliche Beta**: [Advanced BI Analytics](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"} (früher als Revenue Explorer und Advanced Report Builder bezeichnet) wird ab Mitte April für alle aktuellen Benutzenden des Umsatzzyklus-Explorers bereitgestellt. Dieses neue Tool bietet eine flexible Reporting- und Visualisierungsschnittstelle zu Marketo Engage-Daten und liefert detaillierte Informationen zu Fortschritt, Leistung und mehr. Er bietet mehr Interaktivität und Visualisierung, schnellere Leistung und ein nahtloseres und intuitiveres Benutzererlebnis.

Um auf diese Funktion zugreifen zu können, müssen Sie das Add-on „Advanced BI Analytics“ erworben haben. Weitere Informationen erhalten Sie beim Adobe Account Team (Ihrem Account Manager).

* **Einstellung von REST-API-„access_token“-**: Der `access_token` Abfrageparameter, der zum Authentifizieren von Marketo REST-API-Aufrufen verwendet wird, wird nicht mehr unterstützt und ist nach dem 30. Juni 2025 nicht mehr verfügbar. Alle neuen und vorhandenen Integrationen sollten REST-API-Aufrufe mit dem Header „Authorization“ authentifizieren [wie hier beschrieben](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Einstellung der SOAP-**: Die Unterstützung für die Marketo SOAP-API endet am 31. Oktober 2025. Services, die SOAP-API-Funktionen verwenden, sollten zur [REST-API“ migriert ](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

* **Einstellung von Social**: Am Mittwoch, 31. Juli 2024, begann Marketo Engage mit der Einstellung der folgenden Social-Media-Funktionen innerhalb des Produkts:

   * Umfragen
   * Social-Schaltfläche
   * Empfehlungsangebot
   * Videofreigabe
   * Gewinnspiele

Ab diesem Zeitpunkt waren Benutzende nicht mehr in der Lage, diese Social-Media-Funktionen in Marketo Engage zu erstellen, zu klonen oder einzubetten. Vorhandene soziale Assets funktionieren bis zum 31. Januar 2025 weiterhin. Am 1. Februar 2025 hörten die sozialen Assets auf zu funktionieren. Alle in Landingpages eingebetteten Social-Media-Funktionen müssen entfernt werden. [Weitere Informationen](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}
