---
description: Juli 2026 - Versionshinweise zu Marketo - Produktdokumentation
title: Juli 2026 - Versionshinweise
feature: Release Information
source-git-commit: edeb795f12082fab9c72b0ff4305f3db90aa4c46
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 15%
---
# Versionshinweise: August 2026 {#release-notes-aug-26}

Unten finden Sie alle Funktionen, die in der Version vom 26. August enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage Edition auf die Verfügbarkeit der Funktionen.

Die Versionshinweise speziell für Adobe Dynamic Chat [finden Sie hier](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Funktionen aus dem standardmäßigen Veröffentlichungszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Veröffentlichungszyklus und werden ab dem 14. **2026 veröffentlicht** wobei die verbleibenden Funktionen in den folgenden Wochen schrittweise bereitgestellt werden. Funktionen und Veröffentlichungstermine können sich ändern. Überprüfen Sie neben jeder Funktion ihren Status.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
  <tr>
   <td><strong>Neue Benutzeroberfläche von Marketo Engage</strong>: Die Benutzeroberfläche von Marketo Engage hat ein aktualisiertes Design, einschließlich aktualisierter Menüs, Symbole und Layouts, für ein saubereres, moderneres Erlebnis. Dies ist nur eine visuelle Aktualisierung. Vorhandene Funktionen oder Workflows sind davon nicht betroffen.
</td>
   <td>Schrittweiser Rollout im August und September</td>
   <td><i>Nicht zutreffend</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Kampagnen im Archiv deaktivieren</strong>: Durch die Archivierung eines Ordners werden jetzt alle Kampagnen in diesem Ordnerbaum deaktiviert und gekündigt, sodass archivierte Smart-Kampagnen nicht unerwartet ausgeführt werden.
</td>
   <td>Freigegeben</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-folders#disable-campaigns-archive" target="_blank">Deaktivieren von Kampagnen im Archiv</a></td>
  </tr>
    <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer - Kontextmenü für Inhalte generieren</strong>: Die Funktionen zum Generieren von Inhalten in der E-Mail-Designer können jetzt über das Kontextmenü (den schwarzen Balken) aufgerufen werden. Wenn Sie beispielsweise Textinhalte auswählen, wird im Kontextmenü das Symbol Inhalt generieren angezeigt, über das Sie Schnellaktionen durchführen können.</td>
   <td><i>Demnächst</i></td>
   <td><i>Demnächst</i></td>
  </tr>
  </tr>
  </tbody>
</table>
<br/>

## Ankündigungen {#announcements}

* **Marketo AI ist jetzt ein Mitarbeiter für Marketo Engage**: Ein Mitarbeiter für Marketo Engage bietet Agentenfähigkeiten, die darauf ausgelegt sind, zeitaufwendige Marketing-Funktionen zu automatisieren. Neuer Name, gleiche Funktionen, für alle Benutzer verfügbar. [Weitere Informationen](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/coworker-for-marketo/overview){target="_blank"}

* **Einstellung von REST-API-„access_token“-**: Der `access_token` Abfrageparameter, der zum Authentifizieren von Marketo REST-API-Aufrufen verwendet wird, wird nicht mehr unterstützt und ist nach dem 31. August 2026 nicht mehr verfügbar. Alle neuen und vorhandenen Integrationen sollten REST-API-Aufrufe mit dem Header „Authorization“ authentifizieren, [wie hier beschrieben](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **REST API-Kampagnenausführungs-ID**: Unter bestimmten Umständen wurde der Wert der Kampagnenausführungs-ID einer Aktivität manchmal mit falscher Formatierung zwischen zwei Paaren von Anführungszeichen (z. B. `"campaignRunId": ""102938""`) zurückgegeben.<br/>Ab der August-Version wird dieser Wert immer im richtigen numerischen Format (`"campaignRunId": 102938`) zurückgegeben

* **Statische Listengrößenbeschränkungen für Lead-Aktivitäten abrufen und Lead-Änderungen abrufen**: Ab dem 30. September 2026 schlagen Aufrufe der Endpunkte „Lead-Aktivitäten abrufen“ oder „Lead-Änderungen abrufen“, die den `listId`-Parameter enthalten, mit einem 1003-Fehler-Code fehl (was anzeigt, dass die statische Zielliste zu viele Datensätze enthält), wenn die Ziellisten 10.000 oder mehr Leads enthalten. Weitere Informationen finden Sie [Migrationshandbuch](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"} .

* **Limit für REST-API-Zusammenführung von Leads**: Seit dem 31. Juli 2026 führen Aufrufe, die mehr als 25 IDs im leadIds-Parameter eines Zusammenführungs-Leads-API-Aufrufs enthalten, zu einem 1080-Fehler-Code, und der Aufruf wird übersprungen. Aufträge, die die Zusammenführung von mehr als 25 Datensätzen in einem erfordern, sollten in mehrere Aufträge aufgeteilt werden, um den Erfolg dieser Aufrufe sicherzustellen.
