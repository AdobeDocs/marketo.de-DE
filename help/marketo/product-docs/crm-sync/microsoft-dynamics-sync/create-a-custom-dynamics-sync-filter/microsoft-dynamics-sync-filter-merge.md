---
unique-page-id: 10092969
description: Verstehen, wie der Dynamics-Synchronisierungsfilter beim Zusammenführen von Leads funktioniert. Erfahren Sie, wie der erfolgreichste Wert des Datensatzsynchronisierungsfilters bestimmt, ob der Datensatz mit Marketo synchronisiert wird.
title: Microsoft Dynamics-Synchronisierungsfilter - Zusammenführen
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
feature: Microsoft Dynamics
TQID: 'https://experienceleague.adobe.com/wxPBvOQk4SW8gocZOGfagAMAG4OH9ghTqhh0lVRGI-U'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: d5c7388a-594e-4d15-9b39-98d6ce479e8b
    internal-label: Microsoft Dynamics
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%
---
# [!DNL Microsoft] Dynamics-Synchronisationsfilter: Zusammenführen {#microsoft-dynamics-sync-filter-merge}

Beim Zusammenführen von Leads in [!DNL Microsoft Dynamics] wird der Typ Zwei Optionen verwendet: Synchronisierungsfilter = Ja (TRUE) und Synchronisierungsfilter = Nein (FALSE). Beim Zusammenführen zweier Datensätze hängt das Ergebnis davon ab, welcher Datensatz den Wert True und welcher den Wert False hat.

Die Lead-Datensätze werden basierend auf den vom Administrator definierten Workflow-Regeln wahr oder falsch, um den Gewinner zu bestimmen. Der Synchronisierungsfilter für den erfolgreichsten Datensatz bestimmt letztendlich, ob der [!DNL MS Dynamics] Datensatz mit Marketo synchronisiert wird.

Wenn eine Aufzeichnung wahr und eine falsch ist, wird es schwierig.

| Wenn der Synchronisierungsfilter für den verlorenen Datensatz wie folgt lautet: | Der Synchronisierungsfilter für den erfolgreichsten Datensatz lautet: | Dies ist das Ergebnis in Marketo |
|---|---|---|
| [!UICONTROL true] | [!UICONTROL true] | Der erfolgreichste Datensatz wird weiterhin mit Marketo synchronisiert |
| [!UICONTROL false] | [!UICONTROL false] | Der erfolgreichste Datensatz wird weiterhin **nicht** mit Marketo synchronisiert |
| [!UICONTROL false] | [!UICONTROL true] | Der erfolgreichste Datensatz wird mit Marketo synchronisiert |
| [!UICONTROL true] | [!UICONTROL false] | Der erfolgreichste Datensatz wird nicht mit Marketo synchronisiert |
