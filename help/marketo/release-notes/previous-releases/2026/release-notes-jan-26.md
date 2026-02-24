---
description: Januar 2026 - Versionshinweise zu Marketo - Produktdokumentation
title: Januar 2026 - Versionshinweise
feature: Release Information
exl-id: 82773c7e-7c25-4407-8283-b1ae21e470f5
source-git-commit: 466f4b43124a2cb0894c4b8ce605521be1c4b4cd
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 35%

---

# Versionshinweise – Januar 2026 {#release-notes-jan-26}

Im Folgenden finden Sie alle Funktionen, die in der Version vom Januar 2026 enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf die Verfügbarkeit der Funktionen.

Die Versionshinweise speziell für Adobe Dynamic Chat [finden Sie hier](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

## Funktionen aus dem standardmäßigen Veröffentlichungszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Veröffentlichungszyklus und werden ab dem **Samstag, 30. Januar 2026** veröffentlicht, wobei die verbleibenden Funktionen in den folgenden Wochen schrittweise bereitgestellt werden. Veröffentlichungsfunktionen und -daten können sich ändern. Überprüfen Sie neben jeder Funktion ihren Status.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <td><strong>E-Mail-Designer - Verbesserung des KI-Assistenten</strong>: Sie können jetzt in Ihrer Eingabeaufforderung direkt Marken-Assets hinzufügen und das Modell bitten, zum Generieren von Inhalten auf diese Quelle zu verweisen, anstatt ein Marken-Asset manuell als Datei hinzuzufügen.</td>
   <td>Freigegeben</td>
   <td>k. A.</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer - Visuelle Vorschau für Fragmente</strong>: Alle veröffentlichten Fragmente werden jetzt als Miniaturansichten angezeigt, sodass Sie schneller die benötigte Vorlage ermitteln können.</td>
   <td>Freigegeben</td>
   <td>k. A.</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer - Aufzählungszeichen</strong>: Sie können jetzt beim Verfassen einer E-Mail in der E-Mail-Designer Aufzählungszeichen auf mehreren Ebenen erstellen.</td>
   <td>Freigegeben</td>
   <td>k. A.</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer - </strong> Inhaltsverbesserungen: Parität mit der Funktion <i>Dynamischer Inhalt</i> im alten E-Mail-Editor.
   <ul>
   <li>Bedingte Inhalte können jetzt auf die Segmentierung in freigegebenen Ordnern angewendet werden.</li>
   <li>Die Segmentierungen sind jetzt in alphabetischer Reihenfolge sortiert.</li>
   </ul>
   </td>
   <td>Freigegeben</td>
   <td>k. A.</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer - Ordner</strong>: Sie können jetzt Ihre mit der E-Mail-Designer erstellten Assets (E-Mails, E-Mail-Vorlagen, Fragmente) mit Ordnern organisieren.</td>
   <td>Freigegeben</td>
   <td>k. A.</td>
  </tr>
  </tbody>
</table>
<br/>

## Nicht standardmäßige Funktionen für den Versionszyklus {#non-standard-release-cycle-features}

Die folgenden Funktionen wurden außerhalb des standardmäßigen Marketo Engage-Veröffentlichungszyklus veröffentlicht.

### Interaktive Webinare {#interactive-webinars}

* **Umfrage-Pod**: Ein neuer Umfrage-Pod ermöglicht es Hosts, strukturierte Feedback-Formulare direkt in einer Live-Sitzung zu entwerfen und bereitzustellen.

* **Ressourcen-Pod**: Der neue Ressourcen-Pod ersetzt die vorherigen Dateien und Web-Link-Pods und bietet eine einzige, einheitliche Möglichkeit, Ressourcen während Live-Sitzungen freizugeben.

* **Verbesserte Raumoberfläche**: Genießen Sie eine aktualisierte und modernere Raumoberfläche, die auf dem neuesten Spectrum 2-Design-Framework von Adobe basiert und an der Bildsprache anderer Adobe-Produkte wie Creative Cloud und Experience Cloud ausgerichtet ist.

Besuchen Sie [diese Seite](https://helpx.adobe.com/de/adobe-connect/release-note/adobe-connect-12-11-release-notes.html){target="_blank"}, um mehr darüber zu erfahren.

## Ankündigungen {#announcements}

* **Marketo Community-Migration abgeschlossen**: Die neue Adobe Experience League-Community ist jetzt live! [Es wurden &#x200B;](https://experienceleaguecommunities.adobe.com/community-pulse-blog-34/community-update-streamlined-ways-to-engage-and-a-redesigned-homepage-247673?profile.language=de){target="_blank"} Verbesserungen vorgenommen, um Ihr Marketo-Community-Erlebnis noch besser zu gestalten. [Schau dir das an](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-26?profile.language=de){target="_blank"}.

* **Einstellung des Parameters „access_token“ der REST-API**: Der Abfrageparameter `access_token`, der zum Authentifizieren von Marketo REST-API-Aufrufen verwendet wird, wird nicht mehr unterstützt und wird nach dem Mittwoch, 31. März 2026 nicht mehr verfügbar sein. Alle neuen und vorhandenen Integrationen sollten REST-API-Aufrufe mit dem Header „Authorization“ authentifizieren, [wie hier beschrieben](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Abschaffung der SOAP-API**: Die Unterstützung für die Marketo SOAP-API endet am 31. März 2026. Services, die SOAP-API-Funktionen verwenden, sollten zur [REST-API](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} migriert werden.
