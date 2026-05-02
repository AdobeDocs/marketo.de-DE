---
unique-page-id: 1147324
description: Erfahren Sie, wie Sie in einem Schritt des Smart-Campaign-Flusses Feldwerte löschen. Entfernen von Werten aus Personen- oder Firmenfeldern
title: Löschen von Feldwerten
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
feature: Smart Campaigns
source-git-commit: 60c5603fa29bb1039b9d477633beb2c6f5c63486
workflow-type: tm+mt
source-wordcount: '106'
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
