---
description: Juli 2026 - Versionshinweise zu Marketo - Produktdokumentation
title: Juli 2026 - Versionshinweise
feature: Release Information
source-git-commit: 093bb2edda0a9c70bf45462fc8a67c45bda9b4e1
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 19%

---

# Versionshinweise: Juli 2026 {#release-notes-july-26}

Unten finden Sie alle Funktionen, die in der Version vom 26. Juli enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage Edition auf die Verfügbarkeit der Funktionen.

Die Versionshinweise speziell für Adobe Dynamic Chat [finden Sie hier](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Funktionen aus dem standardmäßigen Veröffentlichungszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Veröffentlichungszyklus und werden ab dem 10. **2026 veröffentlicht** wobei die verbleibenden Funktionen in den folgenden Wochen schrittweise bereitgestellt werden. Funktionen und Veröffentlichungstermine können sich ändern. Überprüfen Sie neben jeder Funktion ihren Status.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
  <tr>
   <td><strong>Marketo-KI-Kenntnisse - Produktwissen</strong>: Produktkenntnisse bieten Ihnen On-Demand-Zugriff auf Marketo-Know-how, ohne die Plattform verlassen zu müssen. Stellen Sie eine Frage in einfacher Sprache, und die Marketo-KI greift auf die offizielle Adobe-Dokumentation zurück, um eine Antwort zu geben.
</td>
   <td>Freigegeben</td>
   <td><a href="https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/marketo-ai/skills/product-knowledge" target="_blank">Produktkenntnisse</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Marketo-KI-Kenntnisse - Leads untersuchen</strong>: Finden Sie heraus, warum eine bestimmte Person/ein Lead einen Meilenstein (wie MQL, Programmqualifikation oder eine Kampagne) nicht erreicht hat, und erhalten Sie eine Klartext-Erklärung, was passiert ist.
</td>
   <td>Freigegeben</td>
   <td><a href="https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/marketo-ai/skills/investigate-leads" target="_blank">Leads untersuchen</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer - </strong>: Sie haben jetzt Zugriff auf einsatzbereite, vollständig strukturierte Inhaltsbausteine, die die E-Mail-Assembly beschleunigen.</td>
   <td>Freigegeben</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/email-modules.md" target="_blank">Verwenden von Modulen in der E-Mail-Designer</a></td>
  </tr>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer - Kontextmenü für Inhalte generieren</strong>: Die Funktionen zum Generieren von Inhalten in der E-Mail-Designer können jetzt über das Kontextmenü (den schwarzen Balken) aufgerufen werden. Wenn Sie beispielsweise Textinhalte auswählen, wird im Kontextmenü das Symbol Inhalt generieren angezeigt, über das Sie Schnellaktionen ausführen können.</td>
   <td><i>Demnächst</i></td>
<td><i>Demnächst</i></td>
  </tr>
  </tr>
  </tbody>
</table>
<br/>



## Ankündigungen {#announcements}

* **Einstellung von REST-API-„access_token“-**: Der `access_token` Abfrageparameter, der zum Authentifizieren von Marketo REST-API-Aufrufen verwendet wird, wird nicht mehr unterstützt und ist nach dem 31. August 2026 nicht mehr verfügbar. Alle neuen und vorhandenen Integrationen sollten REST-API-Aufrufe mit dem Header „Authorization“ authentifizieren, [wie hier beschrieben](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.
* **Limit für REST-API-Zusammenführung von Leads**: Ab dem 31. Juli 2026 führen Aufrufe, die mehr als 25 IDs im leadIds-Parameter eines Zusammenführungs-Leads-API-Aufrufs enthalten, zu einem 1080-Fehler-Code, und der Aufruf wird übersprungen. Aufträge, die die Zusammenführung von mehr als 25 Datensätzen in einem erfordern, sollten in mehrere Aufträge aufgeteilt werden, um den Erfolg dieser Aufrufe sicherzustellen.
* **Einstellung der SOAP-**: Die Unterstützung für die Marketo SOAP-API endet am 31. Juli 2026. Services, die SOAP-API-Funktionen verwenden, sollten zur [REST-API](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} migriert werden.
* **Statische Listengrößenbeschränkungen für Lead-Aktivitäten abrufen und Lead-Änderungen abrufen**: Ab dem 30. September 2026 geben Aufrufe der Endpunkte „Lead-Aktivitäten abrufen“ und „Lead-Änderungen abrufen“, die den `listId`-Parameter enthalten, einen 1003-Fehler-Code zurück, wenn die statische Zielliste 10.000 oder mehr Leads enthält. Weitere Informationen finden Sie [&#x200B; „Migrationshandbuch](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"} .
