---
description: Oktober 2024 - Versionshinweise zu Marketo - Produktdokumentation
title: Oktober 2024 – Versionshinweise
feature: Release Information
exl-id: 2e28ae7f-51de-4510-b3e8-79a989f0daf5
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 3%

---

# Versionshinweise: Oktober 2024 {#release-notes-oct-24}

Unten finden Sie alle Funktionen, die in der Version vom Oktober 2024 enthalten sind. Überprüfen Sie Ihre Adobe Marketo Engage Edition auf die Verfügbarkeit der Funktionen.

Die Versionshinweise speziell für Adobe Dynamic Chat [finden Sie hier](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Mit einem Stern (![star](assets/yellow-star.png) gekennzeichnete Funktionen sind kostenpflichtige Add-ons. Weitere Informationen erhalten Sie vom Marketo Engage-Support.

## Standardfunktionen des Veröffentlichungszyklus {#standard-release-cycle-features}

Die folgenden Funktionen fallen unter den standardmäßigen Veröffentlichungszyklus und werden ab dem **. Oktober 2024 veröffentlicht** wobei die verbleibenden Funktionen in den folgenden Wochen schrittweise eingeführt werden. Veröffentlichungsfunktionen und -daten können sich ändern. Überprüfen Sie neben jeder Funktion auf ihren Status.

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:65%">Funktion</th>
   <th style="width:10%">Status</th>
   <th style="width:25%">Dokumentation</th>
  </tr>
    <tr>
   <td><strong>Tokenisierung für interaktive Webinare</strong>: Sie können jetzt Token verwenden, um interaktive Webinare in E-Mails und Landingpages zu bewerben, ohne die Details des Webinars manuell hinzufügen zu müssen.</td>
   <td>Versendet</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/promoting-an-interactive-webinar.md#interactive-webinars-tokens" target="_blank">Bewerben eines interaktiven Webinars</a></td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  </tr>
   <tr>
   <td><strong>Smart List „Set to Affect“ Count</strong>: Zeigt an, wie viele Personen von der Bearbeitung der Qualifizierungsregeln einer Smart-Kampagne betroffen sein werden.</td>
   <td>Versendet</td>
   <td>k. A.</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  </tr>
   <tr>
   <td><strong>Schaltfläche „Mein Konto“ in der Navigationsleiste</strong>: Für diejenigen, die zu Adobe Identity Management System migriert haben, ermöglicht eine neue Schaltfläche „Mein Konto“ in der linken Navigationsleiste die Konfiguration Ihrer Zeitzone und den Zugriff auf Abonnementdetails.</td>
   <td>Versendet</td>
   <td>k. A.</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
   <tr>
   <td><strong>E-Mail-Leistungsbericht - </strong>: An E-Mail-Berichtsmetriken und dem Aktivitäts-Tracking wurden mehrere Verbesserungen vorgenommen, die zusätzliche Einblicke bieten und die Genauigkeit verbessern.
   <ul>
   <li>Aus E-Mail-Leistungsmetriken gelöschte und zusammengeführte Personen filtern</li>
   <li>E-Mails werden jetzt als <i>abgebrochen</i> klassifiziert, nachdem drei Tage auf eine Antwortaktivität gewartet wurde</li>
   <li>Geöffnete E-Mails werden für jede Smart-Kampagne separat als eindeutig gezählt</li>
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
   <td><strong>Salesforce-Synchronisierungsrückstandsmetriken</strong>: Überwachen Sie den Synchronisierungsdurchsatz und die Rückstandstrends, um CRM-Aktualisierungen zu planen und zu planen, um ein optimales Synchronisierungserlebnis zu erzielen.
   </td>
   <td>Versendet</td>
   <td><a href="/help/marketo/product-docs/crm-sync/salesforce-sync/salesforce-sync-backlog-metrics.md" target="_blank">Salesforce Sync Backlog-Metriken</a></td>
  </tr>
 </tbody>
</table>
<br/>

## Ankündigungen {#announcements}

* **Aktualisierung der Massenextraktions-API**: Es wurde ein Problem in der Massenextraktions-API behoben, das die Option columnHeaderNames betraf, mit der Sie benutzerdefinierte Spaltenkopfzeilennamen in der exportierten Datei angeben können. Zuvor konnten Spaltenkopfzeilennamen, die Nicht-ASCII-Zeichen enthielten, beschädigt werden.

* **Einstellung von REST-API-Zugriffs-Token**: Der Abfrageparameter „access_token“, der zum Authentifizieren von Marketo-REST-API-Aufrufen verwendet wird, wird nicht mehr unterstützt und ist nach dem 31. Oktober 2025 nicht mehr verfügbar. Alle neuen und vorhandenen Integrationen sollten REST-API-Aufrufe mit dem Header „Authorization“ authentifizieren [wie hier beschrieben](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/authentication#using-an-access-token).

* **QR-Code veraltet**: Am 4. Oktober 2024 wird die QR-Code-Funktion, die in Push-Benachrichtigungen und In-App-Messaging-Assets verwendet wird, eingestellt. Dazu gehört die Verwendung von QR-Codes für ein neues Testgerät sowie die Erstellung neuer Assets mit QR-Codes. Wenn Funktionen mit geringerer Nutzung verworfen werden, können wir ihre Ressourcen für die Gesamtwartung von Marketo Engage neu zuweisen.

* **Munchkin-Änderungen**

   * **Neue Version**: Am 17. September 2024 beginnt das Rollout von [Munchkin](/help/marketo/product-docs/administration/setup-administration/munchkin.md){target="_blank"} v.164 auf Marketo Engage-Instanzen, bei denen die Einstellung &quot;Munchkin Beta&quot; in **Admin** > **Treasure Chest** aktiviert ist. Der Rollout zu allen anderen Instanzen soll am 29. Oktober beginnen. Diese Version aktualisiert die Erstellung von Munchkin-Cookies. An der Funktionalität gibt es keine Änderungen.

   * **Zeichen aus URL entfernt**: Die von Munchkin JS erstellten Aktivitäten „Besuche auf Web-Seite“ und „Klicks auf Link“ entfernen jetzt nicht URL-codierte Steuerzeichen aus allen URL-Feldern. Durch diese Änderung sollen Fehler im Zusammenhang mit der Übertragung dieser Zeichentypen in Systeme verhindert werden, die diese Zeichen nicht unterstützen und für die in Marketo Engage keine gültige Verwendung besteht.
