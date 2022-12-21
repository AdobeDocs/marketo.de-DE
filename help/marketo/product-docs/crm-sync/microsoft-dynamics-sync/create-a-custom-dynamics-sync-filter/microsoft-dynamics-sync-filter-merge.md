---
unique-page-id: 10092969
description: Microsoft Dynamics-Synchronisierungsfilter - Zusammenführen - Marketo-Dokumente - Produktdokumentation
title: Microsoft Dynamics-Synchronisierungsfilter - Zusammenführen
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 4%

---

# Microsoft Dynamics Sync-Filter: Zusammenführen {#microsoft-dynamics-sync-filter-merge}

Das Zusammenführen von Leads in Microsoft Dynamics verwendet den Typ Zwei Optionen - Synchronisierungsfilter = Ja (TRUE) und Synchronisierungsfilter = Nein (FALSE). Wenn Sie zwei Datensätze zusammenführen, variiert das Ergebnis je nachdem, welcher Datensatz True und False ist.

Die Lead-Datensätze werden basierend auf den Workflow-Regeln, die vom Administrator zur Bestimmung des Gewinners definiert wurden, zu &quot;true&quot;oder &quot;false&quot;. Der Synchronisierungsfilter für den erfolgreichsten Datensatz bestimmt letztendlich, ob der MS Dynamics-Datensatz mit Marketo synchronisiert wird.

Wenn ein Datensatz wahr ist und einer falsch ist, wird er schwierig.

| Wenn der Synchronisierungsfilter für den verlorenen Datensatz: | und der Synchronisierungsfilter für den Gewinnerdatensatz lautet: | Dies führt zu Marketo |
|---|---|---|
| True | True | Der erfolgreichste Rekord wird weiterhin mit Marketo synchronisiert |
| False | False | Der Sieger setzt sich weiter fort **not** Synchronisierung mit Marketo |
| False | True | Der erfolgreichste Datensatz wird mit Marketo synchronisiert. |
| True | False | Der erfolgreichste Datensatz wird nicht mit Marketo synchronisiert |
