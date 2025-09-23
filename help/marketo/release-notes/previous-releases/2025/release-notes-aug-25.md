---
description: August 2025 - Marketo-Dokumentation - Produktdokumentation
title: August 2025 - Versionshinweise
feature: Release Information
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 98%

---

# Versionshinweise – August 2025 {#release-notes-aug-25}

Unten finden Sie alle Funktionen, die in der Version August 2025 enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf die Verfügbarkeit der Funktionen.

Die Versionshinweise speziell für Adobe Dynamic Chat [finden Sie hier](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie vom Marketo Engage-Support.

## Funktionen aus dem standardmäßigen Veröffentlichungszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Veröffentlichungszyklus und werden seit dem **22. August 2025** veröffentlicht, wobei die verbleibenden Funktionen in den folgenden Wochen schrittweise bereitgestellt werden. Veröffentlichungsfunktionen und -daten können sich ändern. Überprüfen Sie neben jeder Funktion ihren Status.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer – Reporting</strong>: Die Leistungsberichte für E-Mail und E-Mail-Links zeigen jetzt Daten aus E-Mails an, die mit dem neuen E-Mail-Designer erstellt wurden.</td>
   <td>Versandt</td>
   <td>k. A.</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer – Entfernung der automatischen Vervollständigung</strong>: Die Option zur automatischen Vervollständigung im Token-Personalisierungseditor verwies auf fehlerhafte Objekte und wurde entfernt. Eine erneute Implementierung ist derzeit nicht geplant.</td>
   <td>Versandt</td>
   <td>k. A.</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer – Optimierung der E-Mail-Vorschau</strong>: Bei einigen Benutzenden traten langsamere Ladezeiten auf, wenn sie versuchten, ihre E-Mail auf der Detailseite für E-Mails/E-Mail-Vorlagen/Fragmente als Vorschau anzuzeigen. Dieses Erlebnis wurde für bis zu 60 % schnellere Ladezeiten optimiert.</td>
   <td>Versandt</td>
   <td>k. A.</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer – Vorlagenkorrekturen</strong>: Bei einigen vorkonfigurierten Vorlagen traten Rendering-Probleme auf (z. B. falsche Darstellung in bestimmten Browsern/im Dunkelmodus, falsch ausgerichtete Bilder, falsch platzierte CTA-Schaltflächen und mehr). Die Probleme werden mit dieser Version alle behoben.</td>
   <td>Versandt</td>
   <td>k. A.</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer – Fehlerbehebung beim Sperren von Inhalten</strong>: Wenn zuvor eine E-Mail-Vorlage mit Inhaltssperre erstellt wurde und die Vorlage zum Erstellen einer E-Mail verwendet wurde, blieb die Inhaltssperre auch dann bestehen, wenn die E-Mail zurückgesetzt oder die Option „Design ändern“ ausgewählt wurde. Das Problem wurde mit dieser Version behoben.</td>
   <td>Versandt</td>
   <td>k. A.</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Berechtigung zum Bearbeiten von Einschränkungen für intelligente Kampagnen</strong>: Admins können nun die Möglichkeit, Einschränkungen für intelligente Kampagnen zu ändern, nur auf Benutzende mit entsprechenden Berechtigungen beschränken.</td>
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Ankündigungen {#announcements}

* **Abschaffung der Marketo Engage Identity**: Im August 2025 beginnt Adobe mit der schrittweisen Einstellung der Unterstützung für Marketo Engage Identity (Anmeldung über `login.marketo.com`). Um eine Unterbrechung des Zugriffs auf Marketo Engage zu verhindern, müssen Sie bis spätestens 30. September 2025 zu [Adobe Identity](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} wechseln.

   * _Abschaffung von IP-Einschränkungen_: Die Unterstützung für das [Einschränken von Marketo-Anmeldungen auf Grundlage der IP](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} endete am 30. Juli 2025. Die Funktion bleibt funktionsfähig, bis die Umstellung auf Adobe Identity abgeschlossen ist. Eine neue standortbasierte Zugriffssteuerungsfunktion für Adobe Identity in der Adobe Admin Console ist demnächst verfügbar.

   * _Abschaffung von Single Sign-on (SSO)_: Die Unterstützung für [Marketo Identity SSO](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} endete am 30. Juli 2025. Die Funktion bleibt funktionsfähig, bis die Umstellung auf Adobe Identity abgeschlossen ist. Das Single Sign-On für Adobe Identity in der Adobe Admin Console muss separat konfiguriert werden. Informationen zu den Einrichtungsschritten finden Sie unter [Einrichten von Identitäten und Single Sign-On](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html){target="_blank"}.

* **Einstellung der Funktion _An Freund/Freundin weiterleiten_**: Am 29. September 2025 wird die Funktion _An Freund/Freundin weiterleiten_ in E-Mails in Marketo Engage 2.0 (dem alten E-Mail-Editor) für alle Abonnements vollständig eingestellt. Dies betrifft das Token „An Freund/Freundin weiterleiten“ und die Links „An Freund/Freundin weiterleiten“ in E-Mails, die bereits mit dem Token gesendet wurden oder gesendet werden. [Weitere Informationen](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Einstellung des Parameters „access_token“ der REST-API**: Der Abfrageparameter `access_token`, der zum Authentifizieren von Marketo REST-API-Aufrufen verwendet wird, wird nicht mehr unterstützt und wird nach dem 31. Oktober 2025 nicht mehr verfügbar sein. Alle neuen und vorhandenen Integrationen sollten REST-API-Aufrufe mit dem Header „Authorization“ authentifizieren, [wie hier beschrieben](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Abschaffung der SOAP-API**: Die Unterstützung für die Marketo SOAP-API endet am 31. Oktober 2025. Services, die SOAP-API-Funktionen verwenden, sollten zur [REST-API](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} migriert werden.
