---
description: Januar 2025 - Versionshinweise zu Marketo - Produktdokumentation
title: Versionshinweise – Januar 2025
feature: Release Information
exl-id: fd816b9c-9e06-4292-87d6-9fa991c4681f
source-git-commit: 29c1b59c9d2598626f546554a8bdc1b26b9e1590
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 35%

---

# Versionshinweise – Januar 2025 {#release-notes-jan-25}

Im Folgenden finden Sie alle Funktionen, die in der Version vom Januar 2025 enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf die Verfügbarkeit der Funktionen.

Die Versionshinweise speziell für Adobe Dynamic Chat [finden Sie hier](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie vom Marketo Engage-Support.

## Funktionen aus dem standardmäßigen Veröffentlichungszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Veröffentlichungszyklus und werden seit dem **Samstag, 17. Januar 2025 veröffentlicht**, wobei die verbleibenden Funktionen in den folgenden Wochen schrittweise bereitgestellt werden. Veröffentlichungsfunktionen und -daten können sich ändern. Überprüfen Sie neben jeder Funktion ihren Status.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
    <tr>
   <td><strong>Neue E-Mail-Designer</strong>: Erstellen Sie moderne und effiziente E-Mails mit der neuen nativen E-Mail-Designer in Marketo Engage. Greifen Sie auf eine der vordefinierten E-Mail-Vorlagen zu oder erstellen Sie einfach Ihre eigenen. Verwenden Sie dynamische Inhalte und greifen Sie über Adobe Experience Manager Cloud Services auf Bilder zu. Verwenden Sie die Funktion Content Accelerator Gen-AI , um innovative und leistungsstarke E-Mails in großem Umfang zu erstellen.
   <p><img src="assets/note-icon.png" alt="Notizensymbol"> HINWEIS: Um auf den neuen E-Mail-Designer zugreifen zu können, muss Ihr Marketo Engage-Abonnement auf das <a href="https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview">Adobe Identity Management System (IMS) migriert </a>. Wenn Ihre Anfrage noch nicht bearbeitet wurde und Sie eine Beschleunigung anfordern möchten, wenden Sie sich bitte an das Adobe Account Team (Ihren Account Manager) oder an den <a href="https://nation.marketo.com/t5/support/ct-p/Support">Marketo Support</a>. Wenden Sie sich an das Adobe-Account-Team , um auf die Funktion Content Accelerator Gen-AI zugreifen zu können.</td>
   <td>Versandt</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/overview.md">E-Mail-Designer – Überblick</a></td>
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

* **Einstellung von Social**: Am Mittwoch, 31. Juli 2024, begann Marketo Engage mit der Einstellung der folgenden Social-Media-Funktionen innerhalb des Produkts:

   * Umfragen
   * Social-Schaltfläche
   * Empfehlungsangebot
   * Videofreigabe
   * Gewinnspiele

Ab diesem Zeitpunkt waren Benutzende nicht mehr in der Lage, diese Social-Media-Funktionen in Marketo Engage zu erstellen, zu klonen oder einzubetten. Vorhandene soziale Assets funktionieren bis zum 31. Januar 2025 weiterhin. Am 1. Februar 2025 werden soziale Assets nicht mehr funktionieren. In Landingpages eingebettete Social-Media-Funktionen müssen entfernt werden. [Weitere Informationen](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **API-Aktualisierung für Programmmitglieder abrufen**: Wir haben die API [Programmmitglieder abrufen](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/program-members#query){target="_blank"} verbessert, um die Möglichkeit zum Abrufen der Kennung von Programmmitgliedern zu unterstützen. Dies geschieht, indem die ID zur Liste der Felder hinzugefügt wird, die im Feld-Parameter der API-Anfrage angegeben sind.

* **Einstellung des Parameters „access_token“ der REST-API**: Der Abfrageparameter `access_token`, der zum Authentifizieren von Marketo REST-API-Aufrufen verwendet wird, wird nicht mehr unterstützt und wird nach dem 31. Oktober 2025 nicht mehr verfügbar sein. Alle neuen und vorhandenen Integrationen sollten REST-API-Aufrufe mit dem Header „Authorization“ authentifizieren, [wie hier beschrieben](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Abschaffung der SOAP-API**: Die Unterstützung für die Marketo SOAP-API endet am 31. Oktober 2025. Services, die SOAP-API-Funktionen verwenden, sollten zur [REST-API](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} migriert werden.
