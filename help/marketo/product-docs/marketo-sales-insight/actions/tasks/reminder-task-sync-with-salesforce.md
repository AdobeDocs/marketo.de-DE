---
description: Reminder Task Sync with Salesforce - Marketo Docs - Produktdokumentation
title: Erinnern von Aufgabensynchronisierung mit Salesforce
exl-id: 11aa6ab5-5489-4c20-a64d-2fd6fe29506f
feature: Sales Insight Actions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 2%

---

# Erinnern von Aufgabensynchronisierung mit Salesforce {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>So erfahren Sie, wie Sie das Auschecken von Aufgaben aktivieren [Synchronisieren von Sales Insight-Aktionsaufgaben/-Erinnerungen mit Salesforce-Aufgaben](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks).

Sobald die Einstellungen für die Aufgabensynchronisierung aktiviert sind, sehen die Benutzer ihre Erinnerungsaufgaben bidirektional mit Salesforce synchronisiert. Dies bedeutet, dass Benutzer Aufgaben entweder über Salesforce- oder Sales Insight-Aktionen verwalten können und zuversichtlich sind, dass die Systeme aufeinander abgestimmt bleiben.

## Reminder Task Field Sync {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

Nachstehend finden Sie eine Liste der Erinnerungsaufgaben-Felder in Sales Insight-Aktionen und der zugehörigen Salesforce-Felder, die über die bidirektionale Aufgabensynchronisierung unterstützt werden.

<table>
 <tr>
  <th>Task-Feld "Sales Insight-Aktionen"</th>
  <th>Salesforce Task Field</th>
  <th>Salesforce-Aufgabe</th>
 </tr>
 <tr>
  <td>Aufgabenname</td>
  <td>Themenfeld</td>
  <td>Ein kurzes Zusammenfassungsfeld, das den Titel der Aufgabe anzeigen soll.</td>
 </tr>
 <tr>
  <td>Status</td>
  <td>Aufgabenstatus</td>
  <td><p>Zeigt den Status der Aufgabe an. Sales Insight-Aktionsaufgaben verfügen über zwei Status, die zwei der Werte in der Liste für den Status der Salesforce-Aufgaben zuordnen.</p>
  <p>Öffnen Sie in Sales Insight Actions = Not Started in Salesforce.</p>
  <p>Abgeschlossen in Sales Insight-Aktionen = Abgeschlossen in Salesforce.</p>
  <p>Die anderen Statuswerte in Salesforce werden nicht mit Sales Insight-Aktionen synchronisiert.</p></td>
 </tr>
 <tr>
  <td>Priorität</td>
  <td>Priorität</td>
  <td><p>Die Priorität von Sales Insight-Aktionen kann entweder "Normal"oder "Hoch"lauten, die den Prioritätswerten Normal und Hoch in Salesforce zugeordnet sind.</p>
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

## Synchronisieren von Sales Insight-Aktionsaufgaben mit Salesforce zum ersten Mal {#syncing-sales-insight-actions-tasks-with-salesforce-for-the-first-time}

Wenn Sie die Synchronisierung zwischen Sales Insight-Aktionen und Salesforce-Aufgaben zum ersten Mal aktivieren, importieren wir Ihre Salesforce-Aufgaben. Wir werden **not** Übertragen Sie alle aktuellen Aufgaben, die Sie in Sales Insight-Aktionen haben, in Salesforce. Um Übersichtlichkeit und Duplikate zu reduzieren, werden nur Aufgaben erstellt, die aus Sales Insight-Aktionen in Salesforce synchronisiert werden *after* Sie synchronisieren Sales Insight-Aktionen mit SFDC.

Folgendes passiert, wenn Sie Sales Insight-Aktionen und SFDC-Aufgaben synchronisieren:

* Sobald Sie auf Bei der Aufgabensynchronisierung speichern klicken, beginnen sie mit der Synchronisierung. Dies wird zunächst einige Zeit in Anspruch nehmen.

* Alle Erinnerungen, die in den letzten 24 Stunden aktualisiert oder erstellt wurden, werden von SFDC zu Sales Insight-Aktionen abgerufen. Die Synchronisation basiert auf dem Fälligkeitsdatum und alle diese Aufgaben werden im Backend synchronisiert, aber im Command Center werden nur noch Aufgaben angezeigt, die heute und morgen fällig sind.

* Wenn die Synchronisierung zuvor aktiviert wurde und Sie alle Aufgaben in SFDC löschen, werden alle Elemente, die in den letzten 15 Tagen gelöscht wurden, aus Command Center gelöscht.

* Solange die Synchronisierung aktiviert ist, synchronisieren wir ständig Aufgaben zwischen Sales Insight Actions und SFDC.

Nach der ersten Synchronisierung werden alle Aufgaben, die Sie in Sales Insight-Aktionen erstellen, bearbeiten, abschließen oder löschen, mit Ihrer Aufgabenliste in Salesforce synchronisiert. Und alles, was in Salesforce erstellt, bearbeitet, abgeschlossen oder gelöscht wurde, aktualisiert Ihre Aufgabenliste in Sales Insight-Aktionen.

Um diese Synchronisierung zu aktivieren, aktivieren Sie einfach das Synchronisierungsfeld in Ihrem [Einstellungsseite](https://toutapp.com/login) in der Webanwendung.

>[!NOTE]
>
>Das Betrefffeld einer Aufgabe kann in Sales Insight-Aktionen aktualisiert werden. Diese Aktualisierung wird im Salesforce-Betrefffeld für die entsprechende synchronisierte Aufgabe synchronisiert, wenn Sie die `{{activity_subject}}` dynamisches Feld in [Anpassung der Aktivitätsdetails](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md) -Einstellungen. Umgekehrt werden alle Aktualisierungen am Betrefffeld in Salesforce _not_ Synchronisieren Sie mit dem Erinnerungsbetreff der Aufgabe &quot;Sales Insight-Aktionen&quot;.
