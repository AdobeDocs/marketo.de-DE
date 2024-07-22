---
unique-page-id: 2360291
description: Blockaktualisierungen für ein Feld - Marketo-Dokumente - Produktdokumentation
title: Aktualisieren eines Felds blockieren
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Aktualisieren eines Felds blockieren {#block-updates-to-a-field}

Durch das Blockieren von Updates in ein Feld können Sie ein einziges Mal in das Feld schreiben und dann den ursprünglichen Wert für die Lebensdauer des Felds beibehalten. Dies kann für ein Feld wie [!UICONTROL Person Source] nützlich sein.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

1. Wechseln Sie zum Bereich **[!UICONTROL Admin]** .

   ![](assets/block-updates-to-a-field-1.png)

1. Klicken Sie auf **[!UICONTROL Feldverwaltung]**.

   ![](assets/block-updates-to-a-field-2.png)

1. Suchen Sie das Feld, wählen Sie es aus und klicken Sie dann unter **[!UICONTROL Feldaktionen]** auf **[!UICONTROL Feldaktualisierungen blockieren]**.

   ![](assets/block-updates-to-a-field-3.png)

   >[!NOTE]
   >
   >Sie können auch Aktualisierungen in benutzerdefinierten Feldern für Programmmitglieder](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md) blockieren.[

1. Wählen Sie die zu blockierenden **[!UICONTROL Eingabequellen]** aus und klicken Sie auf **[!UICONTROL Anwenden]**.

   ![](assets/block-updates-to-a-field-4.png)

   >[!CAUTION]
   >
   >Bei einem Listenimport wird der Status eines Felds, das in der Importvorschau blockiert wird, nur dann angezeigt, wenn das Feld von Marketo basierend auf dem Namen des Felds, das mit _genau_ übereinstimmt, automatisch erkannt wird (oder wenn Alias erstellt wurden). Wenn das Feld manuell aus der Dropdown-Liste Marketo-Feld ausgewählt wird, wird der Blockierungsstatus nicht in der Importvorschau angezeigt, aber die Update-Blockierung für dieses Feld wird weiterhin implementiert.
