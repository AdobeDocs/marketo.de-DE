---
description: Salesforce Sync-Rücklog-Metriken - Marketo-Dokumente - Produktdokumentation
title: Salesforce Sync-Rücklog-Metriken
hide: true
hidefromtoc: true
feature: Reporting
source-git-commit: a9ed4a7e2247a26b376bde64bb1cfd6db2833822
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 0%

---

# Salesforce Sync-Rücklog-Metriken  {#salesforce-sync-backlog-metrics}

Der Synchronisierungs-Backlog stellt die Datensätze dar, für die eine Synchronisierung von Salesforce mit Marketo Engage aussteht, und umgekehrt. Wenn Sie sicherstellen, dass der Rückstand unter Kontrolle bleibt, werden reibungslose und zeitnahe Synchronisierungen durchgeführt.

>[!NOTE]
>
>Das Rückprotokoll deckt die Zahlen ab, für die eine Synchronisierung nach Aktualisierungen auf beiden Seiten aussteht, und nicht die Zahlen, die durch Synchronisierungsflussschritte wie die Durchsatzschritte [Person mit SFDC synchronisieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} oder [Person mit Microsoft synchronisieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md){target="_blank"} ausgeführt werden.

## Zugriff {#how-to-access}

1. Wechseln Sie unter Marketo Engage zum Bereich **Admin** .

   SCREENSHOT

1. Wählen Sie **Salesforce** aus.

   SCREENSHOT

## Zurückdlog-Trend synchronisieren {#sync-backlog-trend}

Der Rückstau spiegelt die Änderungen in den Rückständen wider, die in den letzten 5 Tagen aufgezeichnet wurden. Der Rückstand wird in einem 4-Stunden-Zeitintervall angezeigt, das über 5 Tage verteilt ist. Daher zeigt das Diagramm 6 Intervalle pro Tag mal 5 Tage an, was 30 Intervalle entspricht.

Der Rückstand wird in einem bestimmten 4-Stunden-Zeitintervall auf der x-Achse beobachtet. Dieser Wert gilt für alle Objekte, die synchronisiert werden. Dies ist die Gesamtsumme des Rückstands in Salesforce und Marketo Engage, die auf die Synchronisierung warten.

SCREENSHOT

## Durchsatz und Rückstand synchronisieren {#sync-throughput-and-backlog}

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
    <td>Geschätzte Dauer für die Synchronisierung des Rückstands nach Objekttyp. Wird als "Backlog/Durchschnittliche, pro Stunde synchronisierte Datensätze synchronisieren"berechnet.</td>
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

## Was führt zu Synchronisierungs-Backlogs? {#what-causes-sync-backlogs}

Unabhängig davon, ob die Aktualisierung auf der Marketo Engage- oder CRM-Seite erfolgt, wird der neu zu synchronisierende Datensatz Trigger, um die Informationen auf der anderen Seite über den regulären Marketo Engage-zu-CRM-Synchronisierungszyklus zu aktualisieren. Jedes Mal, wenn ein Datensatz in Salesforce aktualisiert wird, wird ein Zeitstempel für die Systemmodifizierung generiert, der als &quot;SysModStamp&quot;bezeichnet wird. Dadurch wird eine zu synchronisierende Änderung in die Warteschlange gestellt.

Wenn eine große Anzahl von Aktualisierungen vorgenommen wird (z. B. durch eine Änderung des Feldwerts), werden viele Datensätze geändert, was zu neuen SysModStamps führt. Eine große Anzahl von Personen-Datensatz-Updates müssen dann zwischen Marketo Engage und Ihrem CRM neu synchronisiert werden, was manchmal einen momentanen Rückstand verursacht.

## Best Practices für die Verwaltung von Synchronisierungs-Backlogs {#best-practices-for-managing-sync-backlogs}

**Synchronisierte Felder**: Stellen Sie sicher, dass die synchronisierten Felder nur diejenigen sind, die synchronisiert werden müssen. Änderungen an Feldern erhöhen den Synchronisierungs-Backlog, und Felder mit niedrigerer Priorität werden möglicherweise angehalten oder verlangsamen wichtigere Felder bei der Synchronisierung. Wenden Sie sich an den [Marketo Engage-Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} , um Felder zu entfernen, die synchronisiert sind.

**Sensible Felder**: Einige Felder sind anfällig für häufige Aktualisierungen (z. B. Währungsfelder, die Währungsänderungen unterliegen). Überprüfen Sie, ob diese synchronisiert werden müssen oder ob die Felder anders gestaltet werden müssen.

**Benutzerdefinierte Objekte**: Prüfen Sie regelmäßig benutzerdefinierte Objekte, die synchronisiert werden, und entfernen Sie alle Objekte, die nicht mehr synchronisiert werden müssen.

**Aktivitäten**: Überprüfen Sie, ob synchronisierte Aktivitäten vorhanden sind, die aus der Synchronisierung entfernt werden können.

**Planen Sie Massenaktualisierungen während nicht kritischer Stunden**: Überprüfen Sie Ihre Datensynchronisierungsmuster, um nicht kritische Zeiträume zu identifizieren. Ermitteln Sie, ob Massenaktualisierungen in diesen nicht kritischen Zeiträumen geplant werden können.

Wenn Sie alle oben genannten Best Practices befolgen und weiterhin erhebliche Rückstände aufweisen, wenden Sie sich an den [Marketo Engage-Support](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.
