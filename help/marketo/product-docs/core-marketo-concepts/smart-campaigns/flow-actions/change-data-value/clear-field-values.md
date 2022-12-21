---
unique-page-id: 1147324
description: Feldwerte löschen - Marketo-Dokumente - Produktdokumentation
title: Feldwerte löschen
exl-id: cddc7697-4e8f-4a62-865c-efd451abea0c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '102'
ht-degree: 0%

---

# Feldwerte löschen {#clear-field-values}

[Datenwert ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) ist toll, aber wie geht es dir? _remove_ den Wert vollständig? Gute Frage!

1. Wählen Sie im Flussschritt das Feld aus, das Sie löschen möchten, und geben Sie es ein. **NULL** (alle Großbuchstaben) als **Neuer Wert**.

   ![](assets/image2015-3-19-10-3a6-3a14.png)

1. Boom! Ich wette, du wusstest das nicht! Nach Abschluss des Flussschritts wird der Wert des ausgewählten Felds gelöscht.

   ![](assets/image2015-3-19-10-3a11-3a9.png)

   >[!CAUTION]
   >
   >Wenn Sie den neuen Wert leer lassen oder einfach einen Leerzeichen eingeben, wird das Feld nicht wirklich leer sein. Sie müssen NULL eingeben. Beachten Sie auch, dass Flussschritte nach dem Ausführen nicht rückgängig gemacht werden können.
