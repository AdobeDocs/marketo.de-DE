---
description: AWS-Migration - Marketo Engage-Dokumente - Produktdokumentation
title: AWS-Migration
feature: Getting Started
hide: true
exl-id: a4bb6c23-ec63-43ec-9fbe-b1cb3928f233
source-git-commit: 5a260c00311588c3a55f176e7a7977f422bcc8a4
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 1%

---

# AWS-Migration {#aws-migration}

In den nächsten Monaten werden alle Marketo Engage-Abonnements von einem privaten Rechenzentrum in die öffentliche Cloud von AWS migriert, um Zuverlässigkeit, Skalierbarkeit und Geschwindigkeit zu verbessern.

Sie erhalten ca. 30 Tage vor der Migration eine E-Mail sowie eine In-App-Benachrichtigung. Verwenden Sie dieses Handbuch zur Vorbereitung.

## Empfohlene Aktionen

Während des Migrationsfensters sind nicht alle Marketo Engage-Services verfügbar. Wir empfehlen, die folgenden Schritte zu unternehmen, um die Auswirkungen auf Ihr Unternehmen zu minimieren.

* **Vermeiden Sie das Erstellen oder Aktualisieren von Leads/Personen** das Ausführen von Prozessen, die Personendatensätze ändern.

* **Keine Trigger-Folgeprozesse** da geplante Kampagnen angehalten werden.

* **Deaktivieren Sie vorübergehend alle Integrationen** die Daten an oder von Marketo Engage senden oder empfangen.

* **Vermeiden Sie**, Datenimporte oder -exporte oder größere Kampagnen zur Lead-/Personengenerierung.

* **IP-Zulassungslisten überprüfen und aktualisieren** für Anmeldung, API-Zugriff, E-Mail-Versand, Webtracking und Integrationen.

* **Fügen Sie die folgenden IP-** hinzu und behalten Sie Ihre aktuellen IPs unverändert bei:

   * 54.160.246.246
   * 54.237.141.197
   * 52.20.211.99

## Erwartete Service-Auswirkungen

Die folgenden Auswirkungen erfordern keine Maßnahmen Ihrerseits.

* **CRM-Integrationen und LaunchPoint** Services werden deaktiviert, sollten aber danach automatisch fortgesetzt werden.
* **Landingpages, Formulare und Datenerfassung** sind nicht verfügbar und stattdessen wird eine Wartungsmeldung angezeigt.

## Zeitplan {#schedule}

Regelmäßig werden neue Daten und Informationen zu Rechenzentren/Pods hinzugefügt. Schauen Sie also hier vorbei, um mehr darüber zu erfahren.

Bevor Sie sich die nachstehende Tabelle ansehen[&#x200B; erfahren Sie, &#x200B;](/help/marketo/getting-started/things-to-know/system-status-notifications.md#identify) sich Ihr Abonnement im Rechenzentrum und Pod/Server befindet.

<table>
 <tbody>
  <tr>
   <th style="width:75%">Datum</th>
   <th style="width:25%">Pod</th>
  </tr>
  <tr>
   <td>5. Juni 2026</td>
   <td>AB46</td>
  </tr>
  <tr>
   <td>8. Juli 2026</td>
   <td>AB69<br>
   AB64</td>
  </tr>
  <tr>
   <td>9. Juli 2026</td>
   <td>AB70<br>
   AB43</td>
  </tr>
  &lt;/body>
  </table>

## Updates und Support

Setzen Sie ein Lesezeichen für diese Seite, um die neuesten Aktualisierungen zu erhalten. Bei Fragen wenden Sie sich über das Support-Portal in der Admin Console oder [Experience League an den Adobe-Support](https://experienceleague.adobe.com/de/support).
