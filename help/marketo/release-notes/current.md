---
description: Aktuelle Versionshinweise – Marketo-Dokumente – Produktdokumentation
title: Aktuelle Versionshinweise
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: ea9bf2a002415936cdfb5bfb723ce80723003da5
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 4%

---

# Juli 2024 - Versionshinweise {#release-notes-july-24}

Unten finden Sie alle Funktionen der Version vom 24. Juni. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf Funktionsverfügbarkeit.

Die Versionshinweise speziell für Adobe Dynamic Chat [finden Sie hier .](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png)) sind kostenpflichtige Add-ons. Wenden Sie sich an Ihren Marketo Engage-Support-Mitarbeiter, um mehr zu erfahren.

## Standardfunktionen des Versionszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den Standard-Versionszyklus und werden ab der Veröffentlichung auf **26. Juli 2024**, mit einer stufenweisen Einführung der verbleibenden Funktionen in den darauffolgenden Wochen. Die Veröffentlichungsfunktionen und -daten können sich ändern. Bitte überprüfen Sie neben den einzelnen Funktionen nach ihrem Status.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Funktion</th> 
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
     <tr> 
   <td><strong>Marketo REST API-Änderung</strong>: Wir führen eine geringfügige Änderung an der <a href="https://developers.marketo.com/rest-api/user-management/">User Management-API</a>. Beide <a href="https://developers.marketo.com/rest-api/user-management/#browse_users">Benutzer durchsuchen</a> und <a href="https://developers.marketo.com/rest-api/user-management/#delete_user">Benutzer löschen</a> Endpunkte unterstützen jetzt <a href="/help/marketo/product-docs/target-account-management/setup-tam/target-account-management-overview.md">Verwaltung von Target-Konten</a> Benutzer.</td> 
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Ankündigungen {#announcements}

* **Neue Entwicklerdokumentations-Site**: Im Rahmen unserer kontinuierlichen Bemühungen um die Verbesserung des Marketo Engage-Benutzererlebnisses migrieren wir im Juli 2024 die gesamte Entwicklerdokumentation zur Adobe Experience League- und Adobe Developer-Website. [Weitere Infos](https://nation.marketo.com/t5/employee-blogs/new-developer-documentation-website/ba-p/351055){target="_blank"}

* **Zugriffstoken bei der Einstellung von Abfrageparametern**: Die Unterstützung für die Authentifizierung mit Zugriffstoken in einem Abfrageparameter eines Marketo Engage-REST-API-Aufrufs wird in einer zukünftigen Version (spezifisches Datum TBD) entfernt. Vorhandene Integrationen sollten zur Verwendung der Autorisierungs-Kopfzeile migriert werden [hier beschrieben](https://developers.marketo.com/rest-api/authentication/){target="_blank"}. Für die neue Entwicklung sollte nur der Autorisierungs-Header für die Authentifizierung mit Marketo Engage verwendet werden.

* **LinkedIn-erneute Authentifizierung erforderlich**: LinkedIn aktualisiert ihre Marketing-APIs, die von Marketo Engage LinkedIn-Integrationen verwendet werden. Diese Änderungen erfordern eine erneute Authentifizierung aller LinkedIn LaunchPoint-Dienste in Ihren **Admin** > **LaunchPoint** zwischen dem 26. Juli und dem 15. Dezember 2024, um Dienstunterbrechungen zu vermeiden. Anweisungen dazu finden Sie hier . [hier für Lead Gen Forms](/help/marketo/product-docs/demand-generation/social/social-functions/set-up-linkedin-lead-gen-forms.md){target="_blank"} und [hier für übereinstimmende Zielgruppen](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-linkedin-matched-audiences-as-a-launchpoint-service.md){target="_blank"}. Der Lead-Gen-Formulardienst weist den Typ &quot;LinkedIn Lead Gen&quot;auf und der Dienst &quot;Matched Audience&quot;hat den Typ &quot;LinkedIn Matched Audiences&quot;. Weitere Informationen finden Sie im [Häufig gestellte Fragen zur Migration](https://nation.marketo.com/t5/employee-blogs/linkedin-re-authentication-required/ba-p/347794){target="_blank"}.
