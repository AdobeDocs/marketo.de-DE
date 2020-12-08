---
unique-page-id: 10092969
description: Microsoft Dynamics Sync Filter - Merge - Marketing Docs - Produktdokumentation
title: Microsoft Dynamics Sync Filter - Zusammenführen
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---


# Microsoft Dynamics Sync-Filter: Zusammenführen {#microsoft-dynamics-sync-filter-merge}

Beim Zusammenführen von Interessenten in Microsoft Dynamics wird der Typ Zwei Optionen verwendet: Synchronisierungsfilter = Ja (TRUE) und Synchronisierungsfilter = Nein (FALSE). Wenn Sie zwei Datensätze zusammenführen, hängt das Ergebnis davon ab, welcher Datensatz &quot;True&quot;und welcher &quot;False&quot;ist.

Die Interessentendatensätze werden basierend auf den vom Administrator festgelegten Arbeitsablaufregeln zur Bestimmung des Gewinners wahr oder falsch. Der Synchronisierungsfilter für den erfolgreichsten Datensatz bestimmt letztendlich, ob der MS Dynamics Record mit Marketo synchronisiert wird.

Wenn ein Datensatz wahr ist und einer falsch, wird er knifflig.

| Wenn der Synchronisierungsfilter für den verlorenen Datensatz: | und der Synchronisierungsfilter für den Gewinn-Datensatz lautet: | Dies ist das Ergebnis in Marketo |
|---|---|---|
| true | true | Die erfolgreichste Platte wird weiterhin mit Marketo synchronisiert |
| False | False | Der erfolgreichste Datensatz wird weiterhin **nicht** mit Marketo synchronisiert |
| False | true | Der erfolgreichste Datensatz wird mit Marketo synchronisiert |
| true | False | Der erfolgreichste Datensatz wird nicht mit Marketo synchronisiert |

