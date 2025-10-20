---
description: Aktuelle Versionshinweise – Marketo-Dokumente – Produktdokumentation
title: Aktuelle Versionshinweise
hide: true
hidefromtoc: true
feature: Release Information
exl-id: 0ca5e844-c30b-4c86-a23d-d8f2c1bdddf5
source-git-commit: 7234082102356fc05c760f359ef19ca8cff375b5
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 86%

---

# Versionshinweise – Oktober 2025 {#release-notes-oct-25}

Im Folgenden finden Sie alle Funktionen, die in der Version vom Oktober 2025 enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf die Verfügbarkeit der Funktionen.

Die Versionshinweise speziell für Adobe Dynamic Chat [finden Sie hier](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie vom Marketo Engage-Support.

## Funktionen aus dem standardmäßigen Veröffentlichungszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Veröffentlichungszyklus und werden seit dem **Samstag, 31. Oktober 2025** veröffentlicht, wobei die verbleibenden Funktionen in den folgenden Wochen schrittweise bereitgestellt werden. Veröffentlichungsfunktionen und -daten können sich ändern. Überprüfen Sie neben jeder Funktion ihren Status.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
  <tr>
   <td><strong>TITLE</strong>: Text</td>
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>TITLE</strong>: Text</td>
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>TITLE</strong>: Text</td>
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>TITLE</strong>: Text</td>
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
 <tr>
   <td><strong>TITLE</strong>: Text</td>
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr>
  </tbody>
</table>
<br/>

## Ankündigungen {#announcements}

* **Einstellung der REST-API mit doppelten Schrägstrichen**: Am 16. September 2025 wurde Adobe auf eine modernere Hosting-Infrastruktur für REST-API-URLs umgestellt, die neuere Technologien nutzt und so Sicherheit und Skalierbarkeit bietet. Wenn Ihr Abonnement APIs mit einem doppelten Schrägstrich (//) in der URL verwendet hat, lesen Sie bitte [diesen Beitrag von Nation](https://nation.marketo.com/t5/product-blogs/rest-api-double-slash-deprecation/ba-p/358616){target="_blank"} für die nächsten Schritte.

* **Zurück zur Geschwindigkeits-Skripterstellung im neuen E-Mail-Designer**: Adobe Marketo Engage hat im vergangenen Juni für den neuen E-Mail-Designer eine Funktion namens _Bedingter Inhalt_ veröffentlicht. Die Funktion basierte auf Handlebar-Skripterstellung anstelle von Geschwindigkeits-Skripterstellung. Das war ein Bemühen, Ihren dynamischen Inhalten etwas mehr Flexibilität zu verleihen. Als wir jedoch erkannten, dass dadurch manche Token falsch aufgelöst werden, entschieden wir, die Funktion vorübergehend zu deaktivieren. [Weitere Informationen](https://nation.marketo.com/t5/product-blogs/update-on-email-scripting-in-the-new-email-designer/ba-p/358179){target="_blank"}

* **Abschaffung der Marketo Engage Identity**: Im August 2025 beginnt Adobe mit der schrittweisen Einstellung der Unterstützung für Marketo Engage Identity (Anmeldung über `login.marketo.com`). Um eine Unterbrechung des Zugriffs auf Marketo Engage zu verhindern, müssen Sie bis spätestens 30. September 2025 zu [Adobe Identity](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} wechseln.

   * _Abschaffung von IP-Einschränkungen_: Die Unterstützung für das [Einschränken von Marketo-Anmeldungen auf Grundlage der IP](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} endete am 30. Juli 2025. Die Funktion bleibt funktionsfähig, bis die Umstellung auf Adobe Identity abgeschlossen ist. Eine neue standortbasierte Zugriffssteuerungsfunktion für Adobe Identity in der Adobe Admin Console ist demnächst verfügbar.

   * _Abschaffung von Single Sign-on (SSO)_: Die Unterstützung für [Marketo Identity SSO](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} endete am 30. Juli 2025. Die Funktion bleibt funktionsfähig, bis die Umstellung auf Adobe Identity abgeschlossen ist. Das Single Sign-On für Adobe Identity in der Adobe Admin Console muss separat konfiguriert werden. Informationen zu den Einrichtungsschritten finden Sie unter [Einrichten von Identitäten und Single Sign-On](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html){target="_blank"}.

* **Einstellung der Funktion _An Freund/Freundin weiterleiten_**: Am 29. September 2025 wird die Funktion _An Freund/Freundin weiterleiten_ in E-Mails in Marketo Engage 2.0 (dem alten E-Mail-Editor) für alle Abonnements vollständig eingestellt. Dies betrifft das Token „An Freund/Freundin weiterleiten“ und die Links „An Freund/Freundin weiterleiten“ in E-Mails, die bereits mit dem Token gesendet wurden oder gesendet werden. [Weitere Informationen](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Einstellung des Parameters „access_token“ der REST-API**: Der Abfrageparameter `access_token`, der zum Authentifizieren von Marketo REST-API-Aufrufen verwendet wird, wird nicht mehr unterstützt und wird nach dem 31. Januar 2026 nicht mehr verfügbar sein. Alle neuen und vorhandenen Integrationen sollten REST-API-Aufrufe mit dem Header „Authorization“ authentifizieren, [wie hier beschrieben](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Abschaffung der SOAP-API**: Die Unterstützung für die Marketo SOAP-API endet am 31. Januar 2026. Services, die SOAP-API-Funktionen verwenden, sollten zur [REST-API](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} migriert werden.
