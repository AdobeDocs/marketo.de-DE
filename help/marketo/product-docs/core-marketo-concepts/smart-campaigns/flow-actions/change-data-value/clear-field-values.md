---
unique-page-id: 1147324
description: Feldwerte löschen - MarketingToDocs - Produktdokumentation
title: Feldwerte löschen
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '121'
ht-degree: 0%

---


# Feldwerte löschen {#clear-field-values}

** Datenwert [](../../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)ändern** ist großartig, aber wie *entfernen* Sie den Wert vollständig? Gute Frage!

1. Wählen Sie im Flussschritt das Feld, das Sie löschen möchten, und geben Sie **NULL **(Großbuchstaben) als **Neuer Wert** ein.

   ![](assets/image2015-3-19-10-3a6-3a14.png)

1. Boom! Ich wette, du wusstest das nicht! Nach Abschluss des Flussschritts wird der Wert des ausgewählten Felds gelöscht.

   ![](assets/image2015-3-19-10-3a11-3a9.png)

   >[!CAUTION]
   >
   >Wenn Sie den neuen Wert leer lassen oder einfach einen Leerzeichen eingeben, wird das Feld nicht wirklich leer. Sie müssen NULL eingeben. Beachten Sie auch, dass Flussschritte nach dem Ausführen nicht rückgängig gemacht werden können.

   ![(Lächeln)](assets/smile.svg)

Übrigens befindet sich diese kleine Technik in der Zertifizierungsprüfung von Marketo. Sag ihnen nicht, dass wir das gesagt haben!