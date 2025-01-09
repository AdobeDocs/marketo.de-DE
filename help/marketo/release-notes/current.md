---
description: Aktuelle Versionshinweise – Marketo-Dokumente – Produktdokumentation
title: Aktuelle Versionshinweise
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: fa149bb386e98a5b9daa1c7b8933d66b708047c1
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 7%

---

# Versionshinweise: Januar 2025 {#release-notes-jan-25}

Im Folgenden finden Sie alle Funktionen, die in der Version vom Januar 2025 enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage Edition auf die Verfügbarkeit der Funktionen.

Die Versionshinweise speziell für Adobe Dynamic Chat [finden Sie hier](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie von Ihrem Marketo Engage-Support-Mitarbeiter.

## Standardfunktionen des Veröffentlichungszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Veröffentlichungszyklus und werden ab dem 17. **2025 veröffentlicht** wobei die verbleibenden Funktionen in den folgenden Wochen schrittweise bereitgestellt werden. Veröffentlichungsfunktionen und -daten können sich ändern. Überprüfen Sie neben jeder Funktion auf ihren Status.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Funktion</th> 
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
    <tr> 
   <td><strong>Neue E-Mail-Designer</strong>: Erstellen Sie moderne und effiziente E-Mails mit der neuen nativen E-Mail-Designer in Marketo Engage. Greifen Sie auf eine der vordefinierten E-Mail-Vorlagen zu oder erstellen Sie einfach Ihre eigenen. Verwenden Sie dynamische Inhalte und greifen Sie über Adobe Experience Manager Cloud Services auf Bilder zu.</td> 
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Registrierung von Teilnehmern an einer Veranstaltung in interaktiven Webinaren aufheben</strong>: Wenn Sie aus irgendeinem Grund keinen Teilnehmer in Ihrem Webinar haben möchten, können Sie die Registrierung aufheben. Der Workflow entfernt den Registranten sowohl aus dem Marketo-Ereignisprogramm als auch aus Adobe Connect.</td> 
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  <tr> 
   <td><strong>Kampagnen im Archiv deaktivieren</strong>: Deaktivieren Sie aktive Trigger-Kampagnen und brechen Sie alle geplanten Batch-Ausführungen von Kampagnen nach der Archivierung in einem Ordner ab. Da es eine zusätzliche Berechtigungsprüfung für Archivierungsordner gibt, die aktive Trigger enthalten (Kampagne aktivieren und Batch-Kampagne planen), wird diese Funktion mit dieser Version standardmäßig deaktiviert und kann durch Navigieren zu <b>Admin</b> &gt; <b>Schatztruhe</b> in Ihrem Marketo Engage-Abonnement aktiviert werden.</td> 
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Ankündigungen {#announcements}

* **Einstellung von Social**: Am Mittwoch, 31. Juli 2024, begann Marketo Engage mit der Einstellung der folgenden Social-Media-Funktionen im Produkt:

   * Umfragen
   * Social-Schaltfläche
   * Empfehlungsangebot
   * Videofreigabe
   * Gewinnspiele

Ab diesem Zeitpunkt war es den Nutzern nicht mehr möglich, diese Social-Media-Funktionen in Marketo Engage zu erstellen, zu klonen oder einzubetten. Vorhandene soziale Assets funktionieren bis zum 31. Januar 2025 weiterhin. Am 1. Februar 2025 werden soziale Assets nicht mehr funktionieren. In Landingpages eingebettete Social-Media-Funktionen müssen entfernt werden. [Weitere Informationen](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **API-Aktualisierung für Programmmitglieder abrufen**: Wir haben die API [Programmmitglieder abrufen](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/program-members#query){target="_blank"} verbessert, um die Möglichkeit zum Abrufen der Kennung von Programmmitgliedern zu unterstützen. Dies geschieht, indem die ID zur Liste der Felder hinzugefügt wird, die im Feld-Parameter der API-Anfrage angegeben sind.

* **Einstellung von REST-API-„access_token“-**: Der `access_token` Abfrageparameter, der zum Authentifizieren von Marketo REST-API-Aufrufen verwendet wird, wird nicht mehr unterstützt und ist nach dem 30. Juni 2025 nicht mehr verfügbar. Alle neuen und vorhandenen Integrationen sollten REST-API-Aufrufe mit dem Header „Authorization“ authentifizieren [wie hier beschrieben](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* Einstellung der **SOAP-**: Die Unterstützung für die Marketo-SOAP-API endet am 31. Oktober 2025. Services, die SOAP-API-Funktionen verwenden, sollten zur [REST-API“ ](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} werden.
