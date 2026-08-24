---
description: AWS-Migration - Marketo Engage-Dokumente - Produktdokumentation
title: AWS-Migration
feature: Getting Started
exl-id: a4bb6c23-ec63-43ec-9fbe-b1cb3928f233
source-git-commit: 35b46e05dc20fc25e3be470433857705528f76f9
workflow-type: tm+mt
source-wordcount: '864'
ht-degree: 5%

---

# AWS-Migration {#aws-migration}

In den nächsten Monaten werden alle Marketo Engage-Abonnements von einem privaten Rechenzentrum in die öffentliche Cloud von AWS migriert, um Zuverlässigkeit, Skalierbarkeit und Geschwindigkeit zu verbessern.

Sie erhalten ca. 30 Tage vor der Migration eine E-Mail sowie eine In-App-Benachrichtigung. Verwenden Sie dieses Handbuch zur Vorbereitung.

## Empfohlene Aktionen {#actions}

Während des Migrationsfensters sind nicht alle Marketo Engage-Services verfügbar. Wir empfehlen, die folgenden Schritte zu unternehmen, um die Auswirkungen auf Ihr Unternehmen zu minimieren.

* **Vermeiden Sie das Erstellen oder Aktualisieren von Leads/Personen** das Ausführen von Prozessen, die Personendatensätze ändern.

* **Keine Trigger-Folgeprozesse** da geplante Kampagnen angehalten werden.

* **Deaktivieren Sie vorübergehend alle Integrationen** die Daten an oder von Marketo Engage senden oder empfangen.

* **Vermeiden Sie**, Datenimporte oder -exporte oder größere Kampagnen zur Lead-/Personengenerierung.

* **IP-Zulassungslisten überprüfen und aktualisieren** für Anmeldung, API-Zugriff, E-Mail-Versand, Webtracking und Integrationen.

* **Neue IP-Adressen hinzufügen** und die aktuellen IPs unverändert lassen. Siehe die IP-Adressen, die über die ([&#x200B; Tabelle unten) hinzugefügt werden &#x200B;](#ip-addresses).

## Erwartete Service-Auswirkungen {#impacts}

Die folgenden Auswirkungen erfordern keine Maßnahmen Ihrerseits.

* **CRM-Integrationen und LaunchPoint** Services werden deaktiviert, sollten aber danach automatisch fortgesetzt werden.
* **Landingpages, Formulare und Datenerfassung** sind nicht verfügbar und stattdessen wird eine Wartungsmeldung angezeigt.

>[!NOTE]
>
>Wenn Sie [externe Formulare](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md){target="_blank"} verwenden und vermeiden möchten, dass Formulardaten verloren gehen, die erfasst wurden, während Marketo Engage während Ihres Migrationsfensters nicht verfügbar ist, wenden Sie sich [&#128279;](https://experienceleague.adobe.com/de/support){target="_blank"} Adobe-Support **mindestens zwei** im Voraus und geben Sie die Formular-ID und die Munchkin-ID Ihres Abonnements an.

## Identifizieren des Rechenzentrums/Pods {#identify}

Bevor Sie sich die folgenden Tabellen ansehen, [&#x200B; Sie (Erfahren Sie, wie Sie &#x200B;](/help/marketo/getting-started/things-to-know/system-status-notifications.md#identify), in welchem Rechenzentrum und Pod/Server sich Ihr Abonnement befindet).

## Zeitplan {#schedule}

Es werden regelmäßig neue Daten und Daten zum Rechenzentrum/Pod hinzugefügt oder geändert. Überwachen Sie daher diesen Zeitplan für Aktualisierungen.

+++Zeitplan Juli
<table>
 <tbody>
  <tr>
   <th style="width:25%">Datum</th>
   <th style="width:25%">Rechenzentrum/Pod</th>
   <th style="width:25%">Uhrzeit</th>
   <th style="width:25%">Status</th>
  </tr>
  <tr>
   <td>8. Juli 2026</td>
   <td>AB69<br>
   AB64</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
   <td>Abgeschlossen<br>
   Abgeschlossen</td>
  </tr>
  <tr>
   <td>9. Juli 2026</td>
   <td>AB70</td>
   <td>17:00 PDT</td>
   <td>Abgeschlossen</td>
  </tr>
  <tr>
   <td>11. Juli 2026</td>
   <td>AB46</td>
   <td>10 h PDT</td>
   <td>Abgeschlossen</td>
  </tr>
  <tr>
   <td>13. Juli 2026</td>
   <td>NLD101</td>
   <td>10 h PDT</td>
   <td>Abgeschlossen</td>
  </tr>
  <tr>
   <td>15. Juli 2026</td>
   <td>NLD102<br>
   NLD104</td>
   <td>10 h PDT<br>
   11 h PDT</td>
   <td>Abgeschlossen<br>
   Abgeschlossen</td>
  </tr>
  <tr>
   <td>17. Juli 2026</td>
   <td>NLD103<br>
   NLD105</td>
   <td>10 h PDT<br>
   11 h PDT</td>
   <td>Abgeschlossen<br>
   Abgeschlossen</td>
  </tr>
  <tr>
   <td>21. Juli 2026</td>
   <td>AB54</td>
   <td>17:00 PDT</td>
   <td>Abgeschlossen</td>
  </tr>
  <tr>
   <td>23. Juli 2026</td>
   <td>AB48</td>
   <td>17:00 PDT</td>
   <td>Abgeschlossen</td>
  </tr>
  <tr>
   <td>31. Juli 2026</td>
   <td>AB43</td>
   <td>15:00 PDT</td>
   <td>Abgeschlossen</td>
  </tr>
  </body>
</table>

+++

<table>
 <tbody>
  <tr>
   <th style="width:25%">Datum</th>
   <th style="width:25%">Rechenzentrum/Pod</th>
   <th style="width:25%">Uhrzeit</th>
   <th style="width:25%">Status</th>
  </tr>
  <tr>
   <td>12. August 2026</td>
   <td>AB61<br>
   AB17</td>
   <td>15:00 PDT<br>
   16:00 PDT</td>
   <td>Abgeschlossen<br>
   Abgeschlossen</td>
  </tr>
  <tr>
  <td>13. August 2026</td>
   <td>AB68</td>
   <td>16:00 PDT</td>
   <td>Abgeschlossen</td>
  </tr>
  <tr>
   <td>18. August 2026</td>
   <td><i>AB39</i></td>
   <td><i>17:00 PDT</i></td>
   <td><i>Zurückgestellt (Datum wird noch bekannt gegeben)</i></td>
  </tr>
  <tr>
   <td>20. August 2026</td>
   <td>AB42<br>
   <i>AB44</i></td>
   <td>17:00 PDT<br>
   <i>18:00 PDT</i></td>
   <td>Abgeschlossen<br>
   <i>Zurückgestellt (Datum wird noch bekannt gegeben)</i></td>
  </tr>
  <tr>
   <td>26. August 2026</td>
   <td>AB40<br>
   AB50</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
   <td>Planmäßig<br>
   Planmäßig</td>
  </tr>
  <tr>
   <td>28. August 2026</td>
   <td>AB53<br>
   AB56</td>
   <td>15:00 PDT<br>
   16:00 PDT</td>
   <td>Planmäßig<br>
   Planmäßig</td>
  </tr>
  <tr>
   <td>8. September 2026</td>
   <td>AB01<br>
   AB02</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
   <td>Planmäßig<br>
   Planmäßig</td>
  </tr>
  <tr>
   <td>10. September 2026</td>
   <td>AB03<br>
   <i>AB04</i></td>
   <td>17:00 PDT<br>
   <i>18:00 PDT</i></td>
   <td>Planmäßig<br>
   <i>Zurückgestellt (Datum wird noch bekannt gegeben)</i></td>
  </tr>
  <tr>
   <td>15. September 2026</td>
   <td>AB05<br>
   AB06</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
   <td>Planmäßig<br>
   Planmäßig</td>
  </tr>
  <tr>
   <td>17. September 2026</td>
   <td>AB07<br>
   AB08</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
   <td>Planmäßig<br>
   Planmäßig</td>
  </tr>
  <tr>
   <td>22. September 2026</td>
   <td>AB09<br>
   AB12</td>
   <td>17:00 PDT<br>
   18:00 PDT</td>
   <td>Planmäßig<br>
   Planmäßig</td>
  </tr>
  <tr>
   <td>25. September 2026</td>
   <td>AB10<br>
   AB11</td>
   <td>16:00 PDT<br>
   17:00 PDT</td>
   <td>Planmäßig<br>
   Planmäßig</td>
  </tr>
  </body>
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
</body>
</table>

## Updates und Support {#support}

Setzen Sie ein Lesezeichen für diese Seite, um die neuesten Aktualisierungen zu erhalten. Bei Fragen wenden Sie sich über das Support-Portal in der Admin Console oder [Experience League an den Adobe-Support](https://experienceleague.adobe.com/de/support){target="_blank"}.

## Häufig gestellte Fragen {#faq}

**Wo werden die Daten gespeichert?**
Alle Marketo-Benutzerdaten werden in Amazon Web Services (AWS) gespeichert. Marketo hat seine Infrastruktur von eigenen physischen Rechenzentren auf die Cloud-Plattform von AWS für Unternehmen migriert.

**Wo werden personenbezogene Daten gespeichert?**
Personenbezogene Daten werden in Amazon Aurora gespeichert, dem vollständig verwalteten relationalen Datenbankdienst von AWS. Aurora repliziert Daten auf sechs Arten in drei separaten Verfügbarkeitszonen innerhalb der AWS-Region, um personenbezogene Daten vor Hardwarefehlern, Speicherverlusten und lokalen Infrastrukturereignissen zu schützen.

**Wem gehört die Speicherumgebung?**
Die Speicherinfrastruktur ist im Besitz und wird von Amazon Web Services (AWS) betrieben. Adobe (Marketo) fungiert als Kunde von AWS unter einem Modell der gemeinsamen Verantwortung: AWS ist für die Sicherheit und Verfügbarkeit der zugrunde liegenden Infrastruktur verantwortlich, während Adobe für die Sicherheit der Daten und Anwendungen verantwortlich ist, die darin ausgeführt werden.

**Was sind die vollständigen Details zu Produktion, Backup-/DR-Standorten und Speichertechnologie?**
Marketo verwendet Amazon Aurora, eine Cloud-native relationale Datenbank-Engine, die vollständig von AWS verwaltet wird, als primäre Datenbanktechnologie. Aurora entkoppelt die Datenverarbeitung und -speicherung, repliziert Daten automatisch auf sechs Wegen in drei Verfügbarkeitszonen innerhalb der Produktionsregion und benötigt zur Bestätigung eines Schreibvorgangs ein Quorum von vier Kopien.

Aurora führt auch kontinuierliche, automatische Backups in Echtzeit auf Amazon S3 durch, sodass Point-in-Time Recovery (PITR) zu jeder Sekunde innerhalb des konfigurierten Aufbewahrungsfensters möglich ist.

Derzeit erfolgt die Aurora-Bereitstellung von Marketo innerhalb einer einzigen AWS-Region, ohne dass eine regionenübergreifende Replikation erforderlich ist. Die Produktionsdaten verbleiben innerhalb der ausgewiesenen regionalen Infrastruktur, und die Notfallwiederherstellung erfolgt durch Auroras Multi-AZ-Speicherredundanz und kontinuierliche Backups anstatt durch ein geografisches Failover auf eine sekundäre Region. Dieser Wert kann im Zuge der Weiterentwicklung der AWS-Infrastruktur von Marketo weiter ausgewertet werden.
