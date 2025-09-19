---
description: Aktuelle Versionshinweise – Marketo-Dokumente – Produktdokumentation
title: Aktuelle Versionshinweise
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 6d09e0f684844d7d2ced6205d7becde90ffcd7c7
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 60%

---

# Versionshinweise – September 2025 {#release-notes-sep-25}

Im Folgenden finden Sie alle Funktionen, die in der Version vom September 2025 enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf die Verfügbarkeit der Funktionen.

Die Versionshinweise speziell für Adobe Dynamic Chat [finden Sie hier](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie vom Marketo Engage-Support.

## Funktionen aus dem standardmäßigen Veröffentlichungszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Veröffentlichungszyklus und werden seit dem **Samstag, 19. September 2025** veröffentlicht, wobei die verbleibenden Funktionen in den folgenden Wochen schrittweise bereitgestellt werden. Veröffentlichungsfunktionen und -daten können sich ändern. Überprüfen Sie neben jeder Funktion ihren Status.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
  <tr>
   <td><strong>Bindung von Webinar-Aktivitäten auf Anfrage</strong>: Benutzende interaktiver Webinare haben jetzt für mehr als 30 Tage verfügbare On-Demand-Dashboard-Daten für Webinare (zuvor waren es nur bis zu 30 Tage ab dem Tag des Webinars).</td>
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer Collaboration - Workflow für Content-</strong>: Sie können jetzt mit Ihren Marketo-Kollegen in einem E-Mail-Asset zusammenarbeiten und Kommentare abgeben. Tag-Team-Mitglieder (Marketo-Benutzer mit entsprechenden Asset-Berechtigungen) und sie erhalten eine E-Mail- oder Push-Benachrichtigung.</td>
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer - Berechtigungen für KI-</strong>: Marketo-Administratoren können bestimmten Benutzenden Zugriff auf GenAI-Funktionen gewähren.</td>
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer - Dunkelmodus</strong>: Sie können jetzt den Dunkelmodus verwenden, der es unterstützenden E-Mail-Clients und Apps ermöglicht, E-Mails mit dunkleren Hintergründen und helleren Farben für Text, Schaltflächen und andere Benutzeroberflächenelemente anzuzeigen.</td>
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer - </strong>: Bei einigen Benutzenden traten Umleitungsprobleme mit URLs für E-Mails auf, die mit der neuen Designer erstellt wurden (z. B. funktionierte das direkte Einfügen der URLs oder das Lesezeichen für E-Mail-Assets nicht immer). Dieses Problem wurde behoben. Darüber hinaus werden Links zu E-Mail<b>Assets von </b>E-Mail-Vorlagen<b> &gt; Details</b> &gt; <b>Verwendet von</b> zum entsprechenden E-Mail-Asset umgeleitet.</td>
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Ankündigungen {#announcements}

* **Zurück zur Velocity-Skripterstellung in der neuen E-Mail-Designer**: Adobe Marketo Engage hat im vergangenen Juni eine Funktion namens _Bedingter Inhalt_ für die neue E-Mail-Designer veröffentlicht. Die Funktion basiert auf Handlebar-Skripterstellung anstelle von Velocity-Skripterstellung, in dem Bemühen, Ihren dynamischen Inhalten etwas mehr Flexibilität zu bieten. Aber als wir herausfanden, dass es dazu führte, dass einige Token falsch aufgelöst wurden, entschieden wir uns, es vorübergehend zu deaktivieren. [Weitere Informationen](https://nation.marketo.com/t5/product-blogs/update-on-email-scripting-in-the-new-email-designer/ba-p/358179){target="_blank"}

* **Abschaffung der Marketo Engage Identity**: Im August 2025 beginnt Adobe mit der schrittweisen Einstellung der Unterstützung für Marketo Engage Identity (Anmeldung über `login.marketo.com`). Um eine Unterbrechung des Zugriffs auf Marketo Engage zu verhindern, müssen Sie bis spätestens 30. September 2025 zu [Adobe Identity](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} wechseln.

   * _Abschaffung von IP-Einschränkungen_: Die Unterstützung für das [Einschränken von Marketo-Anmeldungen auf Grundlage der IP](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} endete am 30. Juli 2025. Die Funktion bleibt funktionsfähig, bis die Umstellung auf Adobe Identity abgeschlossen ist. Eine neue standortbasierte Zugriffssteuerungsfunktion für Adobe Identity in der Adobe Admin Console ist demnächst verfügbar.

   * _Abschaffung von Single Sign-on (SSO)_: Die Unterstützung für [Marketo Identity SSO](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} endete am 30. Juli 2025. Die Funktion bleibt funktionsfähig, bis die Umstellung auf Adobe Identity abgeschlossen ist. Das Single Sign-On für Adobe Identity in der Adobe Admin Console muss separat konfiguriert werden. Informationen zu den Einrichtungsschritten finden Sie unter [Einrichten von Identitäten und Single Sign-On](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html){target="_blank"}.

* **Einstellung der Funktion _An Freund/Freundin weiterleiten_**: Am 29. September 2025 wird die Funktion _An Freund/Freundin weiterleiten_ in E-Mails in Marketo Engage 2.0 (dem alten E-Mail-Editor) für alle Abonnements vollständig eingestellt. Dies betrifft das Token „An Freund/Freundin weiterleiten“ und die Links „An Freund/Freundin weiterleiten“ in E-Mails, die bereits mit dem Token gesendet wurden oder gesendet werden. [Weitere Informationen](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Einstellung des Parameters „access_token“ der REST-API**: Der Abfrageparameter `access_token`, der zum Authentifizieren von Marketo REST-API-Aufrufen verwendet wird, wird nicht mehr unterstützt und wird nach dem 31. Oktober 2025 nicht mehr verfügbar sein. Alle neuen und vorhandenen Integrationen sollten REST-API-Aufrufe mit dem Header „Authorization“ authentifizieren, [wie hier beschrieben](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Abschaffung der SOAP-API**: Die Unterstützung für die Marketo SOAP-API endet am 31. Oktober 2025. Services, die SOAP-API-Funktionen verwenden, sollten zur [REST-API](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} migriert werden.
