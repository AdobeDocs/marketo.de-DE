---
unique-page-id: 10093688
description: hinzufügen Marketo Benutzerdefinierte Objektfelder - Marketo Docs - Produktdokumentation
title: Benutzerdefinierte Objektfelder Hinzufügen Marketo
translation-type: tm+mt
source-git-commit: 65182770291dc14fbe915a40403fc09b433aae86
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---


# Benutzerdefinierte Objektfelder Hinzufügen Marketo {#add-marketo-custom-object-fields}

Nachdem Sie ein benutzerdefiniertes Objekt erstellt haben, müssen Sie Felder hinzufügen, um Ihren geschäftlichen Anforderungen zu entsprechen.

Felder definieren die spezifischen Informationen, die von einem benutzerdefinierten Objekt verwendet werden. Verknüpfungsfelder haben einen speziellen Auftrag, um benutzerdefinierte Objekte zu verbinden, und werden in einem [separaten Artikel](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md) behandelt.

1. Klicken Sie auf **Admin** und wählen Sie unter **Datenbankverwaltung** **Marketo Benutzerspezifische Objekte**.

   ![](assets/image2016-1-18-9-3a2-3a6.png)

1. Wählen Sie das Objekt aus, dem Sie das Feld auf der rechten Seite hinzufügen möchten.

   ![](assets/image2016-1-18-9-3a5-3a3.png)

1. Klicken Sie auf der Registerkarte **Felder** auf **Neues Feld**.

   ![](assets/image2015-9-15-16-3a53-3a40.png)

   >[!NOTE]
   >
   >Die drei oben aufgeführten Felder werden automatisch von Marketo erstellt, wenn Sie ein benutzerdefiniertes Objekt erstellen. Marketo verwaltet diese Felder automatisch und Sie können sie weder bearbeiten noch löschen.

1. Geben Sie einen Anzeigenamen und eine Beschreibung ein.

   ![](assets/image2015-10-5-11-3a35-3a48.png)

   >[!NOTE]
   >
   >Der API-Name kann nur bearbeitet werden, bis er genehmigt wurde.

1. Wählen Sie jetzt einen entsprechenden Datentyp aus der Liste.

   ![](assets/image2015-10-5-11-3a37-3a24.png)

1. Ziehen Sie den Deduplizierungsregler nach oben, wenn Sie das neue Feld als eindeutigen Bezeichner verwenden möchten. Klicken Sie auf **Speichern**, um abzuschließen.

   ![](assets/image2015-10-5-11-3a40-3a12.png)

   >[!TIP]
   >
   >Deduplizierungsfelder können zum Abrufen, Aktualisieren oder Löschen benutzerdefinierter Objekte verwendet werden. Jede benutzerdefinierte Objektdefinition muss mindestens ein (und nicht mehr als drei) dedupliziertes Feld enthalten.

1. hinzufügen anderen erforderlichen Felder.

   >[!NOTE]
   >
   >Wenn Sie eine Eins-zu-viele-Struktur erstellen, müssen Sie dem benutzerdefinierten Objekt ein Feld &quot;Link&quot;hinzufügen. Für eine Viele-zu-viele-Struktur benötigen Sie im benutzerdefinierten Objekt kein Verknüpfungsfeld, Sie müssen jedoch zwei Verknüpfungsfelder in das intermediäre Objekt einfügen. Weitere Informationen zu Typen von benutzerdefinierten Objekten finden Sie unter [Hinzufügen Felder für benutzerdefinierte Objektverknüpfungen von Marketo ](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md), um die Verknüpfungsfelder zu erstellen, und [Benutzerdefinierte Marketo-Objekte](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md).

>[!MORELIKETHIS]
>
>* [Benutzerdefinierte Objektverknüpfungsfelder Hinzufügen Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Bearbeiten und Löschen eines benutzerdefinierten Marketo-Objekts](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Benutzerdefinierte Marketo-Objektfelder bearbeiten und löschen](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [Benutzerdefinierte Marketo-Objekte](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

