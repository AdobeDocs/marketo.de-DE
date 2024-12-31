---
unique-page-id: 14352541
description: Erstmaliges Synchronisieren von Sales Connect-Aufgaben mit Salesforce - Marketo-Dokumente - Produktdokumentation
title: Erstmaliges Synchronisieren von Sales Connect-Aufgaben mit Salesforce
exl-id: 42ac6b4f-76ac-40d7-9e10-7e0d3886a638
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Erstmaliges Synchronisieren von Sales Connect-Aufgaben mit Salesforce {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Wenn Sie die Synchronisierung zwischen Sales Connect- und Salesforce-Aufgaben zum ersten Mal aktivieren, importieren wir Ihre Salesforce-Aufgaben. Wir werden **nicht** alle aktuellen Aufgaben, die Sie in Sales Connect an Salesforce haben, übertragen. Um Übersichtlichkeit und Duplikate zu vermeiden, werden nur Aufgaben von Sales Connect mit Salesforce synchronisiert, *nachdem* Sie Sales Connect mit SFDC synchronisiert haben.

Folgendes passiert, wenn Sie Sales Connect- und SFDC-Aufgaben synchronisieren:

- Sobald Sie bei der Synchronisierung von Aufgaben auf Speichern klicken, beginnen sie mit der Synchronisierung. Dies wird zunächst einige Zeit in Anspruch nehmen.

- Alle Erinnerungen, die in den letzten 24 Stunden aktualisiert oder erstellt wurden, werden von SFDC an Sales Connect übertragen. Die Synchronisierung basiert auf dem Fälligkeitsdatum, und alle diese Aufgaben werden im Backend synchronisiert. Im Command Center werden jedoch nur Aufgaben angezeigt, die heute und morgen fällig sind.

- Wenn die Synchronisierung zuvor aktiviert wurde und Sie alle Aufgaben in SFDC löschen, werden alle in den letzten 15 Tagen gelöschten Elemente aus dem Command Center gelöscht.

- Solange die Synchronisierung aktiviert ist, werden Aufgaben zwischen Sales Connect und SFDC kontinuierlich synchronisiert.

Nach der ersten Synchronisierung werden alle Aufgaben, die Sie in Sales Connect erstellen, bearbeiten, abschließen oder löschen, mit Ihrer Aufgabenliste in Salesforce synchronisiert. Und alles, was in Salesforce erstellt, bearbeitet, abgeschlossen oder gelöscht wird, aktualisiert Ihre Aufgabenliste in Sales Connect.

Um diese Synchronisierung zu aktivieren, aktivieren Sie einfach das Kontrollkästchen Synchronisieren auf Ihrer [Einstellungsseite](https://toutapp.com/login) in der Web-Anwendung.
