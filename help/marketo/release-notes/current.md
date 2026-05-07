---
description: Aktuelle Versionshinweise – Marketo-Dokumente – Produktdokumentation
title: Aktuelle Versionshinweise
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: b1c177e03fab297e5f94b1848103ac3239e4d079
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 23%

---

# März 2026 - Versionshinweise {#release-notes-mar-26}

Nachstehend finden Sie alle Funktionen, die in der Version vom 26. März enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf die Verfügbarkeit der Funktionen.

Die Versionshinweise speziell für Adobe Dynamic Chat [finden Sie hier](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Funktionen aus dem standardmäßigen Veröffentlichungszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Veröffentlichungszyklus und werden ab dem 27. **2026 veröffentlicht** wobei die verbleibenden Funktionen in den folgenden Wochen schrittweise eingeführt werden. Veröffentlichungsfunktionen und -daten können sich ändern. Überprüfen Sie neben jeder Funktion ihren Status.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
  <tr>
   <td><strong>E-Mail an Designer - Marken verwalten (Betaversion)</strong>: Generieren Sie E-Mail-Inhalte basierend auf den spezifischen Richtlinien Ihres Unternehmens/Ihrer Marke zum Schreiben von Kopien.</td>
   <td>Freigegeben</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/brands/manage-brands.md" target="_blank">Erstellen und Verwalten von Marken</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer - Schnellaktionen</strong>: <i>Parität mit dem alten E-Mail-Editor</i>. Schnellaktionen sind jetzt für alle E-Mail-Designer-Assets (E-Mails, E-Mail-Vorlagen, Fragmente) verfügbar. Zu den unterstützten Schnellaktionen gehören Duplizieren, Löschen, Verschieben und Erstellen/Bearbeiten von Entwürfen.
   </td>
   <td>Freigegeben</i></td>
   <td>Nicht zutreffend</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
   <tr>
   <td><strong>Email Designer - Outlook Rendering Fix</strong>: Dieses Update behebt Rendering-Probleme, insbesondere in MS Outlook. Im erweiterten HTML-Modus können Sie kleinere HTML-/CSS-Änderungen vornehmen oder Ihrer E-Mail-Vorlage Skript-Tags hinzufügen.
   </td>
   <td>Freigegeben</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/advanced-html-mode.md" target="_blank">Bearbeiten von E-Mail-Vorlagen mit dem erweiterten HTML-Editor</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer - Marken-Score-Checker</strong>: Bewerten Sie die allgemeine Inhaltsqualität, um mögliche Probleme mit Lesbarkeit, Inhaltskohärenz und Effektivität unabhängig von Ihren Markenrichtlinien zu identifizieren.</td>
   <td>Freigegeben</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/brands/brand-score.md" target="_blank">Markenbewertung</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Push-Benachrichtigungen</strong>: Umleitungs-URIs, die in Push-Benachrichtigungen konfiguriert sind, unterstützen jetzt Marketo Engage-Token (nur für <i>Launch-App-</i>).
   </td>
   <td>Freigegeben</td>
   <td><a href="/help/marketo/product-docs/mobile-marketing/push-notifications/configure-mobile-push-notification.md#redirect-uris">Umleitungs-URIs</a></td>
  </tr>
  </tbody>
</table>
<br/>

## Ankündigungen {#announcements}

* **Einstellung von SEO** Funktionen: Am Dienstag, 31. März 2026, wird Marketo Engage die Suchmaschinenoptimierungsfunktion (SEO) einstellen. Wenn Sie SEO nicht aktiv verwenden, müssen Sie nichts tun. Wenn Sie SEO in letzter Zeit verwendet haben, haben Sie die Möglichkeit, Ihre Daten zu exportieren. [Weitere Informationen](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-27/seo-feature-deprecation-248617){target="_blank"}.

* **Limit für REST-API-Zusammenführung Leads**: Ab dem 31. März 2026 führen Aufrufe, die mehr als 25 IDs im leadIds-Parameter eines Zusammenführungs-Leads-API-Aufrufs enthalten, zu einem 1080-Fehler-Code, und der Aufruf wird übersprungen. Aufträge, die die Zusammenführung von mehr als 25 Datensätzen in einem erfordern, sollten in mehrere Aufträge aufgeteilt werden, um den Erfolg dieser Aufrufe sicherzustellen.

* **Einstellung von REST-API-„access_token“-**: Der `access_token` Abfrageparameter, der zum Authentifizieren von Marketo REST-API-Aufrufen verwendet wird, wird nicht mehr unterstützt und ist nach dem 31. Juli 2026 nicht mehr verfügbar. Alle neuen und vorhandenen Integrationen sollten REST-API-Aufrufe mit dem Header „Authorization“ authentifizieren, [wie hier beschrieben](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Einstellung der SOAP-**: Die Unterstützung für die Marketo SOAP-API endet am 31. Juli 2026. Services, die SOAP-API-Funktionen verwenden, sollten zur [REST-API](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} migriert werden.
