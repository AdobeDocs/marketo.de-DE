---
unique-page-id: 2360291
description: Blockieren von Aktualisierungen für ein Feld - Marketing-Dokumente - Produktdokumentation
title: Blockieren von Aktualisierungen für ein Feld
translation-type: tm+mt
source-git-commit: 9f88e7cebc5e9d0d4491d65d332ccfdd9a31c395
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---


# Blockieren von Aktualisierungen für ein Feld {#block-updates-to-a-field}

Durch das Blockieren von Updates für ein Feld können Sie einmalig in das Feld schreiben und dann den ursprünglichen Wert für die gesamte Feldlebensdauer beibehalten. Dies kann für ein Feld wie &quot;Personenquelle&quot;nützlich sein.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

1. Wechseln Sie zu **Admin** und klicken Sie auf **Feldverwaltung**.

   ![](assets/image2014-9-24-13-3a54-3a40.png)

1. Suchen Sie das Feld, wählen Sie es aus und klicken Sie dann unter **Feldaktionen** auf **Feldaktualisierungen blockieren**.

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >Sie können auch Updates für die benutzerdefinierten Felder [Programm-Mitglied](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md) blockieren.

1. Wählen Sie die zu blockierenden **Eingabequellen** aus und klicken Sie auf **Anwenden**.

   ![](assets/image2014-9-24-13-3a55-3a16.png)

   >[!CAUTION]
   >
   >Beim Importieren einer Liste wird der Feldstatus, der in der Vorschau &quot;Importieren&quot;blockiert wird, nur dann angezeigt, wenn das Feld automatisch von Marketo anhand des Feldnamens erkannt wird, der _genau_ entspricht (oder wenn Aliase eingerichtet sind). Wenn das Feld manuell aus der Dropdownliste &quot;Feld markieren&quot;ausgewählt wird, wird der Blockierungsstatus nicht in der Vorschau &quot;Importieren&quot;angezeigt, aber die Updateblockung für dieses Feld wird trotzdem implementiert.
