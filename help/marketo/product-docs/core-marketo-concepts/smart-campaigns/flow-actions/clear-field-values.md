---
unique-page-id: 1147324
description: Feldwerte löschen - Marketo-Dokumente - Produktdokumentation
title: Feldwerte löschen
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
feature: Smart Campaigns
source-git-commit: 12f2399859c784095cc2c1df772c66c649106ba3
workflow-type: tm+mt
source-wordcount: '95'
ht-degree: 0%

---

# Feldwerte löschen {#clear-field-values}

[Datenwert ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) ist großartig. Wie kann der Wert jedoch _vollständig entfernt werden?_ Gute Frage!

1. Wählen Sie im Flussschritt das Feld aus, das Sie löschen möchten, und geben Sie **NULL** (alle Großbuchstaben) als **Neuer Wert** ein.

   ![](assets/clear-field-values-1.png)

1. Nach Abschluss des Flussschritts wird der Wert des ausgewählten Felds gelöscht.

   ![](assets/clear-field-values-2.png)

   >[!CAUTION]
   >
   >Wenn Sie den neuen Wert leer lassen oder einfach einen Leerzeichen eingeben, wird das Feld nicht wirklich leer sein. Sie müssen NULL eingeben. Beachten Sie auch, dass Flussschritte nach dem Ausführen nicht rückgängig gemacht werden können.
