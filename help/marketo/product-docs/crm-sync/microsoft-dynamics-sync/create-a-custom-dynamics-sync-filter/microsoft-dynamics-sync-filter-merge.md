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

# Microsoft Dynamics-Synchronisierungsfilter: Zusammenführen {#microsoft-dynamics-sync-filter-merge}

Beim Zusammenführen von Leads in Microsoft Dynamics wird der Typ Zwei Optionen verwendet: Synchronisierungsfilter = Ja (TRUE) und Synchronisierungsfilter = Nein (FALSE). Beim Zusammenführen zweier Datensätze hängt das Ergebnis davon ab, welcher Datensatz den Wert True und welcher den Wert False hat.

Die Lead-Datensätze werden basierend auf den vom Administrator definierten Workflow-Regeln wahr oder falsch, um den Gewinner zu bestimmen. Der Synchronisierungsfilter für den erfolgreichsten Datensatz bestimmt letztendlich, ob der MS Dynamics-Datensatz mit Marketo synchronisiert wird.

Wenn eine Aufzeichnung wahr ist und die andere falsch ist, wird es schwierig.

| Wenn der Synchronisierungsfilter für den verlorenen Datensatz wie folgt lautet: | Der Synchronisierungsfilter für den erfolgreichsten Datensatz lautet: | Dies ist das Ergebnis in Marketo |
|---|---|---|
| True | True | Der erfolgreichste Datensatz wird weiterhin mit Marketo synchronisiert |
| Falsch | Falsch | Der erfolgreichste Datensatz wird weiterhin _nicht_ mit Marketo synchronisiert |
| Falsch | True | Der erfolgreichste Datensatz wird mit Marketo synchronisiert |
| True | Falsch | Der erfolgreichste Datensatz wird nicht mit Marketo synchronisiert |
