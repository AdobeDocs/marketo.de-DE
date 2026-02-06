---
description: März 2025 - Versionshinweise zu Marketo - Produktdokumentation
title: Versionshinweise – März 2025
feature: Release Information
exl-id: a0e45d8e-6b74-4ab0-a1ba-4dae3754bc8f
source-git-commit: 8e72b24e18ae108ec74e6d4fa6b04f10130439a4
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 38%

---

# Versionshinweise – März 2025 {#release-notes-mar-25}

Nachstehend finden Sie alle Funktionen, die in der Version vom 25. März enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf die Verfügbarkeit der Funktionen.

Die Versionshinweise speziell für Adobe Dynamic Chat [finden Sie hier](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie vom Marketo Engage-Support.

## Funktionen aus dem standardmäßigen Veröffentlichungszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Veröffentlichungszyklus und werden ab dem **Samstag, 28. März 2025** veröffentlicht, wobei die verbleibenden Funktionen in den folgenden Wochen schrittweise bereitgestellt werden. Veröffentlichungsfunktionen und -daten können sich ändern. Überprüfen Sie neben jeder Funktion ihren Status.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
    <tr>
   <td><strong>E-Mail-Designer in allen Programmen verfügbar</strong>: Die neuen E-Mails von E-Mail-Designer sind jetzt für alle Interaktions-, Standard- und Veranstaltungsprogramme verfügbar (mit Ausnahme interaktiver Webinar-Programme). Zuvor waren sie nur in E-Mail-Programmen verfügbar.</td>
   <td>Freigegeben</td>
   <td>k. A.</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>GenAI-Funktionen in interaktiven Webinaren</strong>: Sie können jetzt Kapitel sowie eine Zusammenfassung für On-Demand-Webinare erstellen. Bearbeiten und exportieren Sie eine HTML-Datei Ihrer Daten.</td>
   <td>Freigegeben</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/gen-ai">GenAI-Funktionen</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Meine Token für Global und Workspace</strong>: Konfigurieren Sie meine Token sowohl auf Arbeitsbereich- als auch auf globaler Ebene, um eine verbesserte Produktivität und Kontrolle über Marken- und Marketingmaterialien in Marketo Engage-Arbeitsbereichen und sogar ganzen Instanzen zu ermöglichen.</td>
   <td>Freigegeben</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md#create-a-my-token">Erstellen eines globalen My Token</a></td>
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

Ab diesem Zeitpunkt waren Benutzende nicht mehr in der Lage, diese Social-Media-Funktionen in Marketo Engage zu erstellen, zu klonen oder einzubetten. Vorhandene soziale Assets funktionieren bis zum 31. Januar 2025 weiterhin. Am 1. Februar 2025 hörten die sozialen Assets auf zu funktionieren. Alle in Landingpages eingebetteten Social-Media-Funktionen müssen entfernt werden. [Weitere Informationen](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **Einstellung des Parameters „access_token“ der REST-API**: Der Abfrageparameter `access_token`, der zum Authentifizieren von Marketo-REST-API-Aufrufen verwendet wird, wird nicht mehr unterstützt und ist nach dem 31. März 2026 nicht mehr verfügbar. Alle neuen und vorhandenen Integrationen sollten REST-API-Aufrufe mit dem Header „Authorization“ authentifizieren, [wie hier beschrieben](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Abschaffung der SOAP-API**: Die Unterstützung für die Marketo SOAP-API endet am 31. März 2026. Services, die SOAP-API-Funktionen verwenden, sollten zur [REST-API](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} migriert werden.

* **Neue Analytics-Funktion - Öffentliche Beta**: [Advanced BI Analytics](/help/marketo/product-docs/reporting/advanced-bi-analytics/overview.md){target="_blank"} (früher als Revenue Explorer und Advanced Report Builder bezeichnet) wird ab Mitte April für alle aktuellen Benutzenden des Umsatzzyklus-Explorers bereitgestellt. Dieses neue Tool bietet eine flexible Reporting- und Visualisierungsschnittstelle zu Marketo Engage-Daten und liefert detaillierte Informationen zu Fortschritt, Leistung und mehr. Er bietet mehr Interaktivität und Visualisierung, schnellere Leistung und ein nahtloseres und intuitiveres Benutzererlebnis.

Um auf diese Funktion zugreifen zu können, müssen Sie das Add-on „Advanced BI Analytics“ erworben haben. Weitere Informationen erhalten Sie beim Adobe Account Team (Ihrem Account Manager).
