---
description: Reminder Task Sync with Salesforce - Marketo Docs - Produktdokumentation
title: Erinnern von Aufgabensynchronisierung mit Salesforce
exl-id: 4de933db-4626-4845-be70-8ad55d03a18e
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 2%

---

# Erinnern von Aufgabensynchronisierung mit Salesforce {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>Um zu erfahren, wie Sie die Aufgabensynchronisierung aktivieren, sehen Sie sich die Informationen unter [Aufgaben/Erinnerungen für die Vertriebsverbindung mit Salesforce-Aufgaben synchronisieren](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md#sync-sales-connect-tasks-reminders-to-salesforce-tasks) an.

Sobald die Einstellungen für die Aufgabensynchronisierung aktiviert sind, sehen die Benutzer ihre Erinnerungsaufgaben bidirektional mit Salesforce synchronisiert. Dies bedeutet, dass Benutzer Aufgaben entweder über Salesforce oder Sales Connect verwalten können und sicher sind, dass die Systeme aufeinander abgestimmt bleiben.

## Reminder Task Field Sync {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

Im Folgenden finden Sie eine Liste der Erinnerungsaufgaben-Felder in Sales Connect und der zugehörigen Salesforce-Felder, die über die bidirektionale Aufgabensynchronisierung unterstützt werden.

<table>
 <tr>
  <th>Aufgabenfeld "Sales Connect"</th>
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
  <td><p>Zeigt den Status der Aufgabe an. Sales Connect -Aufgaben haben zwei Status, die zwei der Werte in der Liste der Aufgabenstatus-Auswahl in Salesforce zuordnen.</p>
  <p>Öffnen Sie in Sales Connect = Not Started in Salesforce.</p>
  <p>Abgeschlossen in Sales Connect = Abgeschlossen in Salesforce.</p>
  <p>Die anderen Statuswerte in Salesforce werden nicht mit Sales Connect synchronisiert.</p></td>
 </tr>
 <tr>
  <td>Priorität</td>
  <td>Priorität</td>
  <td><p>Die Priorität von Sales Connect kann entweder "Normal"oder "Hoch"lauten, die den Prioritätswerten Normal und Hoch in Salesforce zugeordnet sind.</p>
  <p>Der Wert mit niedriger Priorität in Salesforce wird nicht mit Sales Connect synchronisiert.</p></td>
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

## Synchronisieren von Sales Connect-Aufgaben mit Salesforce zum ersten Mal {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Wenn Sie die Synchronisierung zwischen Sales Connect- und Salesforce-Aufgaben zum ersten Mal aktivieren, importieren wir Ihre Salesforce-Aufgaben. Wir übernehmen **nicht** alle aktuellen Aufgaben, die Sie in Sales Connect haben, mit Salesforce. Um Übersichtlichkeit und Duplikate zu reduzieren, sind die einzigen Aufgaben, die von Sales Connect mit Salesforce synchronisiert werden, Aufgaben, die *nach* der Synchronisierung von Sales Connect mit SFDC erstellt wurden.

Folgendes geschieht, wenn Sie Sales Connect- und SFDC-Aufgaben synchronisieren:

* Sobald Sie auf Bei der Aufgabensynchronisierung speichern klicken, beginnen sie mit der Synchronisierung. Dies wird zunächst einige Zeit in Anspruch nehmen.

* Alle Erinnerungen, die in den letzten 24 Stunden aktualisiert oder erstellt wurden, werden von SFDC an Sales Connect abgerufen. Die Synchronisation basiert auf dem Fälligkeitsdatum und alle diese Aufgaben werden im Backend synchronisiert, aber im Command Center werden nur noch Aufgaben angezeigt, die heute und morgen fällig sind.

* Wenn die Synchronisierung zuvor aktiviert wurde und Sie alle Aufgaben in SFDC löschen, werden alle Elemente, die in den letzten 15 Tagen gelöscht wurden, aus Command Center gelöscht.

* Solange die Synchronisierung aktiviert ist, synchronisieren wir ständig Aufgaben zwischen Sales Connect und SFDC.

Nach der ersten Synchronisierung werden alle Aufgaben, die Sie in Sales Connect erstellen, bearbeiten, abschließen oder löschen, mit Ihrer Aufgabenliste in Salesforce synchronisiert. Und alles, was in Salesforce erstellt, bearbeitet, abgeschlossen oder gelöscht wurde, aktualisiert Ihre Aufgabenliste in Sales Connect.

Um diese Synchronisierung zu aktivieren, aktivieren Sie einfach das Kontrollkästchen &quot;Synchronisieren&quot;auf Ihrer [Einstellungsseite](https://toutapp.com/login) in der Webanwendung.

>[!NOTE]
>
>Das Betrefffeld einer Aufgabe kann in Sales Connect aktualisiert werden. Dieses Update wird im Betrefffeld Salesforce für die entsprechende synchronisierte Aufgabe synchronisiert, wenn Sie das dynamische Feld `{{activity_subject}}` in Ihren Einstellungen für die [Anpassung der Aktivitätsdetails](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md) verwenden. Umgekehrt werden alle Aktualisierungen am Betrefffeld in Salesforce _nicht_ mit dem Betrefffeld der Erinnerungsaufgabe für Sales Connect synchronisiert.
