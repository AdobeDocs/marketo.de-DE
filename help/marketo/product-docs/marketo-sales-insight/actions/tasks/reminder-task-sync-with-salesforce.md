---
description: Erinnerungsaufgabe - Synchronisieren mit Salesforce - Marketo-Dokumente - Produktdokumentation
title: Erinnerungsaufgabe - Synchronisieren mit Salesforce
exl-id: 11aa6ab5-5489-4c20-a64d-2fd6fe29506f
feature: Sales Insight Actions
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# Erinnerungsaufgabe - Synchronisieren mit [!DNL Salesforce] {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>Informationen zum Aktivieren der Aufgabensynchronisierung finden Sie unter [Synchronisieren von Insight-Aktionsaufgaben/-Erinnerungen mit Salesforce-Aufgaben](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks).

Sobald die Einstellungen für die Aufgabensynchronisierung aktiviert sind, werden die Erinnerungsaufgaben bidirektional mit [!DNL Salesforce] synchronisiert. Das bedeutet, dass Benutzer Aufgaben entweder aus [!DNL Salesforce] oder aus [!DNL Sales Insight Actions] verwalten können und darauf vertrauen können, dass die Systeme aufeinander abgestimmt bleiben.

## Erinnerungsaufgabe - Feldsynchronisierung {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

Nachstehend finden Sie eine Liste der Erinnerungsaufgabenfelder in [!DNL Sales Insight Actions] und der entsprechenden [!DNL Salesforce], die von der bidirektionalen Aufgabensynchronisierung unterstützt werden.

<table>
 <tr>
  <th>[!DNL Sales Insight Actions] Aufgabenfeld</th>
  <th>[!DNL Salesforce] Aufgabenfeld</th>
  <th>[!DNL Salesforce] Aufgabe</th>
 </tr>
 <tr>
  <td>[!UICONTROL Aufgabenname]</td>
  <td>[!UICONTROL Betrefffeld]</td>
  <td>Ein kurzes Zusammenfassungsfeld, das den Titel der Aufgabe anzeigen soll.</td>
 </tr>
 <tr>
  <td>[!UICONTROL Status]</td>
  <td>[!UICONTROL Aufgabenstatus]</td>
  <td><p>Zeigt den Status der Aufgabe an. [!DNL Sales Insight Actions] Aufgaben haben zwei Status, die zwei Werten in der Auswahlliste [!DNL Salesforce] Aufgabenstatus zugeordnet sind.</p>
  <p>Öffnen in [!DNL Sales Insight Actions] = Nicht gestartet in [!DNL Salesforce].</p>
  <p>Abgeschlossen in [!DNL Sales Insight Actions] = Abgeschlossen in [!DNL Salesforce].</p>
  <p>Die anderen Statuswerte in [!DNL Salesforce] werden nicht mit [!DNL Sales Insight Actions] synchronisiert.</p></td>
 </tr>
 <tr>
  <td>[!UICONTROL -Priorität]</td>
  <td>[!UICONTROL -Priorität]</td>
  <td><p>[!DNL Sales Insight Actions] Die Priorität kann entweder Normal oder Hoch sein, was den Werten mit normaler und hoher Priorität in [!DNL Salesforce] entspricht.</p>
  <p>Der Wert für die niedrige Priorität in [!DNL Salesforce] wird nicht mit [!DNL Sales Insight Actions] synchronisiert.</p></td>
 </tr>
 <tr>
  <td>[!UICONTROL Fälligkeitsdatum]</td>
  <td>[!UICONTROL Fälligkeitsdatum]</td>
  <td>Das Datum, an dem die Aufgabe fällig ist.</td>
 </tr>
 <tr>
  <td>[!UICONTROL Details]</td>
  <td>[!UICONTROL Kommentare]</td>
  <td>Zeigt detailliertere Informationen darüber an, was mit der Erinnerungsaufgabe abgeschlossen werden sollte.</td>
 </tr>
</table>

## Erstmaliges Synchronisieren [!DNL Sales Insight Actions] Aufgaben mit [!DNL Salesforce] {#syncing-sales-insight-actions-tasks-with-salesforce-for-the-first-time}

Wenn Sie die Synchronisierung zwischen [!DNL Sales Insight Actions] und [!DNL Salesforce] Aufgaben zum ersten Mal aktivieren, importieren wir Ihre [!DNL Salesforce] Aufgaben. Wir werden **nicht** alle aktuellen Aufgaben, die Sie in [!DNL Sales Insight Actions] haben, an [!DNL Salesforce] weiterleiten. Um Übersichtlichkeit und Duplikate zu vermeiden, werden nur Aufgaben von [!DNL Sales Insight Actions] in [!DNL Salesforce] synchronisiert, die *nach* der Synchronisierung von [!DNL Sales Insight Actions] mit SFDC erstellt werden.

Folgendes passiert, wenn Sie [!DNL Sales Insight Actions]- und SFDC-Aufgaben synchronisieren:

* Sobald Sie bei der Synchronisierung von Aufgaben auf Speichern klicken, beginnen sie mit der Synchronisierung. Dies wird zunächst einige Zeit in Anspruch nehmen.

* Alle Erinnerungen, die in den letzten 24 Stunden aktualisiert oder erstellt wurden, werden von SFDC nach [!DNL Sales Insight Actions] übertragen. Die Synchronisierung basiert auf dem Fälligkeitsdatum, und alle diese Aufgaben werden im Backend synchronisiert. Im Command Center werden jedoch nur Aufgaben angezeigt, die heute und morgen fällig sind.

* Wenn die Synchronisierung zuvor aktiviert wurde und Sie alle Aufgaben in SFDC löschen, werden alle in den letzten 15 Tagen gelöschten Elemente aus dem Command Center gelöscht.

* Wir synchronisieren Aufgaben zwischen [!DNL Sales Insight Actions] und SFDC kontinuierlich, solange die Synchronisierung aktiviert ist.

Nach der ersten Synchronisierung werden alle Aufgaben, die Sie in [!DNL Sales Insight Actions] erstellen, bearbeiten, abschließen oder löschen, mit Ihrer Aufgabenliste in [!DNL Salesforce] synchronisiert. Und alles, was in [!DNL Salesforce] erstellt, bearbeitet, abgeschlossen oder gelöscht wird, aktualisiert Ihre Aufgabenliste in [!DNL Sales Insight Actions].

Um diese Synchronisierung zu aktivieren, aktivieren Sie einfach das Kontrollkästchen Synchronisieren auf Ihrer [Einstellungsseite](https://toutapp.com/login) in der Web-Anwendung.

>[!NOTE]
>
>Das Betrefffeld einer Aufgabe kann in [!DNL Sales Insight Actions] aktualisiert werden. Diese Aktualisierung wird im [!DNL Salesforce] Betrefffeld für die entsprechende synchronisierte Aufgabe synchronisiert, wenn Sie das dynamische Feld `{{activity_subject}}` in Ihren Einstellungen [Anpassung von Aktivitätsdetails](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md) verwenden. Umgekehrt werden alle Aktualisierungen, die am Betrefffeld in [!DNL Salesforce] vorgenommen _,_ mit dem Betrefffeld [!DNL Sales Insight Actions] Erinnerungsaufgabe synchronisiert.
