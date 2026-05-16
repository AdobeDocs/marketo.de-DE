---
unique-page-id: 2360291
description: Blockaktualisierungen an ein Feld, sodass der erste geschriebene Wert für die Lebensdauer des Datensatzes beibehalten wird.
title: Blockieren von Aktualisierungen eines Felds
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
feature: Field Management
TQID: https://experienceleague.adobe.com/XHwNOU3s7CWDUp21LaxOTo--NA1nYZvCL7G4y5AjUFg
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: e64968b2-4ee5-47f9-8cae-0588f184b9eb
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 182
ht-degree: 7%

---

# Blockieren von Aktualisierungen eines Felds {#block-updates-to-a-field}

Wenn Sie Aktualisierungen an einem Feld blockieren, können Sie nur einmal in das Feld schreiben und dann den ursprünglichen Wert während der Lebensdauer des Datensatzes beibehalten. Dies kann für ein Feld wie „Person [!UICONTROL &quot; nützlich ].

>[!NOTE]
>
>**Admin-Berechtigungen erforderlich**

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
