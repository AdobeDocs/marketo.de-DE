---
description: Aktuelle Versionshinweise – Marketo-Dokumente – Produktdokumentation
title: Aktuelle Versionshinweise
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 0d2416651da183460ad1f60ff5d566cbfc7abd12
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 10%

---

# April 2024 - Versionshinweise {#release-notes-apr-24}

Unten finden Sie alle Funktionen der Version vom 24. April. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf Funktionsverfügbarkeit.

Die Versionshinweise speziell für Adobe Dynamic Chat [finden Sie hier .](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png)) sind kostenpflichtige Add-ons. Wenden Sie sich an Ihren Marketo Engage-Support-Mitarbeiter, um mehr zu erfahren.

## Standardfunktionen des Versionszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den Standard-Versionszyklus und werden ab der Veröffentlichung auf **26. April 2024**, mit einer stufenweisen Einführung der verbleibenden Funktionen in den darauffolgenden Wochen. Die Veröffentlichungsfunktionen und -daten können sich ändern. Bitte überprüfen Sie neben den einzelnen Funktionen nach ihrem Status.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Funktion</th> 
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
     <tr> 
   <td><strong>Verbesserungen bei interaktiven Webinaren</strong>: Hosts und Moderatoren können jetzt einen Webinartitel hinzufügen, einen Raum umbenennen und Interaktionsdaten nach der Ereignisbereitstellung manuell synchronisieren.</td> 
   <td>Versendet</td>
   <td><li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/create-an-interactive-webinar.md">Erstellen eines interaktiven Webinars</a></li>
   <li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/event-workflows.md#manual-sync">Manuelle Synchronisierung</a></li></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Verbesserungen am Audit-Protokoll</strong>: Im Audit-Protokoll können jetzt neue Aktionstypen für Änderungen im Feldmanagement, Änderungen an Benutzern und Rollen sowie die Anzahl der aus Listen und Smart-Listen exportierten Personen erfasst werden.</td> 
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Neue Berechtigungen für Benutzer und Rollen</strong>: Es sind neue Berechtigungen verfügbar, die Benutzern detaillierteren Zugriff auf Marketo Engage bieten. Kontrollteile von Admin, die noch nicht erfasst wurden, wie z. B. neue Erlebnisse und vorausschauende Zielgruppen, teilen Berechtigungen auf, um Zugriff auf das Asset-Audit-Protokoll und das Admin Audit-Protokoll separat zu gewähren, und verwenden neue Berechtigungen zum Erstellen und Verschieben für Assets und Ordner, um schreibgeschützte Benutzer daran zu hindern, Änderungen vorzunehmen. 
   <p>Während die neuen Berechtigungen ab dem 26. April in Ihrer Marketo Engage-Instanz erscheinen, sind sie zunächst passiv und werden später in diesem Quartal verfügbar sein.
   <li>Zugriff auf Adobe Experience Manager</li>
   <li>Adobe-Organisationszuordnung aufrufen</li>
   <li>Auf Admin Audit-Protokoll zugreifen</li>
   <li>Asset-Audit-Protokoll aufrufen</li>
   <li>Auf neues Erlebnis zugreifen</li>
   <li>Zugriff auf vorausschauende Zielgruppen</li>
   <li>Bericht erstellen</li>
   <li>Liste erstellen</li>
   <li>Kampagnenaktivität exportieren</li>
   </td> 
   <td>Versendet</td>
   <td><a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md">Beschreibung der Rollenberechtigungen</a></td>
  </tr>
 </tbody> 
</table>
<br/>

## Ankündigungen {#announcements}

* **API-Update für Aktivitäten**: Am 26. April fügen wir Web- und E-Mail-basierten Aktivitäten mehrere neue Attribute hinzu, die zurückgegeben werden, wenn Sie Aktivitäten mit der [MARKETO REST API](https://developers.marketo.com/rest-api/lead-database/activities/){target="_blank"}. The activities listed below will now include Browser, Platform, Device, and User Agent attributes. Call the [Get Activity Types](https://developers.marketo.com/rest-api/endpoint-reference/lead-database-endpoint-reference/#!/Activities/getAllActivityTypesUsingGET){target="_blank"} -Endpunkt, um die Attributdetails für jede Aktivität zu überprüfen.

**Internetbasierte Aktivitäten**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:30%">Aktivität</th> 
   <th style="width:70%">Neu hinzugefügte Attribute</th>
   </tr>
  <tr> 
   <td>Visit Webpage</td> 
   <td>Browser, Plattform, Gerät</td>
  </tr>
   <tr> 
   <td>Formular ausfüllen</td> 
   <td>Browser, Plattform, Gerät</td>
  </tr>
  <tr> 
   <td>Auf Link klicken</td> 
   <td>Browser, Plattform, Gerät</td>
  </tr>
 </tbody> 
</table>

**E-Mail-basierte Aktivitäten**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:30%">Aktivität</th> 
   <th style="width:70%">Neu hinzugefügte Attribute</th>
  </tr>
   <tr> 
   <td>E-Mail senden</td> 
   <td>Browser, Plattform, Gerät, Benutzeragent</td>
  </tr>
   </tr>
  <tr> 
   <td>E-Mail übermittelt</td> 
   <td>Browser, Plattform, Gerät, Benutzeragent</td>
  </tr>
   <tr> 
   <td>E-Mail war aufgrund eines Bounce-Ereignisses unzustellbar</td> 
   <td>Browser, Plattform, Gerät, Benutzeragent</td>
  </tr>
  <tr> 
   <td>E-Mail abbestellen</td> 
   <td>Browser, Plattform, Gerät</td>
  </tr>
  <tr> 
   <td>E-Mail öffnen</td> 
   <td>Browser</td>
  </tr>
   <tr> 
   <td>Klicken auf E-Mail</td> 
   <td>Browser</td>
  </tr>
  <tr> 
   <td>E-Mail war aufgrund eines Soft Bounce-Ereignisses unzustellbar</td> 
   <td>Browser, Plattform, Gerät, Benutzeragent</td>
  </tr>
 </tbody> 
</table>
