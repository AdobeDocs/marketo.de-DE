---
description: Aktuelle Versionshinweise – Marketo-Dokumente – Produktdokumentation
title: Aktuelle Versionshinweise
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
TQID: https://experienceleague.adobe.com/QJFy7PeGXlvS3jcJGcZJROlc8c1UvphO-TOOwPUQeX8
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
    internal-label: Forms
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: f71e690b-4480-4b67-9ef5-88f42f9cdfdb
    internal-label: Resources
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
    internal-label: Templates
subfeature_v2:
  - id: c942e9f6-ed06-481a-abdd-1195363d1452
    internal-label: Dynamic Chat
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: edeb795f12082fab9c72b0ff4305f3db90aa4c46
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 18%
---
# Versionshinweise: September 2026 {#release-notes-sep-26}

Im Folgenden finden Sie alle Funktionen, die in der Version vom September 2026 enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage Edition auf die Verfügbarkeit der Funktionen.

Die Versionshinweise speziell für Adobe Dynamic Chat [finden Sie hier](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Funktionen aus dem standardmäßigen Veröffentlichungszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Veröffentlichungszyklus und werden ab dem 25. **2026 veröffentlicht** wobei die verbleibenden Funktionen in den folgenden Wochen schrittweise bereitgestellt werden. Funktionen und Veröffentlichungstermine können sich ändern. Überprüfen Sie neben jeder Funktion ihren Status.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
  <tr>
   <td><strong>Neue Benutzeroberfläche von Marketo Engage</strong>: Die Benutzeroberfläche von Marketo Engage hat ein aktualisiertes Design, einschließlich aktualisierter Menüs, Symbole und Layouts, für ein saubereres, moderneres Erlebnis. Dies ist nur eine visuelle Aktualisierung. Vorhandene Funktionen oder Workflows sind davon nicht betroffen. <i>Die Möglichkeit, die klassische Benutzeroberfläche auszuwählen, wird über die Version vom Januar 2027 verfügbar sein</i>.
</td>
   <td>Allgemeine Verfügbarkeit bis Ende September</td>
   <td><i>Nicht zutreffend</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Partition beim Importieren auswählen</strong>: Sie können jetzt beim Importieren von Personendatensätzen in Umgebungen, in denen Arbeitsbereiche und Partitionen aktiviert sind, aus der Liste der Partitionen des lokalen Arbeitsbereichs auswählen.</td>
   <td><i>Demnächst</i></td>
   <td><i>Demnächst</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Sofortiger Warnhinweis bei CRM-Synchronisierung</strong>: Benutzer, die CRM-Benachrichtigungen abonniert haben, erhalten eine sofortige Benachrichtigung, wenn sich der aktivierte Status ihrer nativen CRM-Synchronisierung ändert, was Admins eine größere Sichtbarkeit ihres CRM-Synchronisierungsstatus gibt.</td>
   <td><i>Demnächst</i></td>
   <td><i>Demnächst</i></td>
  </tr>
   <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Self-Service-Flussschritte - Erhöhtes Callback-Timeout</strong>: Der Zeitraum für das Callback-Timeout für Self-Service-Flussschritte wird von einer Stunde auf vier Stunden erhöht. Auf Ihrer Seite ist keine Aktion erforderlich.</td>
   <td><i>Demnächst</i></td>
   <td><i>Demnächst</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail Designer - </strong>: Sie können jetzt den Inhaltstyp „Tabelle“ per Drag-and-Drop in Ihre E-Mail ziehen, wobei die Anzahl der Spalten und Zeilen festgelegt werden kann.</td>
   <td><i>Demnächst</i></td>
   <td><i>Demnächst</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Ankündigungen {#announcements}

* **API-Namensbeschränkungen für benutzerdefinierte Aktivitätsattribute**: API-Namen für benutzerdefinierte Aktivitätsattribute, die über die API oder die Benutzeroberfläche erstellt wurden, dürfen jetzt nur alphanumerische Zeichen und Unterstriche enthalten und müssen mit einem alphanumerischen Zeichen beginnen.

* **Statische Listengrößenbeschränkungen für Lead-Aktivitäten abrufen und Lead-Änderungen abrufen**: Ab dem 30. September 2026 schlagen Aufrufe der Endpunkte „Lead-Aktivitäten abrufen“ oder „Lead-Änderungen abrufen“, die den `listId`-Parameter enthalten, mit einem 1003-Fehler-Code fehl (was anzeigt, dass die statische Zielliste zu viele Datensätze enthält), wenn die Ziellisten 10.000 oder mehr Leads enthalten. Weitere Informationen finden Sie [Migrationshandbuch](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/migration){target="_blank"} .

* **Einstellung von REST-API-„access_token“-**: Der `access_token` Abfrageparameter, der zum Authentifizieren von Marketo REST-API-Aufrufen verwendet wird, wird seit dem 31. August 2026 nicht mehr unterstützt. Alle neuen und vorhandenen Integrationen sollten REST-API-Aufrufe mit dem Header „Authorization“ authentifizieren, [wie hier beschrieben](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **REST-API Kampagnenausführungs-ID**: Unter bestimmten Umständen wurde der Wert der Kampagnenausführungs-ID einer Aktivität manchmal mit falscher Formatierung zwischen zwei Paaren von Anführungszeichen zurückgegeben (z. B. `"campaignRunId": ""102938""`).<br/>Ab der August-Version wird dieser Wert immer im richtigen numerischen Format (`"campaignRunId": 102938`) zurückgegeben.

* **Einstellung der Erfassung von Bildern aus dem Web**: Um den modernen Best Practices für Sicherheit und Datenschutz zu entsprechen, wird die Funktion [Abrufen von Bildern aus ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/images-and-files/grab-the-images-from-a-web-page){target="_blank"}Web) ab der Oktober-Version eingestellt.
