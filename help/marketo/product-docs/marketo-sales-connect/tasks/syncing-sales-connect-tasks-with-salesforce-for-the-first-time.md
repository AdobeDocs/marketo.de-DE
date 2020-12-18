---
unique-page-id: 14352541
description: Synchronisieren von Sales Connect-Aufgaben mit Salesforce zum ersten Mal - Marketing Docs - Produktdokumentation
title: Aufgaben mit Salesforce zum ersten Mal synchronisieren
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---


# Synchronisieren von Sales Connect-Aufgaben mit Salesforce zum ersten Mal {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Wenn Sie zum ersten Mal die Synchronisierung zwischen Sales Connect- und Salesforce-Aufgaben aktivieren, importieren wir Ihre Salesforce-Aufgaben. Wir werden **nicht** alle aktuellen Aufgaben, die Sie in Sales Connect zu Salesforce haben, übergeben. Zur Vermeidung von Unübersichtlichkeit und Duplikaten sind die einzigen Aufgaben, die von Sales Connect mit Salesforce synchronisiert werden, Aufgaben, die *nach* der Synchronisierung von Sales Connect mit SFDC erstellt wurden.

Folgendes passiert, wenn Sie Sales Connect- und SFDC-Aufgaben synchronisieren:

- Sobald Sie bei der Synchronisierung der Aufgaben auf Speichern klicken, beginnen sie zu synchronisieren. Das wird zunächst einige Zeit dauern.

- Alle Erinnerungen, die in `last 24 hours` aktualisiert oder erstellt wurden, werden von SFDC zu Sales Connect abgerufen. Die Synchronisierung basiert auf `due date` und alle diese Aufgaben werden im Back-End synchronisiert, aber im Command Center werden nur noch Aufgaben angezeigt, die heute und morgen fällig sind.

- Wenn die Synchronisierung zuvor aktiviert wurde und Sie alle Aufgaben im SFDC löschen, wird alles, was in den letzten 15 Tagen gelöscht wurde, aus dem Command Center gelöscht.

- Solange die Synchronisierung aktiviert ist, synchronisieren wir die Aufgaben zwischen Sales Connect und SFDC ständig.

Nach der anfänglichen Synchronisierung werden alle Aufgaben, die Sie in Sales Connect erstellen, bearbeiten, abschließen oder löschen, mit Ihrer Aufgaben-Liste in Salesforce synchronisiert. Und alles, was in Salesforce erstellt, bearbeitet, abgeschlossen oder gelöscht wurde, aktualisiert Ihre Aufgaben-Liste in Sales Connect.

Um diese Synchronisierung zu aktivieren, markieren Sie einfach das Synchronisierungsfeld in Ihrer [Einstellungsseite](http://toutapp.com/next#settings/crm/salesforce/configure) in der Webanwendung.

