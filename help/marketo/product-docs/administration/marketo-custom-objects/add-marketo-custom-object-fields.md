---
unique-page-id: 10093688
description: Benutzerdefinierte Marketo-Objektfelder hinzufügen - Marketo Docs - Produktdokumentation
title: Benutzerdefinierte Marketo-Objektfelder hinzufügen
exl-id: 6d776d97-93e2-4708-9ce5-2172e02b71c3
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Benutzerdefinierte Marketo-Objektfelder hinzufügen {#add-marketo-custom-object-fields}

Nachdem Sie ein benutzerdefiniertes Objekt erstellt haben, müssen Sie Felder hinzufügen, um Ihre geschäftlichen Anforderungen zu erfüllen.

Felder definieren die spezifischen Informationen, die von einem benutzerdefinierten Objekt verwendet werden. Verknüpfungsfelder haben einen speziellen Auftrag, um benutzerdefinierte Objekte zu verbinden. Sie werden in einer [separater Artikel](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md).

1. Klicken **Admin** und in **Datenbankverwaltung** auswählen **Benutzerdefinierte Marketo-Objekte**.

   ![](assets/image2016-1-18-9-3a2-3a6.png)

1. Wählen Sie rechts das Objekt aus, dem Sie das Feld hinzufügen möchten.

   ![](assets/image2016-1-18-9-3a5-3a3.png)

1. Im **Felder** Registerkarte, klicken Sie auf **Neues Feld**.

   ![](assets/image2015-9-15-16-3a53-3a40.png)

   >[!NOTE]
   >
   >Die drei oben gezeigten Felder werden von Marketo automatisch erstellt, wenn Sie ein benutzerdefiniertes Objekt erstellen. Marketo verwaltet diese Felder automatisch und Sie können sie weder bearbeiten noch löschen.

1. Geben Sie einen Anzeigenamen und eine Beschreibung ein.

   ![](assets/image2015-10-5-11-3a35-3a48.png)

   >[!NOTE]
   >
   >Der API-Name kann nur bearbeitet werden, bis er genehmigt wurde.

1. Wählen Sie nun einen geeigneten Datentyp aus der Liste aus.

   ![](assets/image2015-10-5-11-3a37-3a24.png)

1. Ziehen Sie den Regler Deduplizieren , wenn Sie das neue Feld als eindeutige Kennung verwenden möchten. Klicken **Speichern** zu beenden.

   ![](assets/image2015-10-5-11-3a40-3a12.png)

   >[!TIP]
   >
   >Mithilfe von Deduplizierungsfeldern können benutzerdefinierte Objekte abgerufen, aktualisiert oder gelöscht werden. Jede benutzerdefinierte Objektdefinition muss mindestens ein (und höchstens drei) dedupliziertes Feld enthalten.

1. Fügen Sie weitere erforderliche Felder hinzu.

   >[!NOTE]
   >
   >Wenn Sie eine Eins-zu-viele-Struktur erstellen, müssen Sie ein Feld Link zu Ihrem benutzerdefinierten Objekt hinzufügen. Für eine n:n-Struktur benötigen Sie im benutzerdefinierten Objekt kein Verknüpfungsfeld, sondern müssen zwei Verknüpfungsfelder in das zwischengeschaltete Objekt einfügen. Siehe [Benutzerdefinierte Marketo-Objektverknüpfungsfelder hinzufügen](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md) um die Verknüpfungsfelder zu erstellen, und [Grundlegendes zu benutzerdefinierten Marketo-Objekten](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) für weitere Informationen zu Typen von benutzerdefinierten Objekten.

>[!MORELIKETHIS]
>
>* [Benutzerdefinierte Marketo-Objektverknüpfungsfelder hinzufügen](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Bearbeiten und Löschen eines benutzerdefinierten Marketo-Objekts](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Benutzerdefinierte Marketo-Objektfelder bearbeiten und löschen](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [Grundlegendes zu benutzerdefinierten Marketo-Objekten](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

