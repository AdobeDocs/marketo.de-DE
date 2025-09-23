---
description: Erinnerungsaufgabe - Synchronisieren mit Salesforce - Marketo-Dokumente - Produktdokumentation
title: Synchronisieren von Erinnerungsaufgaben mit Salesforce
exl-id: 4de933db-4626-4845-be70-8ad55d03a18e
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 1%

---

# Erinnerungsaufgabe - Synchronisieren mit [!DNL Salesforce] {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>Informationen zum Aktivieren der Aufgabensynchronisierung finden Sie unter [Synchronisieren [!DNL Sales Connect] Aufgaben/Erinnerungen an [!DNL Salesforce] Aufgaben](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md#sync-sales-connect-tasks-reminders-to-salesforce-tasks).

Sobald die Einstellungen für die Aufgabensynchronisierung aktiviert sind, werden die Erinnerungsaufgaben bidirektional mit [!DNL Salesforce] synchronisiert. Das bedeutet, dass Benutzer Aufgaben entweder aus [!DNL Salesforce] oder aus [!DNL Sales Connect] verwalten können und darauf vertrauen können, dass die Systeme aufeinander abgestimmt bleiben.

## Erinnerungsaufgabe - Feldsynchronisierung {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

Nachstehend finden Sie eine Liste der Erinnerungsaufgabenfelder in [!DNL Sales Connect] und der entsprechenden [!DNL Salesforce], die von der bidirektionalen Aufgabensynchronisierung unterstützt werden.

<table>
 <tr>
  <th>[!DNL Sales Connect] Aufgabenfeld</th>
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
  <td><p>Zeigt den Status der Aufgabe an. [!DNL Sales Connect] Aufgaben haben zwei Status, die zwei Werten in der Auswahlliste [!DNL Salesforce] Aufgabenstatus zugeordnet sind.</p>
  <p>Öffnen in [!DNL Sales Connect] = Nicht gestartet in [!DNL Salesforce].</p>
  <p>Abgeschlossen in [!DNL Sales Connect] = Abgeschlossen in [!DNL Salesforce].</p>
  <p>Die anderen Statuswerte in [!DNL Salesforce] werden nicht mit [!DNL Sales Connect] synchronisiert.</p></td>
 </tr>
 <tr>
  <td>[!UICONTROL-Priorität]</td>
  <td>[!UICONTROL-Priorität]</td>
  <td><p>[!DNL Sales Connect] Die Priorität kann entweder Normal oder Hoch sein, was den Werten mit normaler und hoher Priorität in [!DNL Salesforce] entspricht.</p>
  <p>Der Wert für die niedrige Priorität in [!DNL Salesforce] wird nicht mit [!DNL Sales Connect] synchronisiert.</p></td>
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

## Erstmaliges Synchronisieren [!DNL Sales Connect] Aufgaben mit [!DNL Salesforce] {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Wenn Sie die Synchronisierung zwischen [!DNL Sales Connect] und [!DNL Salesforce] Aufgaben zum ersten Mal aktivieren, importieren wir Ihre [!DNL Salesforce] Aufgaben. Wir werden **nicht** alle aktuellen Aufgaben, die Sie in [!DNL Sales Connect] haben, an [!DNL Salesforce] weiterleiten. Um Übersichtlichkeit und Duplikate zu vermeiden, werden nur Aufgaben von [!DNL Sales Connect] in [!DNL Salesforce] synchronisiert, die *nach* der Synchronisierung von [!DNL Sales Connect] mit SFDC erstellt werden.

Folgendes passiert, wenn Sie [!DNL Sales Connect]- und SFDC-Aufgaben synchronisieren:

* Sobald Sie bei der Synchronisierung von Aufgaben auf Speichern klicken, beginnen sie mit der Synchronisierung. Dies wird zunächst einige Zeit in Anspruch nehmen.

* Alle Erinnerungen, die in den letzten 24 Stunden aktualisiert oder erstellt wurden, werden von SFDC nach [!DNL Sales Connect] übertragen. Die Synchronisierung basiert auf dem Fälligkeitsdatum, und alle diese Aufgaben werden im Backend synchronisiert. Im Command Center werden jedoch nur Aufgaben angezeigt, die heute und morgen fällig sind.

* Wenn die Synchronisierung zuvor aktiviert wurde und Sie alle Aufgaben in SFDC löschen, werden alle in den letzten 15 Tagen gelöschten Elemente aus dem Command Center gelöscht.

* Wir synchronisieren Aufgaben zwischen [!DNL Sales Connect] und SFDC kontinuierlich, solange die Synchronisierung aktiviert ist.

Nach der ersten Synchronisierung werden alle Aufgaben, die Sie in [!DNL Sales Connect] erstellen, bearbeiten, abschließen oder löschen, mit Ihrer Aufgabenliste in [!DNL Salesforce] synchronisiert. Und alles, was in [!DNL Salesforce] erstellt, bearbeitet, abgeschlossen oder gelöscht wird, aktualisiert Ihre Aufgabenliste in [!DNL Sales Connect].

Um diese Synchronisierung zu aktivieren, aktivieren Sie einfach das Kontrollkästchen Synchronisieren auf Ihrer [Einstellungsseite](https://toutapp.com/login) in der Web-Anwendung.

>[!NOTE]
>
>Das Betrefffeld einer Aufgabe kann in [!DNL Sales Connect] aktualisiert werden. Diese Aktualisierung wird im [!DNL Salesforce] Betrefffeld für die entsprechende synchronisierte Aufgabe synchronisiert, wenn Sie das dynamische Feld `{{activity_subject}}` in Ihren Einstellungen [Anpassung von Aktivitätsdetails](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md) verwenden. Umgekehrt werden alle Aktualisierungen, die am Betrefffeld in [!DNL Salesforce] vorgenommen *,* mit dem Betrefffeld [!DNL Sales Connect] Erinnerungsaufgabe synchronisiert.
