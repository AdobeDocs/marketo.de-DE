---
description: Aktuelle Versionshinweise – Marketo-Dokumente – Produktdokumentation
title: Aktuelle Versionshinweise
hide: true
hidefromtoc: true
feature: Release Information
exl-id: 0ca5e844-c30b-4c86-a23d-d8f2c1bdddf5
source-git-commit: f806c0984cf221bd88fdf50013a8f1d2911b5d86
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 62%

---

# Versionshinweise – Januar 2026 {#release-notes-jan-26}

Im Folgenden finden Sie alle Funktionen, die in der Version vom Januar 2026 enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf die Verfügbarkeit der Funktionen.

Die Versionshinweise speziell für Adobe Dynamic Chat [finden Sie hier](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie vom Marketo Engage-Support.

## Funktionen aus dem standardmäßigen Veröffentlichungszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Veröffentlichungszyklus und werden ab dem **Samstag, 30. Januar 2026** veröffentlicht, wobei die verbleibenden Funktionen in den folgenden Wochen schrittweise bereitgestellt werden. Veröffentlichungsfunktionen und -daten können sich ändern. Überprüfen Sie neben jeder Funktion ihren Status.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
  <tr>
   <td><strong>FEATURE TITLE</strong>: Beschreibung der Funktionen.</td>
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>FEATURE TITLE</strong>: Beschreibung der Funktionen.</td>
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>FEATURE TITLE</strong>: Beschreibung der Funktionen.</td>
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Adobe Connect-Funktionen {#adobe-connect-features}

Die Funktion [Interaktive Webinare](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/interactive-webinars-overview){target="_blank"} von Marketo Engage basiert auf Adobe Connect und erweitert das Personenmanagement und Kampagnen mit Ereignisdaten und verbessert die Personenqualität. Im Folgenden finden Sie einige aktuelle Adobe Connect-Versionen, die sich direkt auf Benutzer von interaktiven Webinaren auswirken.

* **Umfrage-Pod**: Adobe Connect 12.11 führt einen neuen Umfrage-Pod ein, mit dem Hosts strukturierte Feedback-Formulare direkt innerhalb einer Live-Sitzung entwerfen und bereitstellen können.

* **Ressourcen-Pod**: Der neue Ressourcen-Pod ersetzt die vorherigen Dateien und Web-Link-Pods und bietet eine einzige, einheitliche Möglichkeit, Ressourcen während Live-Sitzungen freizugeben.

* **Verbesserte Raumschnittstelle**: Adobe Connect 12.11 führt eine aktualisierte und modernere Raumschnittstelle ein, die auf Adobes neuestem Spectrum 2-Design-Framework basiert und an die Bildsprache angepasst ist, die in anderen Adobe-Produkten wie Creative Cloud und Experience Cloud verwendet wird.

Ausführliche Informationen finden Sie in den Versionshinweisen zu [Adobe Connect 12.11](https://helpx.adobe.com/adobe-connect/release-note/adobe-connect-12-11-release-notes.html){target="_blank"}.

## Ankündigungen {#announcements}

* **Einstellung des Parameters „access_token“ der REST-API**: Der Abfrageparameter `access_token`, der zum Authentifizieren von Marketo REST-API-Aufrufen verwendet wird, wird nicht mehr unterstützt und wird nach dem Mittwoch, 31. März 2026 nicht mehr verfügbar sein. Alle neuen und vorhandenen Integrationen sollten REST-API-Aufrufe mit dem Header „Authorization“ authentifizieren, [wie hier beschrieben](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Abschaffung der SOAP-API**: Die Unterstützung für die Marketo SOAP-API endet am Mittwoch, 31. März 2026. Services, die SOAP-API-Funktionen verwenden, sollten zur [REST-API](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} migriert werden.

* **Einstellung der Marketo Engage-Identität**:

   * _Abschaffung von IP-Einschränkungen_: Die Unterstützung für das [Einschränken von Marketo-Anmeldungen auf Grundlage der IP](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} endete am 30. Juli 2025. Die Funktion bleibt funktionsfähig, bis die Umstellung auf Adobe Identity abgeschlossen ist. Eine neue standortbasierte Zugriffssteuerungsfunktion für Adobe Identity in der Adobe Admin Console ist demnächst verfügbar.

   * _Abschaffung von Single Sign-on (SSO)_: Die Unterstützung für [Marketo Identity SSO](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} endete am 30. Juli 2025. Die Funktion bleibt funktionsfähig, bis die Umstellung auf Adobe Identity abgeschlossen ist. Das Single Sign-On für Adobe Identity in der Adobe Admin Console muss separat konfiguriert werden. Informationen zu den Einrichtungsschritten finden Sie unter [Einrichten von Identitäten und Single Sign-On](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html){target="_blank"}.
