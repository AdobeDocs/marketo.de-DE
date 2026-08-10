---
description: Aktuelle Versionshinweise – Marketo-Dokumente – Produktdokumentation
title: Aktuelle Versionshinweise
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
TQID: https://experienceleague.adobe.com/QJFy7PeGXlvS3jcJGcZJROlc8c1UvphO-TOOwPUQeX8
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: f71e690b-4480-4b67-9ef5-88f42f9cdfdbid: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2: id: c942e9f6-ed06-481a-abdd-1195363d1452
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 2b3c872bfdef4b5cd8e80f754609dd0059c164b2
workflow-type: tm+mt
source-wordcount: 434
ht-degree: 21%

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
   <td><strong>Neue Benutzeroberfläche von Marketo Engage</strong>: Die Benutzeroberfläche von Marketo Engage hat ein aktualisiertes Design, einschließlich aktualisierter Menüs, Symbole und Layouts, für ein saubereres, moderneres Erlebnis. Dies ist nur eine visuelle Aktualisierung, es sind keine vorhandenen Funktionen oder Workflows betroffen.
</td>
   <td>Schrittweiser Rollout im Verlauf des Monats August</td>
   <td><i>Nicht zutreffend</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Email Designer - Script Builder</strong>: Script Builder ist ein KI-basierter Assistent, der Ihnen hilft, Personalisierungsskripte schneller zu erstellen.
</td>
   <td><i>Demnächst</i></td>
   <td><i>Demnächst</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Kampagnen im Archiv deaktivieren</strong>: Durch die Archivierung eines Ordners werden jetzt alle Kampagnen in diesem Ordnerbaum deaktiviert und gekündigt, sodass archivierte Smart-Kampagnen nicht unerwartet ausgeführt werden.
</td>
   <td><i>Demnächst</i></td>
   <td><i>Demnächst</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Ankündigungen {#announcements}

* **Einstellung von REST-API-„access_token“-**: Der `access_token` Abfrageparameter, der zum Authentifizieren von Marketo REST-API-Aufrufen verwendet wird, wird nicht mehr unterstützt und ist nach dem 31. August 2026 nicht mehr verfügbar. Alle neuen und vorhandenen Integrationen sollten REST-API-Aufrufe mit dem Header „Authorization“ authentifizieren, [wie hier beschrieben](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **REST API-Kampagnenausführungs-ID**: Unter bestimmten Umständen wurde der Wert der Kampagnenausführungs-ID einer Aktivität manchmal mit falscher Formatierung zwischen zwei Paaren von Anführungszeichen (z. B. `"campaignRunId": ""102938""`) zurückgegeben.<br/>Ab der August-Version wird dieser Wert immer im richtigen numerischen Format (`"campaignRunId": 102938`) zurückgegeben

* **Statische Listengrößenbeschränkungen für Lead-Aktivitäten abrufen und Lead-Änderungen abrufen**: Ab dem 30. September 2026 schlagen Aufrufe der Endpunkte „Lead-Aktivitäten abrufen“ oder „Lead-Änderungen abrufen“, die den `listId` enthalten, fehl, wenn die Ziellisten 10.000 oder mehr Leads enthalten, mit einem Fehler-Code 1003, der angibt, dass die statische Zielliste zu viele Datensätze enthält.

Weitere Informationen finden Sie [Migrationshandbuch](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"} .

* **Limit für REST-API-Zusammenführung von Leads**: Seit dem 31. Juli 2026 führen Aufrufe, die mehr als 25 IDs im leadIds-Parameter eines Zusammenführungs-Leads-API-Aufrufs enthalten, zu einem 1080-Fehler-Code, und der Aufruf wird übersprungen. Aufträge, die die Zusammenführung von mehr als 25 Datensätzen in einem erfordern, sollten in mehrere Aufträge aufgeteilt werden, um den Erfolg dieser Aufrufe sicherzustellen.
