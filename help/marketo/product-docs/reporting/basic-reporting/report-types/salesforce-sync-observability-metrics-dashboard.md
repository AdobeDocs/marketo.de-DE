---
description: Salesforce Sync Observability Metrics Dashboard - Marketo Docs - Produktdokumentation
title: Dashboard "Salesforce Sync Observability Metrics"
hide: true
hidefromtoc: true
feature: Reporting
source-git-commit: 49b1545e61a5d11c1ca6ebf5b17d56ef038f6c65
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---

# Dashboard &quot;Salesforce Sync Observability Metrics&quot; {#salesforce-sync-observability-metrics-dashboard}

Überprüfen Sie Ihre Synchronisierungsleistung und synchronisieren Sie Rücklogs mit diesem Dashboard.

## Durchsatz und Rückstand synchronisieren {#sync-throughput-and-backlog}

1. Gehen Sie unter Marketo Engage in den Admin-Bereich.

   SCREENSHOT

1. Wählen Sie Salesforce aus.

   SCREENSHOT

Die Statistiken spiegeln den Durchsatz und den Rückstand für jeden Objekttyp wider, der in den letzten 24 Stunden synchronisiert wurde. Zu den Objektarten gehören alle Objekte, die synchronisiert werden, einschließlich Lead, Kontakt, Konto, Chancen, Kampagne, Benutzer und benutzerdefinierte Objekte. Die Durchsatzstatistiken werden alle 15 Minuten automatisch aktualisiert. Sie können jedoch manuell mit dem Aktualisierungssymbol aktualisiert werden. Der Rückstand wird stündlich abgerufen.

>[!NOTE]
>
>Statistiken werden rollierend aktualisiert, nicht nach Kalendertag.

SCREENSHOT

<table><thead>
  <tr>
    <th>Feld</th>
    <th>Beschreibung</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Max. synchronisierte Datensätze/Std.</td>
    <td>Die maximale Anzahl von Datensätzen, die pro Stunde synchronisiert wurden (maximaler Durchsatz), die in den letzten 24 Stunden für den Objekttyp beobachtet wurden. Der 24-Stunden-Zeitraum rolliert mit der Zeit, nicht mit dem Kalendertag.</td>
  </tr>
  <tr>
    <td>Synchronisierte Mini-Datensätze/Std</td>
    <td>Die Mindestanzahl der pro Stunde synchronisierten Datensätze (Mindestdurchsatz), die in den letzten 24 Stunden für den Objekttyp beobachtet wurden. Der 24-Stunden-Zeitraum rolliert mit der Zeit, nicht mit dem Kalendertag.</td>
  </tr>
  <tr>
    <td>Durchschnittliche zu synchronisierende Datensätze/Std.</td>
    <td>Die durchschnittliche Anzahl der pro Stunde synchronisierten Datensätze (Mindestdurchsatz), die in den letzten 24 Stunden für den Objekttyp ermittelt wurden. Der 24-Stunden-Zeitraum rolliert mit der Zeit, nicht mit dem Kalendertag. Dies wird als Gesamtzahl der in den letzten 24 Stunden synchronisierten Datensätze berechnet.</td>
  </tr>
  <tr>
    <td>Rückstand synchronisieren</td>
    <td>Der Rückstand der ausstehenden Datensätze bei der Synchronisierung für den Objekttyp. Dies ist die Gesamtsumme der ausstehenden Backlog-Synchronisation in beide Richtungen (von Salesforce zu Marketo Engage und umgekehrt). Der Rückstand von Salesforce wird mithilfe eines API-Aufrufs an Salesforce ermittelt, und der Rückstand von Marketo Engage wird anhand der Statistiken berechnet, die aus dem Änderungs-Datenprotokoll abgerufen werden. Dieser Wert wird stündlich berechnet. Die nächsten beiden Felder in dieser Tabelle geben an, wann der Rückstand zuletzt berechnet wurde bzw. wann der nächste Berechnungszeitplan folgen soll.</td>
  </tr>
  <tr>
    <td>Geschätzter Rückstand (Uhrzeit)</td>
    <td>Geschätzte Dauer für die Synchronisierung des Rückstands nach Objekttyp. Wird als Sync Backlog/Average records synchronisiert, synchronisiert pro Stunde.</td>
  </tr>
  <tr>
    <td>Rückprotokoll zuletzt abgerufen</td>
    <td>Die Zeit der letzten Rückstageberechnung.</td>
  </tr>
  <tr>
    <td>Nächster Rückruf im Backlog</td>
    <td>Der Zeitpunkt der nächsten Rückstageberechnung.</td>
  </tr>
  <tr>
    <td>Status des Rückblicks</td>
    <td>Dies zeigt, ob der Rückstand in den letzten 6 Stunden gestiegen ist. Dies wird als "Wachsen"zurückgeführt, wenn der aktuelle Rückstand größer ist als der vor 6 Stunden aufgezeichnete Rückstand. Andernfalls wird es als "Normal"angezeigt. Dadurch soll angezeigt werden, ob der Synchronisierungsdurchsatz mit dem Rückstand aufholt.</td>
  </tr>
</tbody></table>

## Rückblickstrend {#backlog-trend}

Der Rückstau spiegelt die Änderungen in den Rückständen wider, die in den letzten 5 Tagen aufgezeichnet wurden. Der Rückstand wird in einem 4-Stunden-Zeitintervall angezeigt, das über 5 Tage verteilt ist. Daher zeigt das Diagramm 6 Intervalle pro Tag mal 5 Tage an, was 30 Intervalle entspricht.

Der Rückstand wird in einem bestimmten 4-Stunden-Zeitintervall auf der x-Achse beobachtet. Dieser Wert gilt für alle Objekte, die synchronisiert werden. Dies ist die Gesamtsumme des Rückstands in Salesforce und Marketo Engage, die auf die Synchronisierung warten.

SCREENSHOT
