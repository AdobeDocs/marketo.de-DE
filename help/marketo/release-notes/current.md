---
description: Aktuelle Versionshinweise – Marketo-Dokumente – Produktdokumentation
title: Aktuelle Versionshinweise
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: d61ac2c4b7c3fbd138a75b51bb184e4bfd1eef3c
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 7%

---

# Juli 2024 - Versionshinweise {#release-notes-july-24}

Unten finden Sie alle Funktionen der Version vom 24. Juli. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf Funktionsverfügbarkeit.

Die Versionshinweise speziell für Adobe Dynamic Chat [finden Sie hier](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Mit einem Stern (![Stern](assets/yellow-star.png)) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Wenden Sie sich an Ihren Marketo Engage-Support-Mitarbeiter, um mehr zu erfahren.

## Standardfunktionen des Versionszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Versionszyklus und werden am 26. Juli 2024 veröffentlicht. **(Mit einem stufenweisen Rollout der verbleibenden Funktionen in den nachfolgenden Wochen).** Die Veröffentlichungsfunktionen und -daten können sich ändern. Bitte überprüfen Sie neben den einzelnen Funktionen nach ihrem Status.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Funktion</th> 
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
     <tr> 
   <td><strong>Interaktions-Dashboard für interaktive Webinare</strong>: Rufen Sie eine aggregierte Webinar-Leistungsansicht sowie eine umfassende Übersicht über die Interaktion für jeden Teilnehmer während des Webinars ab, damit Sie mithilfe der Marketo Engage-Orchestrierungs-Tools entscheiden können, welche Ergebnisse zum Targeting führt.</td> 
    <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>Raumverwaltung für interaktive Webinare</strong>: Greifen Sie auf einzelne erstellte Räume zu (und nehmen Sie bei Bedarf Änderungen vor) und greifen Sie auf den Inhalt und die Aufzeichnung zu (und löschen Sie sie bei Bedarf, um den Speicher zu optimieren).</td> 
    <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>Webinar-Anpassung für interaktive Webinare</strong>: Stellen Sie durch die Verwendung einer gemeinsamen Raumschnittstelle, von zwischengeschalteten Bildschirmen (wie z. B. Teilnehmereinstiegsbildschirmen) und benutzerdefinierter Video-Hintergründe ein einheitliches organisationsgenehmigtes Markenerlebnis bereit, sodass die Webinar-Strategie einfacher an die Markenstrategie angepasst werden kann.</td> 
    <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
     <tr> 
   <td><strong>Marketo REST API Change</strong>: Die <a href="https://developers.marketo.com/rest-api/user-management/">User Management API</a> wurde geringfügig geändert. Sowohl die Endpunkte <a href="https://developers.marketo.com/rest-api/user-management/#browse_users">Benutzer durchsuchen</a> als auch <a href="https://developers.marketo.com/rest-api/user-management/#delete_user">Benutzer löschen</a> unterstützen jetzt die Benutzer für die Verwaltung von <a href="/help/marketo/product-docs/target-account-management/setup-tam/target-account-management-overview.md">Target-Konten</a>.</td> 
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Ankündigungen {#announcements}

* **Neue Entwicklerdokumentations-Site**: Im Rahmen unserer kontinuierlichen Bemühungen um die Verbesserung des Marketo Engage-Benutzererlebnisses migrieren wir im Juli 2024 die gesamte Entwicklerdokumentation zur Adobe Experience League- und Adobe Developer-Website. [Weitere Informationen](https://nation.marketo.com/t5/employee-blogs/new-developer-documentation-website/ba-p/351055){target="_blank"}

* **Veraltete Social-Funktionen**: Am Mittwoch, dem 31. Juli 2024, beginnt die Marketo Engage mit der Einstellung der folgenden Social-Funktionen im Produkt:

   * Umfragen
   * Social-Schaltfläche
   * Empfehlungsangebot
   * Videofreigabe
   * Gewinnspiele

Benutzer können keine dieser Social-Funktionen mehr in Marketo Engage erstellen, klonen oder einbetten. Vorhandene Social-Assets werden bis zum 31. Januar 2025 weiterhin funktionieren. [Weitere Informationen](https://nation.marketo.com/t5/employee-blogs/marketo-engage-social-features-deprecation/ba-p/351977){target="_blank"}

* **Zugriffstoken bei Einstellung von Abfrageparametern**: Unterstützung für die Authentifizierung mithilfe von Zugriffstoken in einem Abfrageparameter eines Marketo Engage-REST-API-Aufrufs wird in einer zukünftigen Version (spezifisches Datum TBD) entfernt. Vorhandene Integrationen sollten zur Verwendung der Autorisierungs-Kopfzeile &quot;[hier beschrieben](https://developers.marketo.com/rest-api/authentication/){target="_blank"}&quot;migrieren. Für die neue Entwicklung sollte nur der Autorisierungs-Header für die Authentifizierung mit Marketo Engage verwendet werden.

* **LinkedIn - Erneute Authentifizierung erforderlich**: LinkedIn aktualisiert ihre Marketing-APIs, die von Marketo Engage LinkedIn-Integrationen verwendet werden. Diese Änderungen erfordern eine erneute Authentifizierung aller LinkedIn LaunchPoint-Dienste in Ihrem Menü **Admin** > **LaunchPoint** zwischen dem 26. Juli und dem 15. Dezember 2024, um eine Dienstunterbrechung zu vermeiden. Anweisungen zum Ausführen dieser [hier für Lead Gen Forms](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md){target="_blank"} und [hier für übereinstimmende Zielgruppen](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md){target="_blank"} finden Sie. Der Lead-Gen-Formulardienst weist den Typ &quot;LinkedIn Lead Gen&quot;auf und der Dienst &quot;Matched Audience&quot;hat den Typ &quot;LinkedIn Matched Audiences&quot;. Weitere Informationen finden Sie in den [FAQ zur Migration](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}.
