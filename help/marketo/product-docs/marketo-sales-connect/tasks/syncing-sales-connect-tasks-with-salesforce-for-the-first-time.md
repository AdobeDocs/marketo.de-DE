---
unique-page-id: 14352541
description: Synchronisieren von Sales Connect-Aufgaben mit Salesforce zum ersten Mal - Marketo Docs - Produktdokumentation
title: Synchronisieren von Sales Connect-Aufgaben mit Salesforce zum ersten Mal
exl-id: 42ac6b4f-76ac-40d7-9e10-7e0d3886a638
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Synchronisieren von Sales Connect-Aufgaben mit Salesforce zum ersten Mal {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Wenn Sie die Synchronisierung zwischen Sales Connect- und Salesforce-Aufgaben zum ersten Mal aktivieren, importieren wir Ihre Salesforce-Aufgaben. Wir werden **not** Übertragen Sie alle aktuellen Aufgaben, die Sie in Sales Connect haben, in Salesforce. Um Übersichtlichkeit und Duplikate zu reduzieren, werden nur Aufgaben erstellt, die von Sales Connect mit Salesforce synchronisiert werden *after* Sie synchronisieren Sales Connect mit SFDC.

Folgendes geschieht, wenn Sie Sales Connect- und SFDC-Aufgaben synchronisieren:

- Sobald Sie auf Bei der Aufgabensynchronisierung speichern klicken, beginnen sie mit der Synchronisierung. Dies wird zunächst einige Zeit in Anspruch nehmen.

- Alle Erinnerungen, die in den letzten 24 Stunden aktualisiert oder erstellt wurden, werden von SFDC an Sales Connect abgerufen. Die Synchronisation basiert auf dem Fälligkeitsdatum und alle diese Aufgaben werden im Backend synchronisiert, aber im Command Center werden nur noch Aufgaben angezeigt, die heute und morgen fällig sind.

- Wenn die Synchronisierung zuvor aktiviert wurde und Sie alle Aufgaben in SFDC löschen, werden alle Elemente, die in den letzten 15 Tagen gelöscht wurden, aus Command Center gelöscht.

- Solange die Synchronisierung aktiviert ist, synchronisieren wir ständig Aufgaben zwischen Sales Connect und SFDC.

Nach der ersten Synchronisierung werden alle Aufgaben, die Sie in Sales Connect erstellen, bearbeiten, abschließen oder löschen, mit Ihrer Aufgabenliste in Salesforce synchronisiert. Und alles, was in Salesforce erstellt, bearbeitet, abgeschlossen oder gelöscht wurde, aktualisiert Ihre Aufgabenliste in Sales Connect.

Um diese Synchronisierung zu aktivieren, aktivieren Sie einfach das Synchronisierungsfeld in Ihrem [Einstellungsseite](https://toutapp.com/login) in der Webanwendung.
