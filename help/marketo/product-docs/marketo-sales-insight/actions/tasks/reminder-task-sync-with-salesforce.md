---
description: Erinnerungsaufgabe - Synchronisieren mit Salesforce - Marketo-Dokumente - Produktdokumentation
title: Erinnerungsaufgabe - Synchronisieren mit Salesforce
exl-id: 11aa6ab5-5489-4c20-a64d-2fd6fe29506f
feature: Sales Insight Actions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 2%

---

# Erinnerungsaufgabe - Synchronisieren mit Salesforce {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>Informationen zum Aktivieren der Aufgabensynchronisierung finden Sie unter [Synchronisieren von Sales Insight-Aktionen/Erinnerungen mit Salesforce-Aufgaben](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks).

Sobald die Einstellungen für die Aufgabensynchronisierung aktiviert sind, werden die Erinnerungsaufgaben bidirektional mit Salesforce synchronisiert. Das bedeutet, dass Anwender Aufgaben entweder über Salesforce oder über Sales Insight-Aktionen verwalten und darauf vertrauen können, dass die Systeme aufeinander abgestimmt bleiben.

## Erinnerungsaufgabe - Feldsynchronisierung {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

Nachstehend finden Sie eine Liste der Erinnerungsaufgabenfelder in Sales-Insight-Aktionen und den zugehörigen Salesforce-Feldern, die über die bidirektionale Aufgabensynchronisierung unterstützt werden.

<table>
 <tr>
  <th>Aufgabenfeld „Sales Insights-Aktionen“</th>
  <th>Salesforce-Aufgabenfeld</th>
  <th>Salesforce-Aufgabe</th>
 </tr>
 <tr>
  <td>Aufgabenname</td>
  <td>Betrefffeld</td>
  <td>Ein kurzes Zusammenfassungsfeld, das den Titel der Aufgabe anzeigen soll.</td>
 </tr>
 <tr>
  <td>Status</td>
  <td>Aufgabenstatus</td>
  <td><p>Zeigt den Status der Aufgabe an. Aufgaben für Sales Insights-Aktionen weisen zwei Status auf, die zwei Werten in der Salesforce-Aufgabenstatusauswahlliste zugeordnet sind.</p>
  <p>In Sales Insight-Aktionen öffnen = Nicht in Salesforce gestartet.</p>
  <p>Abgeschlossen in Sales Insight-Aktionen = Abgeschlossen in Salesforce.</p>
  <p>Die anderen Statuswerte in Salesforce werden nicht mit Sales Insight-Aktionen synchronisiert.</p></td>
 </tr>
 <tr>
  <td>Priorität</td>
  <td>Priorität</td>
  <td><p>Die Priorität für Sales Insight-Aktionen kann entweder Normal oder Hoch sein, was den Werten für Normal und Hoch Priorität in Salesforce entspricht.</p>
  <p>Der Wert mit niedriger Priorität in Salesforce wird nicht mit Sales Insight-Aktionen synchronisiert.</p></td>
 </tr>
 <tr>
  <td>Fälligkeitsdatum</td>
  <td>Fälligkeitsdatum</td>
  <td>Das Datum, an dem die Aufgabe fällig ist.</td>
 </tr>
 <tr>
  <td>Details</td>
  <td>Kommentare</td>
  <td>Zeigt detailliertere Informationen darüber an, was mit der Erinnerungsaufgabe abgeschlossen werden sollte.</td>
 </tr>
</table>

## Erstmaliges Synchronisieren von Sales Insight-Aktionsaufgaben mit Salesforce {#syncing-sales-insight-actions-tasks-with-salesforce-for-the-first-time}

Wenn Sie die Synchronisierung zwischen Sales Insight-Aktionen und Salesforce-Aufgaben zum ersten Mal aktivieren, importieren wir Ihre Salesforce-Aufgaben. Wir werden **nicht** alle aktuellen Aufgaben, die Sie in Sales Insight-Aktionen haben, an Salesforce weiterleiten. Um Übersichtlichkeit und Duplikate zu vermeiden, werden nur Aufgaben von Sales Insight-Aktionen in Salesforce synchronisiert, *nachdem* Sie Sales Insight-Aktionen mit SFDC synchronisiert haben.

Folgendes passiert, wenn Sie Sales Insight-Aktionen und SFDC-Aufgaben synchronisieren:

* Sobald Sie bei der Synchronisierung von Aufgaben auf Speichern klicken, beginnen sie mit der Synchronisierung. Dies wird zunächst einige Zeit in Anspruch nehmen.

* Alle Erinnerungen, die in den letzten 24 Stunden aktualisiert oder erstellt wurden, werden von SFDC zu Sales Insight-Aktionen abgerufen. Die Synchronisierung basiert auf dem Fälligkeitsdatum, und alle diese Aufgaben werden im Backend synchronisiert. Im Command Center werden jedoch nur Aufgaben angezeigt, die heute und morgen fällig sind.

* Wenn die Synchronisierung zuvor aktiviert wurde und Sie alle Aufgaben in SFDC löschen, werden alle in den letzten 15 Tagen gelöschten Elemente aus dem Command Center gelöscht.

* Solange die Synchronisierung aktiviert ist, synchronisieren wir Aufgaben zwischen Sales Insight-Aktionen und SFDC kontinuierlich.

Nach der ersten Synchronisierung werden alle Aufgaben, die Sie in Sales Insight-Aktionen erstellen, bearbeiten, abschließen oder löschen, mit Ihrer Aufgabenliste in Salesforce synchronisiert. Und alles, was in Salesforce erstellt, bearbeitet, abgeschlossen oder gelöscht wird, aktualisiert Ihre Aufgabenliste in Sales Insight-Aktionen.

Um diese Synchronisierung zu aktivieren, aktivieren Sie einfach das Kontrollkästchen Synchronisieren auf Ihrer [Einstellungsseite](https://toutapp.com/login) in der Web-Anwendung.

>[!NOTE]
>
>Das Betrefffeld einer Aufgabe kann in Sales Insight-Aktionen aktualisiert werden. Diese Aktualisierung wird im Betrefffeld von Salesforce für die entsprechende synchronisierte Aufgabe synchronisiert, wenn Sie das dynamische Feld &quot;`{{activity_subject}}`&quot; in Ihren Einstellungen [Anpassung von Aktivitätsdetails](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md) verwenden. Umgekehrt werden alle Aktualisierungen, die am Betrefffeld in Salesforce vorgenommen _,_ mit dem Betrefffeld der Erinnerungsaufgabe für Sales Insight-Aktionen synchronisiert.
