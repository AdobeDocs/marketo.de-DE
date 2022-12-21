---
unique-page-id: 1147074
description: Automatische Trigger-Kampagnenbereinigung - Marketo-Dokumente - Produktdokumentation
title: Automatische Auslöser-Kampagnenbereinigung
exl-id: 08012b55-e241-4524-a387-9644f5a2b17e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 3%

---

# Automatische Auslöser-Kampagnenbereinigung {#automatic-trigger-campaign-cleanup}

Marketo bietet einen netten/kostenlosen Dienst zum Deaktivieren von ausgelösten Smart-Kampagnen, die keine Aktivität mehr erhalten. Dies beschleunigt die Gesamtleistung des Systems und spart Ihnen Zeit.

## Was passiert? {#what-happens}

Einmal im Quartal wird Marketo intelligente Kampagnen finden, die seit mindestens sechs Monaten ruhen (keine Personen), und diese deaktivieren.

## Wirst du mich zuerst benachrichtigen? {#will-you-notify-me-first}

Natürlich! Einmal im Quartal erhalten Sie eine Woche im Voraus eine Benachrichtigung, die alle Kampagnen anzeigt, die wir zur Deaktivierung planen.

1. Navigieren Sie zu **Benachrichtigungen** Registerkarte.

   ![](assets/notifications.png)

1. Klicken **Ungenutzte Trigger-Kampagnenbereinigung geplant**. Klicken Sie anschließend auf **Diese Idle Trigger-Kampagnen werden deaktiviert** Link.

   ![](assets/image2015-4-27-20-3a48-3a35.png)

   Es wird eine Liste mit Smart-Kampagnen angezeigt, deren Deaktivierung geplant ist.

   ![](assets/image2015-4-27-20-3a35-3a29.png)

## Welche Kampagnen werden deaktiviert? {#which-campaigns-will-be-deactivated}

Wir werden nur Trigger-Kampagnen deaktivieren, die seit über 6 Monaten aktiv sind, für die in diesem Zeitraum jedoch 0 Personen qualifiziert waren.

## Einen Augenblick! Nicht diese Kampagne! {#wait-not-this-campaign}

Keine Sorge - die Uhr einer Smart-Kampagne kann wie folgt zurückgesetzt werden:

* Eine Person, die sich für die Kampagne qualifiziert.
* Manuelles Deaktivieren und Reaktivieren der Kampagne.

Beide setzen den 6-Monats-Zähler zurück.

## Teilen Sie mir mit, welche Kampagnen deaktiviert wurden? {#will-you-let-me-know-which-campaigns-were-deactivated}

Absolut - Eine Woche nach der ursprünglichen Benachrichtigung werden wir die aufgelisteten Kampagnen deaktivieren (abzüglich aller Kampagnen, die mindestens eine Person qualifiziert oder deaktiviert/reaktiviert wurden) und eine Bestätigungsbenachrichtigung versenden.

1. Wählen Sie die **Ungenutzte Trigger-Kampagnenbereinigung geplant** Benachrichtigung. Klicken Sie auf **Diese inaktiven Trigger-Kampagnen** Link.

   ![](assets/image2015-4-27-20-3a56-3a41.png)

1. Daraufhin wird eine Liste der deaktivierten Kampagnen angezeigt.

   ![](assets/image2015-4-27-20-3a58-3a38.png)
