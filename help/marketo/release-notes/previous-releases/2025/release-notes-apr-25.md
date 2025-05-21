---
description: Aktuelle Versionshinweise – Marketo-Dokumente – Produktdokumentation
title: Aktuelle Versionshinweise
feature: Release Information
exl-id: 94010780-41aa-4212-a1d4-1b78806bd728
source-git-commit: 701155a5beccf3725fe26d2bc75c541c989d4af4
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 6%

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
   <td><strong>SSL-Self-Service (Secure Socket Layer</strong>: Mit der SSL-Verschlüsselung können Sie Landingpages für eine Marketo Engage-Instanz sicher machen. Die Aktivierung dieser Funktion erforderte in der Regel die Unterstützung des Adobe-Supportteams. Marketo-Anwender können sie jetzt selbst aktivieren und so wertvolle Zeit sparen.</td> 
   <td>Versendet</td>
   <td><a href="/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/add-ssl-to-your-landing-pages.md">Hinzufügen von SSL zu Ihren Landingpages</a></td>
  </tr>
 </tbody> 
</table>
<br/>

## Ankündigungen {#announcements}

* **Neue Analytics-Funktion - Öffentliche Beta**: [Advanced BI Analytics](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"} (früher als Revenue Explorer und Advanced Report Builder bezeichnet) wird ab Mitte April für alle aktuellen Benutzenden des Umsatzzyklus-Explorers bereitgestellt. Dieses neue Tool bietet eine flexible Reporting- und Visualisierungsschnittstelle zu Marketo Engage-Daten und liefert detaillierte Informationen zu Fortschritt, Leistung und mehr. Er bietet mehr Interaktivität und Visualisierung, schnellere Leistung und ein nahtloseres und intuitiveres Benutzererlebnis.

Um auf diese Funktion zugreifen zu können, müssen Sie das Add-on „Advanced BI Analytics“ erworben haben. Weitere Informationen erhalten Sie beim Adobe Account Team (Ihrem Account Manager).

* **Einstellung von REST-API-„access_token“-**: Der `access_token` Abfrageparameter, der zum Authentifizieren von Marketo REST-API-Aufrufen verwendet wird, wird nicht mehr unterstützt und wird nach dem 31. Oktober 2025 nicht mehr verfügbar sein. Alle neuen und vorhandenen Integrationen sollten REST-API-Aufrufe mit dem Header „Authorization“ authentifizieren [wie hier beschrieben](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Einstellung der SOAP-**: Die Unterstützung für die Marketo SOAP-API endet am 31. Oktober 2025. Services, die SOAP-API-Funktionen verwenden, sollten zur [REST-API“ migriert ](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

* **Einstellung von Social**: Am Mittwoch, 31. Juli 2024, begann Marketo Engage mit der Einstellung der folgenden Social-Media-Funktionen innerhalb des Produkts:

   * Umfragen
   * Social-Schaltfläche
   * Empfehlungsangebot
   * Videofreigabe
   * Gewinnspiele

Ab diesem Zeitpunkt waren Benutzende nicht mehr in der Lage, diese Social-Media-Funktionen in Marketo Engage zu erstellen, zu klonen oder einzubetten. Vorhandene soziale Assets funktionieren bis zum 31. Januar 2025 weiterhin. Am 1. Februar 2025 hörten die sozialen Assets auf zu funktionieren. Alle in Landingpages eingebetteten Social-Media-Funktionen müssen entfernt werden. [Weitere Informationen](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}
