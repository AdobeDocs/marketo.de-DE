---
unique-page-id: 1147074
description: Automatische Trigger-Kampagnenbereinigung - Marketo-Dokumente - Produktdokumentation
title: Automatische Auslöser-Kampagnenbereinigung
exl-id: 08012b55-e241-4524-a387-9644f5a2b17e
feature: Smart Campaigns
source-git-commit: fec5219c599c805328d77797d2636e549e489ca5
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 3%

---

# Automatische Auslöser-Kampagnenbereinigung {#automatic-trigger-campaign-cleanup}

Marketo verfügt über einen netten/kostenlosen Dienst zum Deaktivieren von ausgelösten Smart-Kampagnen, die keine Aktivität mehr erhalten. Dies beschleunigt die Gesamtleistung des Systems und spart Ihnen Zeit.

## Was passiert? {#what-happens}

Einmal im Quartal wird Marketo Smart-Kampagnen finden, die mindestens 6 Monate lang ruhten (keine Personen) und diese deaktivieren.

## Wirst du mich zuerst benachrichtigen? {#will-you-notify-me-first}

Natürlich! Einmal im Quartal erhalten Sie eine Woche im Voraus eine Benachrichtigung, die alle Kampagnen anzeigt, die wir zur Deaktivierung planen.

1. Klicken Sie auf das Symbol **[!UICONTROL Benachrichtigungen]**.

   ![](assets/automatic-trigger-campaign-cleanup-1.png)

1. Klicken Sie auf **[!UICONTROL Untätigkeit Trigger Campaign Cleanup Scheduled]**. Klicken Sie dann auf den Link **[!UICONTROL Diese inaktiven Trigger-Kampagnen werden deaktiviert]** .

   ![](assets/automatic-trigger-campaign-cleanup-2.png)

   Es wird eine Liste mit Smart-Kampagnen angezeigt, deren Deaktivierung geplant ist.

   ![](assets/automatic-trigger-campaign-cleanup-3.png)

## Welche Kampagnen werden deaktiviert? {#which-campaigns-will-be-deactivated}

Wir werden nur Trigger-Kampagnen deaktivieren, die seit über 6 Monaten aktiv sind, für die in diesem Zeitraum jedoch 0 Personen qualifiziert waren.

## Einen Augenblick! Nicht diese Kampagne! {#wait-not-this-campaign}

Keine Sorge - die Uhr einer Smart-Kampagne kann wie folgt zurückgesetzt werden:

* Eine Person, die sich für die Kampagne qualifiziert.
* Manuelles Deaktivieren und Reaktivieren der Kampagne.

Beide setzen den 6-Monats-Zähler zurück.

## Teilen Sie mir mit, welche Kampagnen deaktiviert wurden? {#will-you-let-me-know-which-campaigns-were-deactivated}

Absolut - Eine Woche nach der ursprünglichen Benachrichtigung werden wir die aufgelisteten Kampagnen deaktivieren (abzüglich aller Kampagnen, die mindestens eine Person qualifiziert oder deaktiviert/reaktiviert wurden) und eine Bestätigungsbenachrichtigung versenden.

1. Wählen Sie die Benachrichtigung **[!UICONTROL Untätigkeit Trigger - Kampagnenbereinigung geplant]** aus. Klicken Sie auf den Link **[!UICONTROL Diese inaktiven Trigger-Kampagnen]** .

   ![](assets/automatic-trigger-campaign-cleanup-4.png)

1. Daraufhin wird eine Liste der deaktivierten Kampagnen angezeigt.

   ![](assets/automatic-trigger-campaign-cleanup-5.png)
