---
unique-page-id: 1147324
description: Erfahren Sie, wie Sie in einem Schritt des Smart-Campaign-Flusses Feldwerte löschen. Entfernen von Werten aus Personen- oder Firmenfeldern
title: Löschen von Feldwerten
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/57QZb7T-y2JVdNeP4nhTl9PDjIX1S9GcQmRAMJ-53E0
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 106
ht-degree: 5%

---

# Löschen von Feldwerten {#clear-field-values}

[Datenwert ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) ist großartig, aber wie _der Wert vollständig_? Gute Frage!

1. Wählen Sie im Flussschritt das Feld aus, das Sie löschen möchten, und geben Sie **[!UICONTROL NULL]** (alle Begrenzungen) als &quot;**[!UICONTROL Wert“]**.

   ![](assets/clear-field-values-1.png)

1. Nach Abschluss des Flussschritts wird der Wert des ausgewählten Felds gelöscht.

   ![](assets/clear-field-values-2.png)

   >[!CAUTION]
   >
   >Wenn Sie den neuen Wert leer lassen oder ein Leerzeichen eingeben, wird das Feld nicht wirklich leer. Sie müssen NULL eingeben. Beachten Sie außerdem, dass Flussschritte nach der Ausführung nicht mehr rückgängig gemacht werden können.
