---
unique-page-id: 2360291
description: Blockaktualisierungen für ein Feld - Marketo-Dokumente - Produktdokumentation
title: Aktualisieren eines Felds blockieren
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 2%

---

# Aktualisieren eines Felds blockieren {#block-updates-to-a-field}

Durch das Blockieren von Updates in ein Feld können Sie ein einziges Mal in das Feld schreiben und dann den ursprünglichen Wert für die Lebensdauer des Felds beibehalten. Dies kann für ein Feld wie Personenquelle nützlich sein.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

1. Navigieren Sie zum **Admin**-Bereich.

   ![](assets/block-updates-to-a-field-1.png)

1. Klicken **Feldverwaltung**.

   ![](assets/block-updates-to-a-field-2.png)

1. Suchen Sie das Feld, wählen Sie es aus und klicken Sie dann unter **Feldaktionen** klicken **Blockfeldaktualisierungen**.

   ![](assets/block-updates-to-a-field-3.png)

   >[!NOTE]
   >
   >Sie können Aktualisierungen in [Benutzerdefinierte Felder für Programmmitglieder](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md) sowie

1. Wählen Sie die **Input Sources** Markieren Sie den gewünschten Block und klicken Sie auf **Anwenden**.

   ![](assets/block-updates-to-a-field-4.png)

   >[!CAUTION]
   >
   >Bei einem Listenimport wird der Status eines Felds, das in der Importvorschau blockiert wird, nur dann angezeigt, wenn das Feld von Marketo basierend auf dem Feldnamen, der mit der _just_ (oder falls Alias festgestellt wurden). Wenn das Feld manuell aus der Dropdown-Liste Marketo-Feld ausgewählt wird, wird der Blockierungsstatus nicht in der Importvorschau angezeigt, aber die Update-Blockierung für dieses Feld wird weiterhin implementiert.
