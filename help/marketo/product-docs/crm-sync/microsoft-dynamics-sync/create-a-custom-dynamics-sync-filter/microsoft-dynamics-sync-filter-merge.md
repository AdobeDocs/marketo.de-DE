---
unique-page-id: 10092969
description: Microsoft Dynamics-Synchronisierungsfilter - Zusammenführen - Marketo-Dokumente - Produktdokumentation
title: Microsoft Dynamics-Synchronisierungsfilter - Zusammenführen
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---

# [!DNL Microsoft] Dynamics-Synchronisationsfilter: Zusammenführen {#microsoft-dynamics-sync-filter-merge}

Beim Zusammenführen von Leads in [!DNL Microsoft Dynamics] wird der Typ Zwei Optionen verwendet: Synchronisierungsfilter = Ja (TRUE) und Synchronisierungsfilter = Nein (FALSE). Beim Zusammenführen zweier Datensätze hängt das Ergebnis davon ab, welcher Datensatz den Wert True und welcher den Wert False hat.

Die Lead-Datensätze werden basierend auf den vom Administrator definierten Workflow-Regeln wahr oder falsch, um den Gewinner zu bestimmen. Der Synchronisierungsfilter für den erfolgreichsten Datensatz bestimmt letztendlich, ob der [!DNL MS Dynamics] Datensatz mit Marketo synchronisiert wird.

Wenn eine Aufzeichnung wahr ist und die andere falsch ist, wird es schwierig.

| Wenn der Synchronisierungsfilter für den verlorenen Datensatz wie folgt lautet: | Der Synchronisierungsfilter für den erfolgreichsten Datensatz lautet: | Dies ist das Ergebnis in Marketo |
|---|---|---|
| [!UICONTROL true] | [!UICONTROL true] | Der erfolgreichste Datensatz wird weiterhin mit Marketo synchronisiert |
| [!UICONTROL false] | [!UICONTROL false] | Der erfolgreichste Datensatz wird weiterhin **nicht** mit Marketo synchronisiert |
| [!UICONTROL false] | [!UICONTROL true] | Der erfolgreichste Datensatz wird mit Marketo synchronisiert |
| [!UICONTROL true] | [!UICONTROL false] | Der erfolgreichste Datensatz wird nicht mit Marketo synchronisiert |
