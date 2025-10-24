---
description: Aktuelle Versionshinweise – Marketo-Dokumente – Produktdokumentation
title: Aktuelle Versionshinweise
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: 7234082102356fc05c760f359ef19ca8cff375b5
workflow-type: ht
source-wordcount: '704'
ht-degree: 100%

---

# Versionshinweise – September 2025 {#release-notes-sep-25}

Unten finden Sie alle Funktionen, die in der Version von September 2025 enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf die Verfügbarkeit der Funktionen.

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
   <td><strong>Speicherung von Aktivitäten zu On-Demand-Webinaren</strong>: Benutzenden interaktiver Webinare stehen Dashboard-Daten zu On-Demand-Webinaren jetzt für mehr als 30 Tage zur Verfügung (zuvor waren es nur bis zu 30 Tage ab dem Tag des Webinars).</td>
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer – Workflow für Content-Zusammenarbeit</strong>: Sie können jetzt mit anderen Marketo-Benutzenden an E-Mail-Assets zusammenarbeiten und Kommentare abgeben. Taggen Sie Team-Mitglieder (Marketo-Benutzende mit entsprechenden Asset-Berechtigungen), sodass sie eine E-Mail- oder Push-Benachrichtigung erhalten.</td>
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer – Berechtigungen für den KI-Assistenten</strong>: Marketo-Admins können bestimmten Benutzenden Zugriff auf GenAI-Funktionen gewähren.</td>
   <td>Versandt</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/ai-assistant.md#set-up-permissions">Berechtigungen einrichten</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer – Dunkler Modus</strong>: Sie können jetzt den dunklen Modus nutzen, in dem E-Mail-Clients und -Apps, die den Modus unterstützen, E-Mails mit dunkleren Hintergründen und helleren Farben für Text, Schaltflächen und andere UI-Elemente anzeigen können.</td>
   <td>Versandt</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-designer/dark-mode.md">Dunkler Modus</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-Mail-Designer – Fehlerbehebung bei Umleitungen</strong>: Bei einigen Benutzenden traten Umleitungsprobleme mit URLs für E-Mails auf, die mit der neuen Designer erstellt wurden (z. B. funktionierte das direkte Einfügen der URLs oder das Hinzufügen von Lesezeichen für E-Mail-Assets nicht immer). Dieses Problem wurde behoben. Darüber hinaus werden Links zu E-Mail-Assets aus <b>E-Mail-Vorlagen</b> &gt; <b>Details</b> &gt; <b>Verwendet von</b> zum entsprechenden E-Mail-Asset umgeleitet.</td>
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Ankündigungen {#announcements}

* **Einstellung der REST-API mit doppelten Schrägstrichen**: Am 16. September 2025 hat Adobe auf eine modernere Hosting-Infrastruktur für REST-API-URLs umgestellt, die neuere Technologien nutzt und so Sicherheit und Skalierbarkeit bietet. Wenn Ihr Abonnement APIs mit einem doppelten Schrägstrich (//) in der URL verwendet hat, finden Sie in [diesem Post von Nation](https://nation.marketo.com/t5/product-blogs/rest-api-double-slash-deprecation/ba-p/358616){target="_blank"} Informationen zu den nächsten Schritten.

* **Zurück zur Geschwindigkeits-Skripterstellung im neuen E-Mail-Designer**: Adobe Marketo Engage hat im vergangenen Juni für den neuen E-Mail-Designer eine Funktion namens _Bedingter Inhalt_ veröffentlicht. Die Funktion basierte auf Handlebar-Skripterstellung anstelle von Geschwindigkeits-Skripterstellung. Das war ein Bemühen, Ihren dynamischen Inhalten etwas mehr Flexibilität zu verleihen. Als wir jedoch erkannten, dass dadurch manche Token falsch aufgelöst werden, entschieden wir, die Funktion vorübergehend zu deaktivieren. [Weitere Informationen](https://nation.marketo.com/t5/product-blogs/update-on-email-scripting-in-the-new-email-designer/ba-p/358179){target="_blank"}

* **Abschaffung der Marketo Engage Identity**: Im August 2025 beginnt Adobe mit der schrittweisen Einstellung der Unterstützung für Marketo Engage Identity (Anmeldung über `login.marketo.com`). Um eine Unterbrechung des Zugriffs auf Marketo Engage zu verhindern, müssen Sie bis spätestens 30. September 2025 zu [Adobe Identity](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} wechseln.

   * _Abschaffung von IP-Einschränkungen_: Die Unterstützung für das [Einschränken von Marketo-Anmeldungen auf Grundlage der IP](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} endete am 30. Juli 2025. Die Funktion bleibt funktionsfähig, bis die Umstellung auf Adobe Identity abgeschlossen ist. Eine neue standortbasierte Zugriffssteuerungsfunktion für Adobe Identity in der Adobe Admin Console ist demnächst verfügbar.

   * _Abschaffung von Single Sign-on (SSO)_: Die Unterstützung für [Marketo Identity SSO](https://experienceleague.adobe.com/de/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} endete am 30. Juli 2025. Die Funktion bleibt funktionsfähig, bis die Umstellung auf Adobe Identity abgeschlossen ist. Das Single Sign-On für Adobe Identity in der Adobe Admin Console muss separat konfiguriert werden. Informationen zu den Einrichtungsschritten finden Sie unter [Einrichten von Identitäten und Single Sign-On](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html){target="_blank"}.

* **Einstellung der Funktion _An Freund/Freundin weiterleiten_**: Am 29. September 2025 wird die Funktion _An Freund/Freundin weiterleiten_ in E-Mails in Marketo Engage 2.0 (dem alten E-Mail-Editor) für alle Abonnements vollständig eingestellt. Dies betrifft das Token „An Freund/Freundin weiterleiten“ und die Links „An Freund/Freundin weiterleiten“ in E-Mails, die bereits mit dem Token gesendet wurden oder gesendet werden. [Weitere Informationen](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Einstellung des Parameters „access_token“ der REST-API**: Der Abfrageparameter `access_token`, der zum Authentifizieren von Marketo REST-API-Aufrufen verwendet wird, wird nicht mehr unterstützt und wird nach dem 31. Januar 2026 nicht mehr verfügbar sein. Alle neuen und vorhandenen Integrationen sollten REST-API-Aufrufe mit dem Header „Authorization“ authentifizieren, [wie hier beschrieben](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Abschaffung der SOAP-API**: Die Unterstützung für die Marketo SOAP-API endet am 31. Januar 2026. Services, die SOAP-API-Funktionen verwenden, sollten zur [REST-API](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} migriert werden.
