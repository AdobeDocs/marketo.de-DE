---
description: April 2024 - Versionshinweise zu Marketo - Produktdokumentation
title: Versionshinweise – April 2024
feature: Release Information
exl-id: d87474f8-fc47-407b-bc97-e343b56c1f8f
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 31%

---

# Versionshinweise – April 2024 {#release-notes-apr-24}

Unten finden Sie alle Funktionen, die in der Version vom April 2024 enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf die Verfügbarkeit der Funktionen.

Die Versionshinweise speziell für Adobe Dynamic Chat [finden Sie hier](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie vom Marketo Engage-Support.

## Funktionen aus dem standardmäßigen Veröffentlichungszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Veröffentlichungszyklus und werden seit dem **Samstag, 26. April 2024** veröffentlicht, wobei die verbleibenden Funktionen in den folgenden Wochen schrittweise bereitgestellt werden. Veröffentlichungsfunktionen und -daten können sich ändern. Überprüfen Sie neben jeder Funktion ihren Status.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
     <tr>
   <td><strong>Verbesserungen bei interaktiven Webinaren</strong>: Sie können jetzt Hosts und Moderatoren die Möglichkeit geben, einen Webinar-Titel hinzuzufügen, einen Raum umzubenennen und Interaktionsdaten nach dem Versand des Ereignisses manuell zu synchronisieren.</td>
   <td>Versandt</td>
   <td><li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/create-an-interactive-webinar.md">Erstellen eines interaktiven Webinars</a></li>
   <li><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/event-workflows.md#manual-sync">Manuelle Synchronisierung</a></li></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>Verbesserungen am Audit-Protokoll</strong>:
   Neue Aktionstypen können jetzt im Audit-Protokoll erfasst werden. Dies betrifft Änderungen im Feld-Management, Änderungen an Benutzenden und Rollen sowie die Anzahl der aus Listen und Smart Lists exportierten Personen.</td>
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
    <tr>
   <td><strong>Berechtigungen für neue Benutzer und Rollen</strong>: Neue Berechtigungen sind verfügbar, die Benutzenden einen granulareren Zugriff auf Marketo Engage bieten. Steuern Sie Teile von Admin, die zuvor nicht kategorisiert wurden, z. B. „Neues Erlebnis“ und „Prädiktive Zielgruppen“, teilen Sie die Berechtigungen auf, um Zugriff auf das Asset-Audit-Protokoll und das Admin-Audit-Protokoll separat zu gewähren, und verwenden Sie neue Berechtigungen zum Erstellen und Verschieben von Assets und Ordnern, um zu verhindern, dass schreibgeschützte Benutzer Änderungen vornehmen.
   <p>Die neuen Berechtigungen werden zwar ab dem 26. April in Ihrer Marketo Engage-Instanz angezeigt, sind aber vorerst passiv und werden im Laufe dieses Quartals verfügbar sein.
   <li>Zugriff auf Adobe Experience Manager</li>
   <li>Zugriff auf die Adobe-Organisationszuordnung</li>
   <li>Zugriff auf das Admin-Audit-Protokoll</li>
   <li>Zugriff auf das Asset-Audit-Protokoll</li>
   <li>Neues Erlebnis</li>
   <li>Zugriff auf prädiktive Zielgruppen</li>
   <li>Bericht erstellen</li>
   <li>Liste erstellen</li>
   <li>Kampagnenaktivität exportieren</li>
   </td>
   <td>Versandt</td>
   <td><a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md">Beschreibungen der Rollenberechtigungen</a></td>
  </tr>
 </tbody>
</table>
<br/>

## Ankündigungen {#announcements}

* **Aktivitäts-API-Aktualisierung**: Am 26. April fügen wir mehrere neue Attribute zu Web- und E-Mail-basierten Aktivitäten hinzu, die zurückgegeben werden, wenn Sie Aktivitäten mit der [Marketo-REST-API abrufen](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Activities){target="_blank"}. Die unten aufgeführten Aktivitäten umfassen jetzt Browser-, Plattform-, Geräte- und Benutzeragenten-Attribute. Rufen Sie den Endpunkt [Aktivitätstypen abrufen](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Activities/operation/getAllActivityTypesUsingGET){target="_blank"} auf, um Attributdetails für jede Aktivität zu überprüfen.

**Web-basierte Aktivitäten**

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
   <td>Senden von E-Mail</td>
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
   <td>Auf E-Mail klicken</td>
   <td>Browser</td>
  </tr>
  <tr>
   <td>E-Mail war aufgrund eines Soft Bounce-Ereignisses unzustellbar</td>
   <td>Browser, Plattform, Gerät, Benutzeragent</td>
  </tr>
 </tbody>
</table>
