---
description: Mai 2025 - Versionshinweise zu Marketo - Produktdokumentation
title: Versionshinweise – Mai 2025
feature: Release Information
exl-id: 99cd1d54-0a80-40fa-9d0c-1cb437be90f0
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 3%

---

# Mai 2025 - Versionshinweise {#release-notes-may-25}

Im Folgenden finden Sie alle Funktionen, die in der Version vom Mai 2025 enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage Edition auf die Verfügbarkeit der Funktionen.

Die Versionshinweise speziell für Adobe Dynamic Chat [finden Sie hier](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie vom Marketo Engage-Support.

## Standardfunktionen des Veröffentlichungszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Veröffentlichungszyklus und werden ab dem 23. **2025 veröffentlicht** wobei die verbleibenden Funktionen in den folgenden Wochen schrittweise bereitgestellt werden. Veröffentlichungsfunktionen und -daten können sich ändern. Überprüfen Sie neben jeder Funktion auf ihren Status.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
  <tr>
   <td><strong>Rollenbasierte Zugriffssteuerung für E-Mail-Designer Assets</strong>: Eine neue Erweiterung des rollenbasierten Zugriffssteuerungssystems (RBAC) bietet detailliertere Berechtigungen und eine verbesserte Benutzerverwaltung für Assets, die von der neuen E-Mail-Designer unterstützt werden.</td>
   <td>Versendet</td>
   <td><a href="https://nation.marketo.com/t5/latest-product-innovations/product-updates-granular-permissions-to-new-email-designer/ba-p/357057">Granulare Berechtigungen für neue E-Mail-Designer (Blogpost)</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>In der E-Mail-Designer erstellte E-Mails klonen</strong>: Sie können jetzt eine bestehende E-Mail klonen, die mit der neuen E-Mail-Designer erstellt wurde.</td>
   <td>Versendet</td>
   <td>k. A.</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Trigger-Token für beliebiges Attribut</strong>: Erweiterte Liste von Trigger-Token zur Unterstützung der Verwendung von Daten aus beliebigen Aktivitätsattributen in Smart-Kampagnenfeldern.</td>
   <td>Versendet</td>
   <td>k. A.</td>
  </tr>
 </tbody>
</table>
<br/>

## Ankündigungen {#announcements}

* **Aktualisierung der Facebook-Offline-Konversionsintegration**: Am 29. Mai 2025 wird die [Facebook-Offline-Konversions](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions){target="_blank"}-Integration für Marketo Engage in die neue Meta [Conversions-API](https://developers.facebook.com/docs/marketing-api/conversions-api){target="_blank"} migriert, da Meta die [Offline-Konversions-API](https://developers.facebook.com/docs/marketing-api/offline-conversions/){target="_blank"} im Einklang mit der Graph-API-Versionierung einstellt. Weitere Informationen finden Sie im Meta-Handbuch zu [Senden von Offline-Ereignissen über die Konversions-API](https://developers.facebook.com/docs/marketing-api/conversions-api/offline-events/){target="_blank"} (CAPI für Offline).

* **Neue Analytics-Funktion - Öffentliche Beta**: [Advanced BI Analytics](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"} (früher als Revenue Explorer und Advanced Report Builder bezeichnet) begann Mitte April mit dem Rollout an alle aktuellen Benutzenden des Umsatzzyklus-Explorers. Dieses neue Tool bietet eine flexible Reporting- und Visualisierungsschnittstelle zu Marketo Engage-Daten und liefert detaillierte Informationen zu Fortschritt, Leistung und mehr. Er bietet mehr Interaktivität und Visualisierung, schnellere Leistung und ein nahtloseres und intuitiveres Benutzererlebnis.

Um auf diese Funktion zugreifen zu können, müssen Sie das Add-on „Advanced BI Analytics“ erworben haben. Weitere Informationen erhalten Sie beim Adobe Account Team (Ihrem Account Manager).

* **Einstellung von REST-API-„access_token“-**: Der `access_token` Abfrageparameter, der zum Authentifizieren von Marketo REST-API-Aufrufen verwendet wird, wird nicht mehr unterstützt und wird nach dem 31. Oktober 2025 nicht mehr verfügbar sein. Alle neuen und vorhandenen Integrationen sollten REST-API-Aufrufe mit dem Header „Authorization“ authentifizieren [wie hier beschrieben](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Einstellung der SOAP-**: Die Unterstützung für die Marketo SOAP-API endet am 31. Oktober 2025. Services, die SOAP-API-Funktionen verwenden, sollten zur [REST-API“ migriert ](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
