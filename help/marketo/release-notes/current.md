---
description: Aktuelle Versionshinweise – Marketo-Dokumente – Produktdokumentation
title: Aktuelle Versionshinweise
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 466f4b43124a2cb0894c4b8ce605521be1c4b4cd
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 58%

---

# Versionshinweise – Februar 2026 {#release-notes-jan-26}

Im Folgenden finden Sie alle Funktionen, die in der Version vom Februar 2026 enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf die Verfügbarkeit der Funktionen.

Die Versionshinweise speziell für Adobe Dynamic Chat [finden Sie hier](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Funktionen aus dem standardmäßigen Veröffentlichungszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Veröffentlichungszyklus und werden ab dem **Samstag, 20. Februar 2026** veröffentlicht, wobei die verbleibenden Funktionen in den folgenden Wochen schrittweise bereitgestellt werden. Veröffentlichungsfunktionen und -daten können sich ändern. Überprüfen Sie neben jeder Funktion ihren Status.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer - </strong>: Parität mit dem alten E-Mail-Editor.
   <ul>
   <li>Freigeben und Archivieren von Ordneraktionen für E-Mail-Designer-Assets.</li>
   <li>Geben Sie Ordner in allen Arbeitsbereichen frei, klicken Sie mit der rechten Maustaste auf einen Ordner, um ein neues Asset zu erstellen, und verschieben Sie Assets per Drag-and-Drop.</li>
   </ul>
   </td>
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer - API</strong>: Sie können jetzt API-Aufrufe für die E-Mail-Designer verwenden.</td>
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail an Designer - Marken verwalten (Betaversion)</strong>: Generieren Sie E-Mail-Inhalte basierend auf den spezifischen Richtlinien Ihres Unternehmens/Ihrer Marke zum Schreiben von Kopien.</td>
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail Designer - Brand Quality Checker</strong>: Bewerten Sie die allgemeine Inhaltsqualität, um mögliche Probleme mit Lesbarkeit, Inhaltskohärenz und Effektivität unabhängig von Ihren Markenrichtlinien zu identifizieren.</td>
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer - KI-Assistenten für die </strong>: Jetzt können Sie zusätzlich zu Firefly auch Nano-Bananenmodelle verwenden, um mit dem KI-Assistenten Bilder für E-Mail-Inhalte zu generieren.</td>
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Ankündigungen {#announcements}

* **Einstellung des Parameters „access_token“ der REST-API**: Der Abfrageparameter `access_token`, der zum Authentifizieren von Marketo-REST-API-Aufrufen verwendet wird, wird nicht mehr unterstützt und ist nach dem 31. März 2026 nicht mehr verfügbar. Alle neuen und vorhandenen Integrationen sollten REST-API-Aufrufe mit dem Header „Authorization“ authentifizieren, [wie hier beschrieben](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Abschaffung der SOAP-API**: Die Unterstützung für die Marketo SOAP-API endet am 31. März 2026. Services, die SOAP-API-Funktionen verwenden, sollten zur [REST-API](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} migriert werden.
