---
description: Juli 2024 - Versionshinweise zu Marketo - Produktdokumentation
title: Versionshinweise – Juli 2024
feature: Release Information
exl-id: ff63af41-2d33-40f8-abca-3fd9493e7916
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 23%

---

# Versionshinweise – Juli 2024 {#release-notes-july-24}

Unten finden Sie alle Funktionen, die in der Version vom 24. Juli enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf die Verfügbarkeit der Funktionen.

Die Versionshinweise speziell für Adobe Dynamic Chat [finden Sie hier](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie vom Marketo Engage-Support.

## Funktionen aus dem standardmäßigen Veröffentlichungszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Veröffentlichungszyklus und werden seit dem **Samstag, 26. Juli 2024 veröffentlicht**, wobei die verbleibenden Funktionen in den folgenden Wochen schrittweise bereitgestellt werden. Veröffentlichungsfunktionen und -daten können sich ändern. Überprüfen Sie neben jeder Funktion ihren Status.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
     <tr>
   <td><strong>Interaktions-Dashboard für interaktive Webinare</strong>: Sie erhalten während des Webinars eine aggregierte Leistungsansicht sowie eine umfassende Ansicht der Interaktion für jeden Teilnehmer, damit Sie über die Orchestrierungs-Tools von Marketo Engage entscheiden können, welche Leads zu Target führen.</td>
    <td>Versandt</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/engagement-dashboard.md" target="_blank">Interaktions-Dashboard</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr>
   <td><strong>Raumverwaltung für interaktive Webinare</strong>: Greifen Sie auf einzelne erstellte Räume zu (und nehmen Sie bei Bedarf Änderungen vor) und greifen Sie auf den Inhalt und die Aufzeichnung zu (und löschen Sie sie bei Bedarf, um die Speicherung zu optimieren).</td>
    <td>Versandt</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/room-management.md" target="_blank">Raumverwaltung</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr>
   <td><strong>Webinar-Anpassung für interaktive Webinare</strong>: Bieten Sie ein einheitliches, von Ihrer Organisation genehmigtes Markenerlebnis durch die Verwendung einer Common-Room-Oberfläche, von Zwischenbildschirmen (z. B. Hintergrundbilder der Teilnehmer-Einstiegsbildschirme) sowie von benutzerdefinierten Videohintergründen, sodass die Webinar-Strategie leichter an die Markenstrategie angepasst werden kann.</td>
    <td>Versandt</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/customization.md" target="_blank">Anpassung interaktiver Webinare</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr>
   <td><strong>Änderung der Marketo REST</strong>-API: Wir führen eine geringfügige Änderung an der <a href="https://developers.marketo.com/rest-api/user-management/">User Management-API“ </a>. Sowohl die Endpunkte <a href="https://developers.marketo.com/rest-api/user-management/#browse_users">Benutzer durchsuchen</a> als auch <a href="https://developers.marketo.com/rest-api/user-management/#delete_user">Benutzer löschen</a> unterstützen jetzt <a href="/help/marketo/product-docs/target-account-management/setup-tam/target-account-management-overview.md">Target Account Management</a>.</td>
   <td>Versandt</td>
   <td>k. A.</td>
  </tr>
 </tbody>
</table>
<br/>

## Ankündigungen {#announcements}

* **Neue Site zur Entwicklerdokumentation**: Im Rahmen unserer kontinuierlichen Bemühungen zur Verbesserung des Marketo Engage-Benutzererlebnisses migrieren wir im Juli 2024 die gesamte Entwicklerdokumentation zur Adobe Experience League und zur Adobe Developer-Website. [Weitere Informationen](https://nation.marketo.com/t5/employee-blogs/new-developer-documentation-website/ba-p/351055){target="_blank"}

* **Einstellung von Social-**: Am Mittwoch, 31. Juli 2024, beginnt Marketo Engage mit der Einstellung der folgenden Social-Media-Funktionen im Produkt:

   * Umfragen
   * Social-Schaltfläche
   * Empfehlungsangebot
   * Videofreigabe
   * Gewinnspiele

Benutzende können keine dieser Social-Media-Funktionen mehr in Marketo Engage erstellen, klonen oder einbetten. Vorhandene soziale Assets funktionieren bis zum 31. Januar 2025 weiterhin. [Weitere Informationen](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **Veraltete Zugriffstoken in Abfrageparametern**: Die Unterstützung für die Authentifizierung mithilfe von Zugriffstoken in einem Abfrageparameter eines Marketo Engage-REST-API-Aufrufs wird in einer zukünftigen Version entfernt (spezifisches Datum wird noch bekannt gegeben). Vorhandene Integrationen sollten zur Verwendung der Autorisierungs-Kopfzeile migriert werden [hier beschrieben](https://developers.marketo.com/rest-api/authentication/){target="_blank"}. Für neue Entwicklungen sollte nur der Autorisierungs-Header für die Authentifizierung mit Marketo Engage verwendet werden.

* **Erneute Authentifizierung für LinkedIn erforderlich**: LinkedIn aktualisiert seine Marketing-APIs, die von Marketo Engage LinkedIn-Integrationen verwendet werden. Diese Änderungen erfordern zwischen dem 26. Juli und dem 15. Dezember 2024 eine erneute Authentifizierung aller LinkedIn LaunchPoint-Services in Ihrem **Admin** > **LaunchPoint**-Menü, um eine Unterbrechung des Services zu vermeiden. Anweisungen dazu finden Sie (hier [&#x200B; Lead Gen Forms](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md){target="_blank"} und [hier für übereinstimmende Zielgruppen](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md){target="_blank"}. Der Formular-Service der Lead-Generation hat den Typ „LinkedIn-Lead-Gen“ und der Dienst für abgeglichene Zielgruppe hat den Typ „LinkedIn-abgeglichene Zielgruppen“. Weitere Informationen finden Sie unter [Häufig gestellte Fragen zur Migration](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}.
