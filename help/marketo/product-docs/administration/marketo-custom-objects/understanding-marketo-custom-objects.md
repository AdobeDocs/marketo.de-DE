---
unique-page-id: 10093188
description: Grundlegendes zu benutzerdefinierten Marketo-Objekten - Marketo-Dokumente - Produktdokumentation
title: Grundlegendes zu benutzerdefinierten Marketo-Objekten
exl-id: f18b1689-c7bc-4da0-8326-7b29733d527d
feature: Custom Objects
source-git-commit: 7fd4d4e12b348ad4d0d69cd3f62cf441eda258b8
workflow-type: tm+mt
source-wordcount: '699'
ht-degree: 0%

---

# Grundlegendes zu benutzerdefinierten Marketo-Objekten {#understanding-marketo-custom-objects}

Verwenden Sie benutzerdefinierte Objekte, um für Ihr Unternehmen spezifische Metriken zu verfolgen.

>[!AVAILABILITY]
>
>Nicht alle Marketo Engage-Benutzer haben diese Funktion erworben. Weitere Informationen erhalten Sie beim Adobe Account Team (Ihrem Account Manager).

Verwenden Sie benutzerdefinierte Objekte als Filter und Trigger in Ihren Smart-Kampagnen. Beispiel:

* **Filter**: Senden von E-Mails nur an Inhaber einer bestimmten Fahrzeugmarke
* **Trigger**: Senden Sie eine E-Mail, wenn ein benutzerdefiniertes Objekt einer Person oder einem Unternehmen hinzugefügt wird.

Sie können benutzerdefinierte Objekte in einer Eins-zu-viele- oder einer Viele-zu-viele-Beziehung einrichten. Beispiel:

* **Eins-zu-viele**: Eine Person besitzt mehrere Autos
* **Viele-zu-viele**: Mehrere Studierende werden in mehreren Kursen aus einem Kurskatalog registriert

Eine Eins-zu-viele-Struktur verwendet ein einzelnes Verknüpfungsfeld, um das benutzerdefinierte Objekt mit einer Person oder einem Unternehmen zu verbinden.

Viele-zu-viele benutzerdefinierte Objekte verwenden zwei Verknüpfungsfelder, die Teil eines Zwischenobjekts sind. Ein Verknüpfungsfeld ist mit der Person oder dem Unternehmen verbunden und ein anderes mit dem benutzerdefinierten Objekt, z. B. dem Kurskatalog. Dieses Zwischenobjekt kann zusätzliche benutzerdefinierte Felder enthalten, z. B. eine Kursnote oder ein Anwesenheitsdatum, die die Art der Verbindung weiter definieren.

>[!TIP]
>
>Importieren Sie benutzerdefinierte Objekte mithilfe von kommagetrennten Werten (CSV) in der Benutzeroberfläche, um ein Datenbeispiel zu testen und zu validieren. Laden Sie dann alle Ihre Dateien mit einer API hoch.

>[!CAUTION]
>
>Sie können benutzerdefinierte Objekte nicht wiederherstellen. Stellen Sie daher sicher, dass Sie sie nicht mehr benötigen, bevor Sie sie löschen.

## Zugreifen auf benutzerdefinierte Marketo-Objekte {#accessing-marketo-custom-objects}

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/understanding-marketo-custom-objects-1.png)

1. Klicken Sie auf **[!UICONTROL Benutzerdefinierte Marketo-Objekte]**.

   ![](assets/understanding-marketo-custom-objects-2.png)

1. Die Anzeige Benutzerdefinierte Marketo-Objekte listet alle Ihre benutzerdefinierten Objekte auf der rechten Seite auf, aber nur die genehmigten im Hauptraster.

   ![](assets/understanding-marketo-custom-objects-3.png)

   >[!NOTE]
   >
   >Das Raster zeigt den Objektnamen, die Anzahl der Datensätze, die Anzahl der Felder und das Datum der letzten Aktualisierung an.

   >[!TIP]
   >
   >Marketo aktualisiert diese Felder automatisch. Sie können die Anzeige jedoch aktualisieren, indem Sie auf das Symbol in der Spalte Datensätze klicken.

1. Klicken Sie auf den Objektnamen rechts, um die Detailseite zu öffnen.

   ![](assets/understanding-marketo-custom-objects-4.png)

## Benutzerdefinierte Objekte anzeigen, die mit einer Person verknüpft sind {#view-custom-objects-associated-to-a-person}

Nachdem Sie die benutzerdefinierte Objektstruktur erstellt haben, werden die benutzerdefinierten Objekte beim Hochladen der spezifischen benutzerdefinierten Objektdaten automatisch mit Personen in der Datenbank verknüpft, indem das Verknüpfungsfeld im benutzerdefinierten Objekt verwendet wird. Sie können Informationen auf der Registerkarte [!UICONTROL Benutzerdefinierte Objekte] auf der Seite mit den Personendetails anzeigen.

1. Wechseln Sie zu **[!UICONTROL Datenbank]**.

   ![](assets/understanding-marketo-custom-objects-5.png)

1. Öffnen Sie Ihre Datenbank und klicken Sie auf die Registerkarte **[!UICONTROL Personen]** . Doppelklicken Sie auf den Datensatz für eine Person, die Sie mit einem benutzerdefinierten Objekt verknüpft haben.

   ![](assets/understanding-marketo-custom-objects-6.png)

1. Klicken Sie auf der Seite mit den Personendetails auf die Registerkarte **[!UICONTROL Benutzerdefinierte Objekte]** . Wählen Sie das Objekt aus der Dropdown-Liste aus.

   ![](assets/understanding-marketo-custom-objects-7.png)

1. Jetzt können Sie eine Liste aller benutzerdefinierten Objekte dieses Typs anzeigen, die mit dieser Person verknüpft sind.

   ![](assets/understanding-marketo-custom-objects-8.png)

   >[!NOTE]
   >
   >In einem Personendatensatz können auf der Registerkarte Benutzerdefiniertes Objekt maximal 100 Datensätze angezeigt werden, sortiert nach ID in absteigender Reihenfolge.

## Verwenden benutzerdefinierter Objekte mit Firmen {#using-custom-objects-with-companies}

Ein benutzerdefiniertes Objekt, das mit dem Unternehmen verknüpft ist, funktioniert am besten, wenn Sie Unternehmen aus dem CRM synchronisieren oder wenn Sie Unternehmen explizit mithilfe der API erstellen. Es wird außerdem empfohlen, die Unternehmens-ID als Verknüpfungsfeld zu verwenden.

Wenn Sie mehrere Personen in Marketo haben, bei denen es sich um Datensätze im CRM oder um reine Marketo-Datensätze handelt, wird ein benutzerdefiniertes Objekt, das mit einer Firma verknüpft ist, nicht mit mehr als einem einzelnen Datensatz verknüpft. Dies liegt daran, dass ein Unternehmen mit mehreren Personen darunter nur unterstützt wird, wenn Unternehmen aus dem CRM synchronisiert werden oder wenn Sie eine API verwenden, um explizit Unternehmen zu erstellen.

Benutzerdefinierte Objekte können nur direkt mit einem einzelnen Datensatz verknüpft werden. Wenn Ihr benutzerdefinierter Objekttyp also nach Unternehmensfeld verknüpft ist, sollten Sie sicherstellen, dass Ihre Personendatensätze entweder über eine Kontaktkonvertierung im CRM-System oder mithilfe des Felds externalCompanyId mit einem Unternehmen verknüpft sind, wenn Sie Unternehmen mithilfe der REST-APIs von Marketo verwalten. Bei Personendatensätzen, die nicht explizit mit Firmendatensätzen verknüpft sind, werden benutzerdefinierte Objekte, die über „Firma“ verknüpft sind, nach dem Zufallsprinzip mit einem einzelnen Datensatz verknüpft, auch wenn der Wert des Firmenfelds für viele Personen freigegeben ist.

Weitere [ finden Sie unter ](/help/marketo/product-docs/administration/marketo-custom-objects/import-custom-object-data.md) von benutzerdefinierten Objektdaten importieren .

>[!MORELIKETHIS]
>
>* [Erstellen von benutzerdefinierten Marketo-Objekten](/help/marketo/product-docs/administration/marketo-custom-objects/create-marketo-custom-objects.md)
>* [Benutzerdefiniertes Objekt genehmigen](/help/marketo/product-docs/administration/marketo-custom-objects/approve-a-custom-object.md)
>* [Bearbeiten und Löschen eines benutzerdefinierten Marketo-Objekts](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Benutzerdefinierte Marketo-Objektfelder hinzufügen](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Benutzerdefinierte Marketo-Objektfelder bearbeiten und löschen](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [Benutzerdefinierte Objektdaten importieren](/help/marketo/product-docs/administration/marketo-custom-objects/import-custom-object-data.md)
