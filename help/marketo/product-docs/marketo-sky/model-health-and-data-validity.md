---
description: Modellkonsistenz und Datenvalidität - Marketo-Dokumente - Produktdokumentation
title: Modellkonsistenz und Datenvalidierung
hide: true
hidefromtoc: true
exl-id: fdb4ae1c-a638-4aa3-aa09-1993760b8be5
source-git-commit: d229d152cbdae4f6b2e35700b85052d9c0b748d6
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---

# Modellkonsistenz und Datenvalidierung {#model-health-and-data-validity}

Die Leistung Ihrer Modelle hängt von der Qualität und Vollständigkeit der Eingabedaten ab. Sehen Sie sich den Einflussfaktor für jedes Ihrer wahrscheinlichen KI-Modelle an. Sehen Sie auch die wichtigsten Faktoren, die zu einer Registrierung für Ereignisse mit höherer/niedrigerer Ereignisanzahl, einer Teilnahme an Ereignissen oder einer Abmeldung führen.

>[!NOTE]
>
>Mit (+) markierte Verhaltensweisen beeinflussen die Prognosen positiv (und umgekehrt).

So bewerten Sie Ihre Modellgesundheit.

Navigieren Sie zum **[!UICONTROL Modelle und Datengesundheit]** Abschnitt unter **[!UICONTROL Vorhersagekräftige Zielgruppen]** im **[!UICONTROL Admin]** Gebiet von Marketo Classic. Hier sehen Sie alle Ihre Modelle und deren Status.

![Bild eins](assets/model-health-and-data-validity-1.png)

* **Trainings-Status**: Gibt an, ob Ihr Modell aktiv trainiert wird (Verbesserung der Prognosen). Das Training findet automatisch alle 2 Wochen statt. Alle Modelle, die _Verarbeitung_ kann bis zu 24 Stunden dauern. Für alle _Fehlgeschlagen_ Modelle, bitte kontaktieren [Marketo-Support](https://nation.marketo.com/t5/Support/ct-p/Support).
* **Scoring-Status**: Gibt an, ob Ihr Modell Prognosen (Wahrscheinlichkeitsprozentsätze) für Programmmitglieder aktiv berechnet.
* **Leistung**: Kategorisierung der Gesundheit Ihres Modells basierend auf der Datenvollständigkeit und Datenqualität (siehe unten).
* **Datenvollständigkeit**: Prozentsatz der vorhandenen/vollständigen Datenattribute
* **Datenqualität**: Prozentsatz der Attribute, die gute, brauchbare Daten enthalten.
