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
source-git-commit: 14cdc585c2c5b972dd3743c5eb3e253a8a91f608
workflow-type: tm+mt
source-wordcount: 481
ht-degree: 22%

---

# Versionshinweise: Juli 2026, #1 vom 2. {#release-notes-july-26-one}

Nachstehend finden Sie alle Funktionen, die in der ersten Version vom Juli 2026 enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf die Verfügbarkeit der Funktionen.

Die Versionshinweise speziell für Adobe Dynamic Chat [finden Sie hier](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Funktionen aus dem standardmäßigen Veröffentlichungszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Veröffentlichungszyklus und werden ab dem 10. **2026 veröffentlicht** wobei die verbleibenden Funktionen in den folgenden Wochen schrittweise bereitgestellt werden. Veröffentlichungsfunktionen und -daten können sich ändern. Überprüfen Sie neben jeder Funktion ihren Status.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
  <tr>
   <td><strong>Marketo-KI-Kenntnisse - Produktwissen</strong>: Produktkenntnisse bieten Ihnen On-Demand-Zugriff auf Marketo-Know-how, ohne die Plattform verlassen zu müssen. Stellen Sie eine Frage in einfacher Sprache, und Marketo AI nutzt die offizielle Adobe-Dokumentation, um sie zu beantworten.</td>
   <td>Offene Betaversion</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-ai/skills/product-knowledge" target="_blank">Produktkenntnisse</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Marketo-KI-Kenntnisse - Leads untersuchen</strong>: Finden Sie heraus, warum eine bestimmte Person/ein Lead einen Meilenstein (wie MQL, Programmqualifikation oder eine Kampagne) nicht erreicht hat, und erhalten Sie eine Klartext-Erklärung, was passiert ist.
</td>
   <td>Offene Betaversion</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-ai/skills/investigate-leads" target="_blank">Leads untersuchen</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer - KI-Assistent Kontextmenü</strong>: Die Funktionen des KI-Assistenten der E-Mail-Designer können jetzt über das Kontextmenü (den schwarzen Balken) aufgerufen werden. Wenn Sie beispielsweise Textinhalte auswählen, wird im Kontextmenü das Symbol KI-Assistent angezeigt, über das Sie Schnellaktionen ausführen können.</td>
   <td><i>Demnächst</i></td>
   <td><i>Demnächst</i></td>
  </tr>
  </tr>
  </tbody>
</table>
<br/>

## Ankündigungen {#announcements}

* **Einstellung von REST-API-„access_token“-**: Der `access_token` Abfrageparameter, der zum Authentifizieren von Marketo REST-API-Aufrufen verwendet wird, wird nicht mehr unterstützt und ist nach dem 31. Juli 2026 nicht mehr verfügbar. Alle neuen und vorhandenen Integrationen sollten REST-API-Aufrufe mit dem Header „Authorization“ authentifizieren, [wie hier beschrieben](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Limit für REST-API-Zusammenführung von Leads**: Ab dem 31. Juli 2026 führen Aufrufe, die mehr als 25 IDs im leadIds-Parameter eines Zusammenführungs-Leads-API-Aufrufs enthalten, zu einem 1080-Fehler-Code, und der Aufruf wird übersprungen. Aufträge, die die Zusammenführung von mehr als 25 Datensätzen in einem erfordern, sollten in mehrere Aufträge aufgeteilt werden, um den Erfolg dieser Aufrufe sicherzustellen.

* **Einstellung der SOAP-**: Die Unterstützung für die Marketo SOAP-API endet am 31. Juli 2026. Services, die SOAP-API-Funktionen verwenden, sollten zur [REST-API](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} migriert werden.

* **Statische Listengrößenbeschränkungen für Lead-Aktivitäten abrufen und Lead-Änderungen abrufen**: Ab dem 30. September 2026 geben Aufrufe der Endpunkte „Lead-Aktivitäten abrufen“ und „Lead-Änderungen abrufen“, die den `listId`-Parameter enthalten, einen 1003-Fehler-Code zurück, wenn die statische Zielliste 10.000 oder mehr Leads enthält. Weitere Informationen finden Sie [ „Migrationshandbuch](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"} .
