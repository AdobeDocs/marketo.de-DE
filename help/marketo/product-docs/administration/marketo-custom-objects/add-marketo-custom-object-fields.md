---
unique-page-id: 10093688
description: Hinzufügen benutzerdefinierter Marketo-Objektfelder - Marketo-Dokumente - Produktdokumentation
title: Benutzerdefinierte Marketo-Objektfelder hinzufügen
exl-id: 6d776d97-93e2-4708-9ce5-2172e02b71c3
feature: Custom Objects
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Benutzerdefinierte Marketo-Objektfelder hinzufügen {#add-marketo-custom-object-fields}

Nachdem Sie ein benutzerdefiniertes Objekt erstellt haben, müssen Sie diesem Felder hinzufügen, um Ihre Geschäftsanforderungen zu erfüllen.

Felder definieren die spezifischen Informationen, die von einem benutzerdefinierten Objekt verwendet werden. Verknüpfungsfelder haben einen speziellen Auftrag zum Verbinden benutzerdefinierter Objekte und werden in einem [ Artikel ](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md).

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/add-marketo-custom-object-fields-1.png)

1. Klicken Sie auf **[!UICONTROL Benutzerdefinierte Marketo-Objekte]**.

   ![](assets/add-marketo-custom-object-fields-2.png)

1. Wählen Sie rechts das Objekt aus, dem Sie das Feld hinzufügen möchten.

   ![](assets/add-marketo-custom-object-fields-3.png)

1. Klicken Sie auf die **[!UICONTROL Felder]** und dann auf **[!UICONTROL Neues Feld]**.

   ![](assets/add-marketo-custom-object-fields-4.png)

   >[!NOTE]
   >
   >Die drei oben gezeigten Felder werden automatisch von Marketo erstellt, wenn Sie ein benutzerdefiniertes Objekt erstellen. Marketo verwaltet diese Felder automatisch, und Sie können sie nicht bearbeiten oder löschen.

1. Geben Sie einen [!UICONTROL Anzeigenamen] und (optional) [!UICONTROL Beschreibung] ein.

   ![](assets/add-marketo-custom-object-fields-5.png)

   >[!NOTE]
   >
   >Der [!UICONTROL API-Name] kann nur bis zu seiner Genehmigung bearbeitet werden.

1. Wählen Sie nun den entsprechenden [!UICONTROL Datentyp] aus der Liste aus.

   ![](assets/add-marketo-custom-object-fields-6.png)

1. Ziehen Sie den [!UICONTROL Deduplizieren]-Schieberegler, wenn Sie das neue Feld als eindeutige Kennung verwenden möchten. Klicken Sie **[!UICONTROL Speichern]**, um den Vorgang abzuschließen.

   ![](assets/add-marketo-custom-object-fields-7.png)

   >[!TIP]
   >
   >Deduplizierungsfelder können zum Abrufen, Aktualisieren oder Löschen benutzerdefinierter Objekte verwendet werden. Jede benutzerdefinierte Objektdefinition muss mindestens ein (und nicht mehr als drei) Deduplizierungsfelder enthalten.

1. Fügen Sie alle anderen erforderlichen Felder hinzu.

   >[!NOTE]
   >
   >Wenn Sie eine Eins-zu-viele-Struktur erstellen, müssen Sie ein Verknüpfungsfeld zu Ihrem benutzerdefinierten Objekt hinzufügen. Bei einer n:n-Struktur benötigen Sie kein Verknüpfungsfeld im benutzerdefinierten Objekt, Sie müssen jedoch zwei Verknüpfungsfelder im Zwischenobjekt hinzufügen. Weitere Informationen [ Typen benutzerdefinierter Objekte finden Sie unter „Hinzufügen benutzerdefinierter Objektverknüpfungsfelder ](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md) Marketo&quot;, um die Verknüpfungsfelder zu erstellen, und [Grundlegendes zu benutzerdefinierten Objekten ](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) Marketo&quot;.

>[!MORELIKETHIS]
>
>* [Benutzerdefinierte Objektverknüpfungsfelder für Marketo hinzufügen](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Bearbeiten und Löschen eines benutzerdefinierten Marketo-Objekts](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Benutzerdefinierte Marketo-Objektfelder bearbeiten und löschen](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [Grundlegendes zu benutzerdefinierten Marketo-Objekten](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
