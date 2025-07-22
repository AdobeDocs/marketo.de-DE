---
unique-page-id: 14352541
description: Erstmaliges Synchronisieren von Sales Connect-Aufgaben mit Salesforce - Marketo-Dokumente - Produktdokumentation
title: Erstmaliges Synchronisieren von Sales Connect-Aufgaben mit Salesforce
exl-id: 42ac6b4f-76ac-40d7-9e10-7e0d3886a638
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# Erstmaliges Synchronisieren [!DNL Sales Connect] Aufgaben mit [!DNL Salesforce] {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Wenn Sie die Synchronisierung zwischen [!DNL Sales Connect] und [!DNL Salesforce] Aufgaben zum ersten Mal aktivieren, importieren wir Ihre [!DNL Salesforce] Aufgaben. Wir werden **nicht** alle aktuellen Aufgaben, die Sie in [!DNL Sales Connect] haben, an [!DNL Salesforce] weiterleiten. Um Übersichtlichkeit und Duplikate zu vermeiden, werden nur Aufgaben von [!DNL Sales Connect] in [!DNL Salesforce] synchronisiert, die *nach* der Synchronisierung von [!DNL Sales Connect] mit SFDC erstellt werden.

Folgendes passiert, wenn Sie [!DNL Sales Connect]- und SFDC-Aufgaben synchronisieren:

- Sobald Sie bei der Synchronisierung von Aufgaben auf Speichern klicken, beginnen sie mit der Synchronisierung. Dies wird zunächst einige Zeit in Anspruch nehmen.

- Alle Erinnerungen, die in den letzten 24 Stunden aktualisiert oder erstellt wurden, werden von SFDC nach [!DNL Sales Connect] übertragen. Die Synchronisierung basiert auf dem Fälligkeitsdatum, und alle diese Aufgaben werden im Backend synchronisiert. Im Command Center werden jedoch nur Aufgaben angezeigt, die heute und morgen fällig sind.

- Wenn die Synchronisierung zuvor aktiviert wurde und Sie alle Aufgaben in SFDC löschen, werden alle in den letzten 15 Tagen gelöschten Elemente aus dem Command Center gelöscht.

- Wir synchronisieren Aufgaben zwischen [!DNL Sales Connect] und SFDC kontinuierlich, solange die Synchronisierung aktiviert ist.

Nach der ersten Synchronisierung werden alle Aufgaben, die Sie in [!DNL Sales Connect] erstellen, bearbeiten, abschließen oder löschen, mit Ihrer Aufgabenliste in [!DNL Salesforce] synchronisiert. Und alles, was in [!DNL Salesforce] erstellt, bearbeitet, abgeschlossen oder gelöscht wird, aktualisiert Ihre Aufgabenliste in [!DNL Sales Connect].

Um diese Synchronisierung zu aktivieren, aktivieren Sie einfach das Kontrollkästchen Synchronisieren auf Ihrer [Einstellungsseite](https://toutapp.com/login) in der Web-Anwendung.
