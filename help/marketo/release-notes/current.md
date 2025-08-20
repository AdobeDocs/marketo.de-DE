---
description: Aktuelle Versionshinweise – Marketo-Dokumente – Produktdokumentation
title: Aktuelle Versionshinweise
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: ab880e2499ed34eb15fd656b5b4eae0635a6e012
workflow-type: tm+mt
source-wordcount: '575'
ht-degree: 6%

---

# Versionshinweise: August 2025 {#release-notes-aug-25}

Unten finden Sie alle Funktionen, die in der Version vom 25. August enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage Edition auf die Verfügbarkeit der Funktionen.

Die Versionshinweise speziell für Adobe Dynamic Chat [finden Sie hier](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie vom Marketo Engage-Support.

## Standardfunktionen des Veröffentlichungszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Veröffentlichungszyklus und werden ab dem 22. **2025 veröffentlicht** wobei die verbleibenden Funktionen in den folgenden Wochen schrittweise bereitgestellt werden. Veröffentlichungsfunktionen und -daten können sich ändern. Überprüfen Sie neben jeder Funktion auf ihren Status.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer - Reporting</strong>: Die Berichte E-Mail-Leistung und E-Mail-Link-Leistung zeigen jetzt Daten aus E-Mails an, die mit der neuen E-Mail-Designer erstellt wurden.</td>
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer - Entfernung der automatischen Vervollständigung</strong>: Die Option zur automatischen Vervollständigung im Token-Personalisierungseditor verwies auf fehlerhafte Objekte und wurde entfernt. Eine erneute Implementierung ist derzeit nicht geplant.</td>
   <td>Versendet</td>
   <td>k. A.</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer - Optimierung </strong> E-Mail-Vorschau: Bei einigen Benutzenden traten langsamere Ladezeiten auf, als sie versuchten, ihre E-Mail auf der Detailseite für E-Mail/E-Mail-Vorlage/Fragment in der Vorschau anzuzeigen. Dieses Erlebnis wurde für bis zu 60 % schnellere Ladezeiten optimiert.</td>
   <td><i>Demnächst verfügbar</i></td>
   <td>k. A.</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer - Vorlagenkorrekturen</strong>: Bei einigen vorkonfigurierten Vorlagen traten Rendering-Probleme auf (z. B. falsche Darstellung in bestimmten Browsern/im Dunkelmodus, falsch ausgerichtete Bilder, falsch platzierte CTA-Schaltflächen und einige mehr). Diese werden mit dieser Version alle behoben.</td>
   <td><i>Demnächst verfügbar</i></td>
   <td>k. A.</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer - Inhaltssperren-Fehlerbehebung</strong>: Wenn zuvor eine E-Mail-Vorlage mit Inhaltssperrung erstellt wurde und die Vorlage zum Erstellen einer E-Mail verwendet wurde, blieb die Inhaltssperre auch dann bestehen, wenn die E-Mail zurückgesetzt oder die Option „Design ändern“ ausgewählt wurde. Dieses Problem wurde mit dieser Version behoben.</td>
   <td><i>Demnächst verfügbar</i></td>
   <td>k. A.</td>
  </tr>
  </tbody>
</table>
<br/>

## Ankündigungen {#announcements}

* **Einstellung der Marketo Engage Identity**: Im August 2025 begann Adobe, die Unterstützung für Marketo Engage Identity auslaufen zu lassen (Anmeldung über `login.marketo.com`). Um einen unterbrochenen Zugriff auf Marketo Engage zu verhindern, müssen Sie spätestens [ 30. September 2025 zu ](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"}Adobe Identity wechseln.

   * _Einstellung von IP-_: Die Unterstützung für [Einschränken von Marketo-Anmeldungen auf der Grundlage von IP](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} wurde am 30. Juli 2025 eingestellt. Die Funktion bleibt funktionsfähig, bis die Umstellung auf Adobe Identity abgeschlossen ist. Eine neue standortbasierte Zugriffssteuerungsfunktion für Adobe Identity in Adobe Admin Console wird in Kürze eingeführt.

   * _Einstellung von Single Sign-On (SSO)_: Die Unterstützung für [Marketo Identity SSO](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} endete am 30. Juli 2025. Die Funktion bleibt funktionsfähig, bis die Umstellung auf Adobe Identity abgeschlossen ist. Single Sign-On für Adobe Identity in der Adobe Admin Console muss separat konfiguriert werden. Informationen zu den Einrichtungsschritten finden Sie unter [Einrichten von Identitäten und Single Sign-On](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html){target="_blank"}.

* **Einstellung von _An einen Freund weiterleiten_ Funktion**: Am 29. September 2025 wird die _An einen Freund weiterleiten_ Funktion in Marketo Engage 2.0-E-Mails (dem alten E-Mail-Editor) für alle Abonnements vollständig eingestellt. Dies betrifft die Links „An einen Freund weiterleiten“ und „An einen Freund weiterleiten“ in E-Mails, die bereits mit dem Token gesendet wurden oder werden. [Weitere Informationen](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Einstellung von REST-API-„access_token“-**: Der `access_token` Abfrageparameter, der zum Authentifizieren von Marketo REST-API-Aufrufen verwendet wird, wird nicht mehr unterstützt und wird nach dem 31. Oktober 2025 nicht mehr verfügbar sein. Alle neuen und vorhandenen Integrationen sollten REST-API-Aufrufe mit dem Header „Authorization“ authentifizieren [wie hier beschrieben](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Einstellung der SOAP-**: Die Unterstützung für die Marketo SOAP-API endet am 31. Oktober 2025. Services, die SOAP-API-Funktionen verwenden, sollten zur [REST-API“ migriert ](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
