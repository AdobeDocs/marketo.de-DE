---
description: Versionshinweise - Februar 2026 - Marketo-Dokumentation - Produktdokumentation
title: Versionshinweise – Februar 2026
feature: Release Information
exl-id: 679d2fca-99ba-4321-ad0d-a297b7f193fc
source-git-commit: 70939d387dcfe6064e179e4e7e91b16c6baa7b8b
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 41%

---

# Versionshinweise – Februar 2026 {#release-notes-feb-26}

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
   <td>Freigegeben</td>
   <td>Nicht zutreffend</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer - API</strong>: Sie können jetzt API-Aufrufe für die E-Mail-Designer verwenden.</td>
   <td>Freigegeben</td>
   <td><a href="https://developer.adobe.com/marketo-apis/api/asset#">Marketo Asset-API</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer - KI-Assistenten für die </strong>: Jetzt können Sie zusätzlich zu Firefly auch Nano-Bananenmodelle verwenden, um mit dem KI-Assistenten Bilder für E-Mail-Inhalte zu generieren.</td>
   <td>Freigegeben</td>
   <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/email-marketing/email-designer/ai-assistant#create-content-for-a-specific-section">Erstellen von Inhalten für einen bestimmten Abschnitt Ihrer E-Mail</a></td>
  </tr>
  </tbody>
</table>
<br/>

## Ankündigungen {#announcements}

* **Einstellung von SEO** Funktionen: Am Dienstag, 31. März 2026, wird Marketo Engage die Suchmaschinenoptimierungsfunktion (SEO) einstellen. Wenn Sie SEO nicht aktiv verwenden, müssen Sie nichts tun. Wenn Sie SEO in letzter Zeit verwendet haben, haben Sie die Möglichkeit, Ihre Daten zu exportieren. [Weitere Informationen](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-27/seo-feature-deprecation-248617){target="_blank"}.

* **Limit für REST-API-Zusammenführung Leads**: Ab dem 31. März 2026 führen Aufrufe, die mehr als 25 IDs im leadIds-Parameter eines Zusammenführungs-Leads-API-Aufrufs enthalten, zu einem 1080-Fehler-Code, und der Aufruf wird übersprungen. Aufträge, die die Zusammenführung von mehr als 25 Datensätzen in einem erfordern, sollten in mehrere Aufträge aufgeteilt werden, um den Erfolg dieser Aufrufe sicherzustellen.

* **Einstellung des Parameters „access_token“ der REST-API**: Der Abfrageparameter `access_token`, der zum Authentifizieren von Marketo-REST-API-Aufrufen verwendet wird, wird nicht mehr unterstützt und ist nach dem Samstag, 31. Juli 2026 nicht mehr verfügbar. Alle neuen und vorhandenen Integrationen sollten REST-API-Aufrufe mit dem Header „Authorization“ authentifizieren, [wie hier beschrieben](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Abschaffung der SOAP-API**: Die Unterstützung für die Marketo SOAP-API endet am Samstag, 31. Juli 2026. Services, die SOAP-API-Funktionen verwenden, sollten zur [REST-API](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} migriert werden.
