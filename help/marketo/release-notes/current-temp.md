---
description: Aktuelle Versionshinweise – Marketo-Dokumente – Produktdokumentation
title: Aktuelle Versionshinweise
hide: true
hidefromtoc: true
feature: Release Information
exl-id: 0ca5e844-c30b-4c86-a23d-d8f2c1bdddf5
source-git-commit: 95dda7d6e09f0e64fbce8e5bd39613f10ebde382
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 51%

---

# Versionshinweise – September 2025 {#release-notes-sep-25}

Im Folgenden finden Sie alle Funktionen, die in der Version vom September 2025 enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf die Verfügbarkeit der Funktionen.

Die Versionshinweise speziell für Adobe Dynamic Chat [finden Sie hier](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie vom Marketo Engage-Support.

## Funktionen aus dem standardmäßigen Veröffentlichungszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Veröffentlichungszyklus und werden seit dem **Samstag, 19. September 2025 veröffentlicht**, wobei die verbleibenden Funktionen in den folgenden Wochen schrittweise bereitgestellt werden. Veröffentlichungsfunktionen und -daten können sich ändern. Überprüfen Sie neben jeder Funktion ihren Status.

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
  </tbody>
</table>
<br/>

## Ankündigungen {#announcements}

* **Zurück zur Velocity-Skripterstellung in der neuen E-Mail-Designer**: Adobe Marketo Engage hat im vergangenen Juni eine Funktion namens _Bedingter Inhalt_ für die neue E-Mail-Designer veröffentlicht. Die Funktion basiert auf Handlebar-Skripterstellung anstelle von Velocity-Skripterstellung, in dem Bemühen, Ihren dynamischen Inhalten etwas mehr Flexibilität zu bieten. Aber als wir herausfanden, dass es dazu führte, dass einige Token falsch aufgelöst wurden, entschieden wir uns, es vorübergehend zu deaktivieren. [Weitere Informationen](https://nation.marketo.com/t5/product-blogs/update-on-email-scripting-in-the-new-email-designer/ba-p/358179){target="_blank"}

* **Einstellung der Marketo Engage Identity**: Im August 2025 begann Adobe, die Unterstützung für Marketo Engage Identity auslaufen zu lassen (Anmeldung über `login.marketo.com`). Um eine Unterbrechung des Zugriffs auf Marketo Engage zu verhindern, müssen Sie bis spätestens 30. September 2025 zu [Adobe Identity](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} wechseln.

   * _Einstellung von IP-_: Die Unterstützung für [Einschränken von Marketo-Anmeldungen auf der Grundlage von IP](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} wurde am 30. Juli 2025 eingestellt. Die Funktion bleibt funktionsfähig, bis die Umstellung auf Adobe Identity abgeschlossen ist. Eine neue standortbasierte Zugriffssteuerungsfunktion für Adobe Identity in Adobe Admin Console wird in Kürze eingeführt.

   * _Einstellung von Single Sign-On (SSO)_: Die Unterstützung für [Marketo Identity SSO](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} endete am 30. Juli 2025. Die Funktion bleibt funktionsfähig, bis die Umstellung auf Adobe Identity abgeschlossen ist. Das Single Sign-On für Adobe Identity in der Adobe Admin Console muss separat konfiguriert werden. Informationen zu den Einrichtungsschritten finden Sie unter [Einrichten von Identitäten und Single Sign-On](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html){target="_blank"}.

* **Einstellung von _An einen Freund weiterleiten_ Funktion**: Am 29. September 2025 wird die _An einen Freund weiterleiten_ Funktion in Marketo Engage 2.0-E-Mails (dem alten E-Mail-Editor) für alle Abonnements vollständig eingestellt. Dies betrifft die Links „An einen Freund weiterleiten“ und „An einen Freund weiterleiten“ in E-Mails, die bereits mit dem Token gesendet wurden oder werden. [Weitere Informationen](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Einstellung des Parameters „access_token“ der REST-API**: Der Abfrageparameter `access_token`, der zum Authentifizieren von Marketo REST-API-Aufrufen verwendet wird, wird nicht mehr unterstützt und wird nach dem 31. Oktober 2025 nicht mehr verfügbar sein. Alle neuen und vorhandenen Integrationen sollten REST-API-Aufrufe mit dem Header „Authorization“ authentifizieren, [wie hier beschrieben](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Abschaffung der SOAP-API**: Die Unterstützung für die Marketo SOAP-API endet am 31. Oktober 2025. Services, die SOAP-API-Funktionen verwenden, sollten zur [REST-API](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} migriert werden.
