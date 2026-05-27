---
description: August 2025 - Marketo-Dokumentation - Produktdokumentation
title: August 2025 - Versionshinweise
feature: Release Information
exl-id: f4f71a77-d0c0-41c3-9362-afbfb467cc7a
TQID: https://experienceleague.adobe.com/Tt3KgAUlQd8oBN2KV-dFUQdEPmlZ-3tOzQ8T-EaCTfI
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: ea90ebee-5c84-42d9-8b21-006bdabc95a3id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bccid: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2: id: c942e9f6-ed06-481a-abdd-1195363d1452
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: cdd65e7e-8839-44a2-bc21-0e03623b5dd1id: e0eb8757-182f-49f3-94a4-1587d16f5094id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 680
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
   <td>Freigegeben</td>
   <td>Nicht zutreffend</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer – Entfernung der automatischen Vervollständigung</strong>: Die Option zur automatischen Vervollständigung im Token-Personalisierungseditor verwies auf fehlerhafte Objekte und wurde entfernt. Eine erneute Implementierung ist derzeit nicht geplant.</td>
   <td>Freigegeben</td>
   <td>Nicht zutreffend</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer – Optimierung der E-Mail-Vorschau</strong>: Bei einigen Benutzenden traten langsamere Ladezeiten auf, wenn sie versuchten, ihre E-Mail auf der Detailseite für E-Mails/E-Mail-Vorlagen/Fragmente als Vorschau anzuzeigen. Dieses Erlebnis wurde für bis zu 60 % schnellere Ladezeiten optimiert.</td>
   <td>Freigegeben</td>
   <td>Nicht zutreffend</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer – Vorlagenkorrekturen</strong>: Bei einigen vorkonfigurierten Vorlagen traten Rendering-Probleme auf (z. B. falsche Darstellung in bestimmten Browsern/im Dunkelmodus, falsch ausgerichtete Bilder, falsch platzierte CTA-Schaltflächen und mehr). Die Probleme werden mit dieser Version alle behoben.</td>
   <td>Freigegeben</td>
   <td>Nicht zutreffend</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer – Fehlerbehebung beim Sperren von Inhalten</strong>: Wenn zuvor eine E-Mail-Vorlage mit Inhaltssperre erstellt wurde und die Vorlage zum Erstellen einer E-Mail verwendet wurde, blieb die Inhaltssperre auch dann bestehen, wenn die E-Mail zurückgesetzt oder die Option „Design ändern“ ausgewählt wurde. Das Problem wurde mit dieser Version behoben.</td>
   <td>Freigegeben</td>
   <td>Nicht zutreffend</td>
  </tr>
  </tbody>
</table>
<br/>

## Ankündigungen {#announcements}

* **Abschaffung der Marketo Engage Identity**: Im August 2025 beginnt Adobe mit der schrittweisen Einstellung der Unterstützung für Marketo Engage Identity (Anmeldung über `login.marketo.com`). Um eine Unterbrechung des Zugriffs auf Marketo Engage zu verhindern, müssen Sie bis spätestens 30. September 2025 zu [Adobe Identity](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} wechseln.

   * _Abschaffung von IP-Einschränkungen_: Die Unterstützung für das [Einschränken von Marketo-Anmeldungen auf Grundlage der IP](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} endete am 30. Juli 2025. Die Funktion bleibt funktionsfähig, bis die Umstellung auf Adobe Identity abgeschlossen ist. Eine neue standortbasierte Zugriffssteuerungsfunktion für Adobe Identity in der Adobe Admin Console ist demnächst verfügbar.

   * _Abschaffung von Single Sign-on (SSO)_: Die Unterstützung für [Marketo Identity SSO](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} endete am 30. Juli 2025. Die Funktion bleibt funktionsfähig, bis die Umstellung auf Adobe Identity abgeschlossen ist. Das Single Sign-On für Adobe Identity in der Adobe Admin Console muss separat konfiguriert werden. Informationen zu den Einrichtungsschritten finden Sie unter [Einrichten von Identitäten und Single Sign-On](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html){target="_blank"}.

* **Einstellung der Funktion _An Freund/Freundin weiterleiten_**: Am 29. September 2025 wird die Funktion _An Freund/Freundin weiterleiten_ in E-Mails in Marketo Engage 2.0 (dem alten E-Mail-Editor) für alle Abonnements vollständig eingestellt. Dies betrifft das Token „An Freund/Freundin weiterleiten“ und die Links „An Freund/Freundin weiterleiten“ in E-Mails, die bereits mit dem Token gesendet wurden oder gesendet werden. [Weitere Informationen](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Einstellung des Parameters „access_token“ der REST-API**: Der Abfrageparameter `access_token`, der zum Authentifizieren von Marketo-REST-API-Aufrufen verwendet wird, wird nicht mehr unterstützt und ist nach dem 31. März 2026 nicht mehr verfügbar. Alle neuen und vorhandenen Integrationen sollten REST-API-Aufrufe mit dem Header „Authorization“ authentifizieren, [wie hier beschrieben](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Abschaffung der SOAP-API**: Die Unterstützung für die Marketo SOAP-API endet am 31. März 2026. Services, die SOAP-API-Funktionen verwenden, sollten zur [REST-API](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} migriert werden.
