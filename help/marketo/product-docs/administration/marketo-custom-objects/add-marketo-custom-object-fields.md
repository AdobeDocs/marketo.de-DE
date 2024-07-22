---
unique-page-id: 10093688
description: Benutzerdefinierte Marketo-Objektfelder hinzufügen - Marketo Docs - Produktdokumentation
title: Benutzerdefinierte Marketo-Objektfelder hinzufügen
exl-id: 6d776d97-93e2-4708-9ce5-2172e02b71c3
feature: Custom Objects
source-git-commit: 99c38fd24631e94a9554bf09de11e8eb607150d6
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Benutzerdefinierte Marketo-Objektfelder hinzufügen {#add-marketo-custom-object-fields}

Nachdem Sie ein benutzerdefiniertes Objekt erstellt haben, müssen Sie Felder hinzufügen, um Ihre geschäftlichen Anforderungen zu erfüllen.

Felder definieren die spezifischen Informationen, die von einem benutzerdefinierten Objekt verwendet werden. Verknüpfungsfelder haben einen speziellen Auftrag, benutzerdefinierte Objekte zu verbinden, und werden in einem [separaten Artikel](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md) behandelt.

1. Wechseln Sie zum Bereich **[!UICONTROL Admin]** .

   ![](assets/add-marketo-custom-object-fields-1.png)

1. Klicken Sie auf **[!UICONTROL Marketo Custom Objects]**.

   ![](assets/add-marketo-custom-object-fields-2.png)

1. Wählen Sie rechts das Objekt aus, dem Sie das Feld hinzufügen möchten.

   ![](assets/add-marketo-custom-object-fields-3.png)

1. Klicken Sie auf die Registerkarte **[!UICONTROL Felder]** und dann auf **[!UICONTROL Neues Feld]**.

   ![](assets/add-marketo-custom-object-fields-4.png)

   >[!NOTE]
   >
   >Die drei oben gezeigten Felder werden von Marketo automatisch erstellt, wenn Sie ein benutzerdefiniertes Objekt erstellen. Marketo verwaltet diese Felder automatisch und Sie können sie weder bearbeiten noch löschen.

1. Geben Sie einen [!UICONTROL Anzeigenamen] und (optional) [!UICONTROL Beschreibung] ein.

   ![](assets/add-marketo-custom-object-fields-5.png)

   >[!NOTE]
   >
   >Der API-Name kann nur bearbeitet werden, bis er genehmigt wurde.

1. Wählen Sie nun einen entsprechenden [!UICONTROL Datentyp] aus der Liste aus.

   ![](assets/add-marketo-custom-object-fields-6.png)

1. Ziehen Sie den Schieberegler [!UICONTROL Deduplizierung] nach oben, wenn Sie das neue Feld als eindeutige Kennung verwenden möchten. Klicken Sie auf **[!UICONTROL Speichern]** , um den Vorgang abzuschließen.

   ![](assets/add-marketo-custom-object-fields-7.png)

   >[!TIP]
   >
   >Mithilfe von Deduplizierungsfeldern können benutzerdefinierte Objekte abgerufen, aktualisiert oder gelöscht werden. Jede benutzerdefinierte Objektdefinition muss mindestens ein (und höchstens drei) dedupliziertes Feld enthalten.

1. Fügen Sie weitere erforderliche Felder hinzu.

   >[!NOTE]
   >
   >Wenn Sie eine Eins-zu-viele-Struktur erstellen, müssen Sie ein Feld Link zu Ihrem benutzerdefinierten Objekt hinzufügen. Für eine n:n-Struktur benötigen Sie im benutzerdefinierten Objekt kein Verknüpfungsfeld, sondern müssen zwei Verknüpfungsfelder in das zwischengeschaltete Objekt einfügen. Weitere Informationen zu den Typen von benutzerdefinierten Objekten finden Sie unter [Marketo-Felder für benutzerdefinierte Objektverknüpfungen hinzufügen](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md) , um die Verknüpfungsfelder zu erstellen, und unter [Grundlagen zu benutzerdefinierten Objekten in Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) .

>[!MORELIKETHIS]
>
>* [Benutzerdefinierte Marketo-Objektverknüpfungsfelder hinzufügen](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Bearbeiten und Löschen eines benutzerdefinierten Marketo-Objekts](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Benutzerdefinierte Marketo-Objektfelder bearbeiten und löschen](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [Grundlegendes zu benutzerdefinierten Marketo-Objekten](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
