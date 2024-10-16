---
description: Salesforce Sync-Rücklog-Metriken - Marketo-Dokumente - Produktdokumentation
title: Salesforce Sync-Rücklog-Metriken
hide: true
hidefromtoc: true
feature: Reporting
source-git-commit: 38929abef0f64762c92b153630ce75373ba7a300
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 0%

---

# Salesforce Sync-Rücklog-Metriken  {#salesforce-sync-backlog-metrics}

Der Synchronisierungs-Backlog ist der Name, der für die Datensätze verwendet wird, deren Synchronisierung aussteht. Es werden Einträge berücksichtigt, die von Salesforce zu Marketo Engage synchronisiert werden müssen, und umgekehrt. Wenn Sie sicherstellen, dass der Rückstand unter Kontrolle bleibt, werden die Synchronisierungen reibungslos und zeitabhängig durchgeführt. Das Rückprotokoll deckt die Zahlen ab, für die Synchronisierungspost-Aktualisierungen auf beiden Seiten ausstehen, und nicht die Zahlen, die von Synchronisierungsfluss-Schritten wie den Durchlaufschritten &quot;Lead mit SFDC synchronisieren&quot;ausgeführt werden.

## Zugriff {#how-to-access}

1. Wechseln Sie unter Marketo Engage zum Bereich **Admin** .

   ![](assets/salesforce-sync-backlog-metrics-1.png)

1. Wählen Sie **Salesforce** aus.

   ![](assets/salesforce-sync-backlog-metrics-2.png)

## Zurückdlog-Trend synchronisieren {#sync-backlog-trend}

Der Rückstau spiegelt die Änderungen in den Rückständen wider, die in den letzten 5 Tagen aufgezeichnet wurden. Der Rückstand wird in einem 4-Stunden-Zeitintervall angezeigt, das über 5 Tage verteilt ist. Daher zeigt das Diagramm 6 Intervalle pro Tag mal 5 Tage an, was 30 Intervalle entspricht.

Der Rückstand wird in einem bestimmten 4-Stunden-Zeitintervall auf der x-Achse beobachtet. Dieser Wert gilt für alle Objekte, die synchronisiert werden. Dies ist die Gesamtsumme des Rückstands in Salesforce und Marketo Engage, die auf die Synchronisierung warten.

![](assets/salesforce-sync-backlog-metrics-3.png)

## Durchsatz und Rückstand synchronisieren {#sync-throughput-and-backlog}

Die Statistiken spiegeln den Durchsatz und den Rückstand für jeden Objekttyp wider, der in den letzten 24 Stunden synchronisiert wurde. Zu den Objektarten gehören alle Objekte, die synchronisiert werden, einschließlich Lead, Kontakt, Konto, Chancen, Kampagne, Benutzer und benutzerdefinierte Objekte. Die Durchsatzstatistiken werden alle 15 Minuten automatisch aktualisiert. Sie können jedoch manuell mit dem Aktualisierungssymbol aktualisiert werden. Der Rückstand wird stündlich abgerufen.

>[!NOTE]
>
>Statistiken werden rollierend aktualisiert, nicht nach Kalendertag.

![](assets/salesforce-sync-backlog-metrics-4.png)

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

## Best Practices für die Verwaltung von Synchronisierungs-Backlogs {#best-practices}

**Für Benutzer synchronisieren sichtbare Felder**: Stellen Sie sicher, dass die zu synchronisierenden Felder nur diejenigen sind, die synchronisiert werden müssen, und dass sie für die Marketing-Maßnahmen von Nutzen sind. Jedes Update eines Datensatzes in Salesforce, das den letzten geänderten Zeitstempel aktualisiert, führt einen Datensatz in die Warteschlange des Synchronisierungs-Backlogs. Außerdem kann die Synchronisierung unnötiger Felder die Synchronisierung wichtiger Felder verlangsamen. Wenn die unnötigen Felder vom Synchronisierungsbenutzer ausgeblendet werden, führt eine Aktualisierung dieser Felder zu einem Überspringen, der viel schneller ist als eine Aktualisierung. Arbeiten Sie mit Ihrem Salesforce-Administrator zusammen, um hier die Best Practices zu überprüfen und zu aktualisieren, welche Felder für den Marketo Sync-Benutzer sichtbar sind.

**Ausblenden oder Filtern unnötiger Datensätze**: Wenn ein Datensatz nicht vermarktbar ist, verschwendet er möglicherweise Synchronisierungsressourcen. Wenn der Synchronisierungsbenutzer sie nicht sehen kann, werden keine Ressourcen verschwendet, die versucht haben, sie zu synchronisieren. [Marketo Engage-Unterstützung](https://nation.marketo.com/t5/support/ct-p/Support#_blank){target="_blank"} kann beim Einrichten eines Synchronisierungsfilters hilfreich sein, um die Synchronisierung von Datensätzen anhand zusätzlicher Kriterien zu verhindern. Weitere Informationen zum Einrichten eines benutzerdefinierten Synchronisierungsfilters [finden Sie hier](https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758){target="_blank"}. Es wird dringend empfohlen, Indexfelder in Salesforce zu verwenden (kontaktieren Sie Vertriebsmitarbeiter, um weitere Informationen zu erhalten).

**Planen Sie Massenaktualisierungen während nicht kritischer Stunden**: Überprüfen Sie Ihre Datensynchronisierungsmuster, um nicht kritische Zeiträume zu identifizieren. Überprüfen Sie, ob Massenaktualisierungen in diesen nicht kritischen Zeiträumen nach Möglichkeit geplant werden können.

**Häufig aktualisierte Felder**: Einige Felder sind anfällig für häufige Aktualisierungen. Beispielsweise Währungsfelder, die Währungsänderungen unterliegen. Überprüfen Sie, ob diese synchronisiert werden müssen oder ob die Felder anders gestaltet werden sollen. Wenn Sie andere Felder haben, die häufig aktualisiert werden und nicht benötigt werden, verbergen Sie sie vor dem Synchronisierungsbenutzer. Besprechen Sie mit Ihren SFDC-Admin-Integrationen, welche die Felder möglicherweise aktualisieren.

**Benutzerdefinierte Objekte**: Prüfen Sie regelmäßig die [benutzerdefinierten Objekte](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync){target="_blank"}, die zum Synchronisieren und Deaktivieren von Objekten aktiviert sind, die nicht mehr synchronisiert werden müssen.

**Aktivitäten**: [Überprüfen Sie, ob die Synchronisierung für Aktivitäten](https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/crm-sync/salesforce-sync/setup/optional-steps/customize-activities-sync){target="_blank"} aktiviert ist, die möglicherweise aus der Synchronisierung entfernt werden.  Diese Aktivitäten werden nur einmal pro Tag und Lead synchronisiert.

**Fehler bei der Überprüfungssynchronisierung**: Die Ausnahmebehandlung kann die Synchronisierung verlangsamen. Die Überprüfung von Benutzerbenachrichtigungen und die Fehlerbehebung können den Synchronisierungsstatus verbessern.

**Support kontaktieren**: Wenn Sie alle oben genannten Best Practices befolgen und weiterhin erhebliche Rückstände aufweisen, wenden Sie sich an den [Marketo Engage-Support](https://nation.marketo.com/t5/support/ct-p/Support#_blank){target="_blank"}.
