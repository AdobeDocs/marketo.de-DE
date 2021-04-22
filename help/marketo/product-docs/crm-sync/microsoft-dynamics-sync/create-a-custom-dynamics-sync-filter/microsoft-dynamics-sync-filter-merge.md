---
unique-page-id: 10092969
description: Microsoft Dynamics Sync Filter - Merge - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync Filter - Zusammenführen
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 4%

---

# Microsoft Dynamics Sync-Filter: Zusammenführen {#microsoft-dynamics-sync-filter-merge}

Beim Zusammenführen von Interessenten in Microsoft Dynamics wird der Typ Zwei Optionen verwendet: Synchronisierungsfilter = Ja (TRUE) und Synchronisierungsfilter = Nein (FALSE). Wenn Sie zwei Datensätze zusammenführen, hängt das Ergebnis davon ab, welcher Datensatz &quot;True&quot;und welcher &quot;False&quot;ist.

Die Interessentendatensätze werden basierend auf den vom Administrator festgelegten Arbeitsablaufregeln zur Bestimmung des Gewinners wahr oder falsch. Der Synchronisierungsfilter für den erfolgreichsten Datensatz bestimmt letztendlich, ob der MS Dynamics Record mit Marketo synchronisiert wird.

Wenn ein Datensatz wahr ist und einer falsch, wird er knifflig.

| Wenn der Synchronisierungsfilter für den verlorenen Datensatz: | und der Synchronisierungsfilter für den Gewinn-Datensatz lautet: | Dies ist das Ergebnis in Marketo |
|---|---|---|
| Wahr | Wahr | Die erfolgreichste Aufzeichnung wird weiterhin mit Marketo synchronisiert |
| Falsch | Falsch | Der erfolgreichste Datensatz wird weiterhin mit Marketo synchronisiert.**** |
| Falsch | Wahr | Der erfolgreichste Datensatz wird mit Marketo synchronisiert |
| Wahr | Falsch | Der erfolgreichste Datensatz wird nicht mit Marketo synchronisiert |
