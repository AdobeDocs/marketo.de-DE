---
description: Erinnerungsaufgabe - Synchronisieren mit Salesforce - Marketo-Dokumente - Produktdokumentation
title: Erinnerungsaufgabe - Synchronisieren mit Salesforce
exl-id: 4de933db-4626-4845-be70-8ad55d03a18e
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 2%

---

# Erinnerungsaufgabe - Synchronisieren mit Salesforce {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>Informationen zum Aktivieren der Aufgabensynchronisierung finden Sie unter [Synchronisieren von Verkaufsaufgaben/Erinnerungen mit Salesforce-Aufgaben](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md#sync-sales-connect-tasks-reminders-to-salesforce-tasks).

Sobald die Einstellungen für die Aufgabensynchronisierung aktiviert sind, werden die Erinnerungsaufgaben bidirektional mit Salesforce synchronisiert. Das bedeutet, dass Anwender Aufgaben entweder über Salesforce oder Sales Connect verwalten und darauf vertrauen können, dass die Systeme aufeinander abgestimmt bleiben.

## Erinnerungsaufgabe - Feldsynchronisierung {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

Nachstehend finden Sie eine Liste der Erinnerungsaufgabenfelder in Sales Connect und die zugehörigen Salesforce-Felder, die über die bidirektionale Aufgabensynchronisierung unterstützt werden.

<table>
 <tr>
  <th>Aufgabenfeld „Verkaufsverbindung“</th>
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
  <td><p>Zeigt den Status der Aufgabe an. Sales Connect-Aufgaben haben zwei Status, die zwei Werten in der Salesforce-Aufgabenstatusauswahlliste zugeordnet sind.</p>
  <p>In Sales Connect öffnen = Nicht in Salesforce gestartet.</p>
  <p>Abgeschlossen in Sales Connect = Abgeschlossen in Salesforce.</p>
  <p>Die anderen Statuswerte in Salesforce werden nicht mit Sales Connect synchronisiert.</p></td>
 </tr>
 <tr>
  <td>Priorität</td>
  <td>Priorität</td>
  <td><p>Die Sales Connect-Priorität kann entweder Normal oder Hoch sein, was den normalen und hohen Prioritätswerten in Salesforce zugeordnet wird.</p>
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

## Erstmaliges Synchronisieren von Sales Connect-Aufgaben mit Salesforce {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Wenn Sie die Synchronisierung zwischen Sales Connect- und Salesforce-Aufgaben zum ersten Mal aktivieren, importieren wir Ihre Salesforce-Aufgaben. Wir werden **nicht** alle aktuellen Aufgaben, die Sie in Sales Connect an Salesforce haben, übertragen. Um Übersichtlichkeit und Duplikate zu vermeiden, werden nur Aufgaben von Sales Connect mit Salesforce synchronisiert, *nachdem* Sie Sales Connect mit SFDC synchronisiert haben.

Folgendes passiert, wenn Sie Sales Connect- und SFDC-Aufgaben synchronisieren:

* Sobald Sie bei der Synchronisierung von Aufgaben auf Speichern klicken, beginnen sie mit der Synchronisierung. Dies wird zunächst einige Zeit in Anspruch nehmen.

* Alle Erinnerungen, die in den letzten 24 Stunden aktualisiert oder erstellt wurden, werden von SFDC an Sales Connect übertragen. Die Synchronisierung basiert auf dem Fälligkeitsdatum, und alle diese Aufgaben werden im Backend synchronisiert. Im Command Center werden jedoch nur Aufgaben angezeigt, die heute und morgen fällig sind.

* Wenn die Synchronisierung zuvor aktiviert wurde und Sie alle Aufgaben in SFDC löschen, werden alle in den letzten 15 Tagen gelöschten Elemente aus dem Command Center gelöscht.

* Solange die Synchronisierung aktiviert ist, werden Aufgaben zwischen Sales Connect und SFDC kontinuierlich synchronisiert.

Nach der ersten Synchronisierung werden alle Aufgaben, die Sie in Sales Connect erstellen, bearbeiten, abschließen oder löschen, mit Ihrer Aufgabenliste in Salesforce synchronisiert. Und alles, was in Salesforce erstellt, bearbeitet, abgeschlossen oder gelöscht wird, aktualisiert Ihre Aufgabenliste in Sales Connect.

Um diese Synchronisierung zu aktivieren, aktivieren Sie einfach das Kontrollkästchen Synchronisieren auf Ihrer [Einstellungsseite](https://toutapp.com/login) in der Web-Anwendung.

>[!NOTE]
>
>Das Betrefffeld einer Aufgabe kann in Sales Connect aktualisiert werden. Diese Aktualisierung wird im Betrefffeld von Salesforce für die entsprechende synchronisierte Aufgabe synchronisiert, wenn Sie das dynamische Feld &quot;`{{activity_subject}}`&quot; in Ihren Einstellungen [Aktivitätsdetailanpassung](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md) verwenden. Umgekehrt werden alle Aktualisierungen, die am Betrefffeld in Salesforce vorgenommen _,_ mit dem Betrefffeld der Sales Connect-Erinnerungsaufgabe synchronisiert.
