---
unique-page-id: 2360291
description: Blockieren von Aktualisierungen eines Felds - Marketo-Dokumente - Produktdokumentation
title: Blockieren von Aktualisierungen eines Felds
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Blockieren von Aktualisierungen eines Felds {#block-updates-to-a-field}

Wenn Sie Aktualisierungen an einem Feld blockieren, können Sie nur einmal in das Feld schreiben und dann den ursprünglichen Wert während der Lebensdauer des Felds beibehalten. Source Dies kann für ein Feld wie „Person [!UICONTROL &quot; nützlich ].

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/block-updates-to-a-field-1.png)

1. Klicken Sie **[!UICONTROL Feldverwaltung]**.

   ![](assets/block-updates-to-a-field-2.png)

1. Suchen Sie das Feld, wählen Sie es aus und klicken Sie dann unter **[!UICONTROL Feldaktionen]** auf **[!UICONTROL Feldaktualisierungen blockieren]**.

   ![](assets/block-updates-to-a-field-3.png)

   >[!NOTE]
   >
   >Sie können auch Aktualisierungen von [Benutzerdefinierte Felder für Programmteilnehmer](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md) blockieren.

1. Wählen Sie die **[!UICONTROL Eingabequellen]** die Sie blockieren möchten, und klicken Sie auf **[!UICONTROL Anwenden]**.

   ![](assets/block-updates-to-a-field-4.png)

   >[!CAUTION]
   >
   >Beim Import einer Liste wird der Status eines Felds, das in der Importvorschau blockiert wird, nur angezeigt, wenn das Feld automatisch von Marketo anhand des Namens des Felds erkannt wird, das _exakt_ entspricht (oder wenn Aliase erstellt wurden). Wenn das Feld manuell aus der Dropdown-Liste Marketo-Feld ausgewählt wird, wird der Status Blockiert in der Importvorschau nicht angezeigt, aber die Update-Blockierung für dieses Feld wird weiterhin implementiert.
