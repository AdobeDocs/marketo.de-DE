---
unique-page-id: 10092969
description: Microsoft Dynamics-Synchronisierungsfilter - Zusammenführen - Marketo-Dokumente - Produktdokumentation
title: Microsoft Dynamics-Synchronisierungsfilter - Zusammenführen
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 4%

---

# Microsoft Dynamics Sync-Filter: Zusammenführen {#microsoft-dynamics-sync-filter-merge}

Das Zusammenführen von Leads in Microsoft Dynamics verwendet den Typ Zwei Optionen - Synchronisierungsfilter = Ja (TRUE) und Synchronisierungsfilter = Nein (FALSE). Wenn Sie zwei Datensätze zusammenführen, variiert das Ergebnis je nachdem, welcher Datensatz True und False ist.

Die Lead-Datensätze werden basierend auf den Workflow-Regeln, die vom Administrator zur Bestimmung des Gewinners definiert wurden, zu &quot;true&quot;oder &quot;false&quot;. Der Synchronisierungsfilter für den Gewinnerdatensatz bestimmt letztendlich, ob der MS Dynamics-Datensatz mit Marketo synchronisiert wird.

Wenn ein Datensatz wahr ist und ein Datensatz falsch ist, wird er schwierig.

| Wenn der Synchronisierungsfilter für den verlorenen Datensatz: | und der Synchronisierungsfilter für den Gewinnerdatensatz lautet: | Dies führt zu Marketo |
|---|---|---|
| True | True | Der erfolgreichste Rekord wird weiterhin mit Marketo synchronisiert |
| Falsch | Falsch | Der Sieger setzt sich weiter fort _not_ Synchronisierung mit Marketo |
| Falsch | True | Der erfolgreichste Datensatz wird mit Marketo synchronisiert. |
| True | Falsch | Der erfolgreichste Datensatz wird nicht mit Marketo synchronisiert. |
