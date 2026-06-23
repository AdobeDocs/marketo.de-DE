---
description: AWS-Migration - Marketo Engage-Dokumente - Produktdokumentation
title: AWS-Migration
feature: Getting Started
hide: true
exl-id: a4bb6c23-ec63-43ec-9fbe-b1cb3928f233
source-git-commit: 9c2784f06be42e5b65cd338a18b0d37a8fa48d9a
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 2%

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

* **Neue IP-Adressen hinzufügen** und die aktuellen IPs unverändert lassen. Siehe die IP-Adressen, die über die ([&#x200B; Tabelle unten) hinzugefügt werden &#x200B;](#ip-addresses).

## Erwartete Service-Auswirkungen

Die folgenden Auswirkungen erfordern keine Maßnahmen Ihrerseits.

* **CRM-Integrationen und LaunchPoint** Services werden deaktiviert, sollten aber danach automatisch fortgesetzt werden.
* **Landingpages, Formulare und Datenerfassung** sind nicht verfügbar und stattdessen wird eine Wartungsmeldung angezeigt.

## Identifizieren des Rechenzentrums/Pods {#identify}

Bevor Sie sich die folgenden Tabellen ansehen, [&#x200B; Sie (Erfahren Sie, wie Sie &#x200B;](/help/marketo/getting-started/things-to-know/system-status-notifications.md#identify), in welchem Rechenzentrum und Pod/Server sich Ihr Abonnement befindet).

## Zeitplan {#schedule}

Regelmäßig werden neue Daten und Informationen zu Rechenzentren/Pods hinzugefügt. Schauen Sie also hier vorbei, um mehr darüber zu erfahren.

<table>
 <tbody>
  <tr>
   <th style="width:50%">Datum</th>
   <th style="width:20%">Rechenzentrum/Pod</th>
   <th style="width:30%">Uhrzeit</th>
  </tr>
  <tr>
   <td>8. Juli 2026</td>
   <td>AB69<br>
   AB64</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
  </tr>
  <tr>
   <td>9. Juli 2026</td>
   <td>AB70<br>
   AB43</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
  </tr>
  <tr>
   <td>11. Juli 2026</td>
   <td>AB46</td>
   <td>10 h PDT</td>
  </tr>
  <tr>
   <td>13. Juli 2026</td>
   <td>NLD101</td>
   <td>10 h PDT</td>
  </tr>
  <tr>
   <td>15. Juli 2026</td>
   <td>NLD102<br>
   NLD104</td>
   <td>10 h PDT<br>
   11 h PDT</td>
  </tr>
  <tr>
   <td>17. Juli 2026</td>
   <td>NLD103<br>
   NLD105</td>
   <td>10 h PDT<br>
   11 h PDT</td>
  </tr>
  &lt;/body>
</table>

## Hinzuzufügende IP-Adressen {#ip-addresses}

Arbeiten Sie je nach Rechenzentrum mit Ihrer IT-Abteilung zusammen, um die entsprechenden IP-Adressen hinzuzufügen.

<table>
<tbody>
<tr>
  <th style="width:25%">Rechenzentrum</th>
  <th style="width:75%">IP-Adressen</th>
</tr>
<tr>
  <td>AB</td>
  <td>54.160.246.246<br>
  54.237.141.197<br>
  52.20.211.99</td>
</tr>
<tr>
  <td>NLD</td>
  <td>34.247.24.245<br>
18.200.201.81<br>
54.220.138.65</td>
</tr>
&lt;/body>
</table>

## Updates und Support

Setzen Sie ein Lesezeichen für diese Seite, um die neuesten Aktualisierungen zu erhalten. Bei Fragen wenden Sie sich über das Support-Portal in der Admin Console oder [Experience League an den Adobe-Support](https://experienceleague.adobe.com/en/support){target="_blank"}.
