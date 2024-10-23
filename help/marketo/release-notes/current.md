---
description: Aktuelle Versionshinweise – Marketo-Dokumente – Produktdokumentation
title: Aktuelle Versionshinweise
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: a65ff2cb24b264cd2d3a1c9c7e0109bcf69ac996
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 5%

---

# Oktober 2024 - Versionshinweise {#release-notes-oct-24}

Unten finden Sie alle Funktionen der Version vom 24. Oktober. Überprüfen Sie Ihre Adobe Marketo Engage-Edition auf Funktionsverfügbarkeit.

Die Versionshinweise speziell für Adobe Dynamic Chat [finden Sie hier](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Mit einem Stern (![Stern](assets/yellow-star.png)) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Wenden Sie sich an Ihren Marketo Engage-Support-Mitarbeiter, um mehr zu erfahren.

## Standardfunktionen des Versionszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Versionszyklus und werden ab dem 4. Oktober 2024 veröffentlicht. Außerdem wird in den folgenden Wochen ein stufenweiser Rollout der verbleibenden Funktionen veröffentlicht. **** Die Veröffentlichungsfunktionen und -daten können sich ändern. Bitte überprüfen Sie neben den einzelnen Funktionen nach ihrem Status.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Funktion</th> 
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
    <tr> 
   <td><strong>Verbesserte Registrierungsdaten im Interaktions-Dashboard für interaktive Webinare</strong>: Sie können jetzt sehen, welche Unternehmen am meisten teilgenommen haben, und das Unternehmen, den Titel und die Branche auf Lead-Ebene in Berichten aktualisieren, die im Interaktions-Dashboard verfügbar sind.</td> 
   <td><i>Demnächst verfügbar</i></td>
   <td><i>Demnächst verfügbar</i></td>
  </tr>
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
    <tr> 
   <td><strong>Tokenisierung für interaktive Webinare</strong>: Sie können jetzt Token verwenden, um interaktive Webinare in E-Mails und Landingpages zu bewerben, ohne die Webinardetails manuell hinzufügen zu müssen.</td> 
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
   <td><strong>Smart List "Set to Affect" Count</strong>: Ermitteln Sie, wie viele Personen von der Bearbeitung der Qualifikationsregeln einer Smart-Kampagne betroffen sind.</td> 
   <td>Versendet</td>
   <td>Nicht zutreffend</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
   <tr> 
   <td><strong>Schaltfläche "Mein Konto"in der Navigationsleiste</strong>: Für diejenigen, die zum Adobe Identity Management System migriert haben, ermöglicht eine neue Schaltfläche "Mein Konto"in der linken Navigationsleiste die Konfiguration Ihrer Zeitzone und den Zugriff auf Abonnementdetails.</td> 
   <td>Versendet</td>
   <td>Nicht zutreffend</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   <tr> 
   <td><strong>Verbesserungen bei E-Mail-Leistungsberichten</strong>: An den E-Mail-Berichtsmetriken und dem Aktivitäts-Tracking wurden mehrere Verbesserungen vorgenommen, die zusätzliche Einblicke bieten und die Genauigkeit verbessern.
   <ul>
   <li>Gelöschte und zusammengeführte Personen aus E-Mail-Leistungsmetriken filtern</li>
   <li>E-Mails, die nach drei Tagen auf Reaktionsaktivität als <i>abgebrochen</i> gewartet wurden</li>
   <li>Die Anzahl der Öffnungen in E-Mails wird separat für jede Smart-Kampagne angezeigt</li>
   <li>Verbessertes E-Mail-Aktivitäts-Tracking durch Verfeinerung des Standort des Tracking-Pixels</li>
   </td> 
   <td>Versendet</td>
   <td><a href="/help/marketo/product-docs/email-marketing/email-programs/email-program-data/email-performance-report.md" target="_blank">E-Mail-Leistungsbericht</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   <tr> 
   <td><strong>Salesforce Sync Backlog Metrics</strong>: Überwachen Sie den Synchronisierungsdurchsatz und die Trends bei der Rückgängigmachen der Synchronisierung, um CRM-Aktualisierungen für ein optimales Synchronisierungserlebnis zu planen und zu planen.
   </td> 
   <td>Versendet</td>
   <td><a href="/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-backlog-metrics.md" target="_blank">Salesforce Sync-Rücklog-Metriken</a></td>
  </tr>
 </tbody> 
</table>
<br/>

## Ankündigungen {#announcements}

* **REST API access_token Parameter Deprecation**: Der Abfrageparameter &quot;access_token&quot;zum Authentifizieren von Marketo REST API-Aufrufen wird nicht mehr unterstützt und ist nach dem 30. Juni 2025 nicht mehr verfügbar. Alle neuen und vorhandenen Integrationen sollten REST-API-Aufrufe mithilfe der &quot;Autorisierungs&quot;-Kopfzeile [authentifizieren, wie hier ](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/authentication#using-an-access-token) beschrieben.


* **QR-Code-Deprecation**: Am 4. Oktober 2024 wird die QR-Code-Funktion, die in Push-Benachrichtigungen und In-App-Nachrichten-Assets verwendet wird, nicht mehr unterstützt. Dazu gehört die Verwendung von QR-Codes für ein neues Testgerät sowie die Erstellung neuer Assets mit QR-Codes. Die Veraltung von Funktionen mit geringerer Nutzung ermöglicht es uns, ihre Ressourcen auf die Gesamtwartung von Marketo Engage umzuleiten.

* **Munchkin-Änderungen**

   * **Neue Version**: Am 17. September 2024 beginnt der Rollout von [Munchkin](/help/marketo/product-docs/administration/setup-administration/munchkin.md){target="_blank"} v.164 zu Marketo Engage-Instanzen, bei denen die Einstellung &quot;Munchkin Beta&quot;unter **Admin** > **Schatztruhe** aktiviert ist. Der Rollout für alle anderen Instanzen soll am 29. Oktober beginnen. Diese Version aktualisiert die Erstellung von Munchkin-Cookies. Die Funktionalität ändert sich nicht.

   * **Zeichen aus URL entfernt**: Die von Munchkin JS erstellten Aktivitäten &quot;Besuche der Webseite&quot;und &quot;Klicks Link&quot;entfernen jetzt nicht URL-kodierte Steuerzeichen aus allen URL-Feldern. Diese Änderung soll Fehler bei der Übertragung dieser Zeichentypen in Systeme verhindern, die sie nicht unterstützen und keine gültige Verwendung innerhalb von Marketo Engage haben.
