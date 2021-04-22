---
unique-page-id: 10093188
description: Benutzerdefinierte Marketo-Objekte - Marketo Docs - Produktdokumentation
title: Benutzerdefinierte Marketo-Objekte
exl-id: f18b1689-c7bc-4da0-8326-7b29733d527d
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 2%

---

# Benutzerdefinierte Marketo-Objekte {#understanding-marketo-custom-objects}

Verwenden Sie benutzerdefinierte Objekte, um unternehmensspezifische Metriken zu verfolgen.

>[!AVAILABILITY]
>
>Nicht alle Kunden haben diese Funktion erworben. Detaillierte Informationen erhalten Sie vom zuständigen Vertriebsmitarbeiter.

Verwenden Sie benutzerdefinierte Objekte als Filter und Trigger in Ihren intelligenten Kampagnen. Zum Beispiel:

* **Filter**: E-Mails nur an Inhaber einer bestimmten Fahrzeugmarke senden
* **Trigger**: Senden Sie eine E-Mail, wenn einer Person oder Firma ein benutzerdefiniertes Objekt hinzugefügt wird.

Sie können benutzerdefinierte Objekte in einer Eins-zu-viele- oder einer Viele-zu-viele-Beziehung einrichten. Zum Beispiel:

* **Eins-zu-viele**: Eine Person besitzt mehrere Autos
* **Viele-zu-viele**: Mehrere Schüler/innen sind in mehreren Kursen aus einem Kurskatalog eingeschrieben

Eine Eins-zu-viele-Struktur verwendet ein einzelnes Verknüpfungsfeld, um das benutzerdefinierte Objekt mit einer Person oder einer Firma zu verbinden.

Viele zu viele benutzerdefinierte Objekte verwenden zwei Verknüpfungsfelder, die Teil eines Zwischenobjekts sind. Ein Feld &quot;Link&quot;ist mit der Person oder Firma verbunden und ein anderes mit dem benutzerdefinierten Objekt, z. B. dem Kurskatalog. Dieses intermediäre Objekt kann zusätzliche benutzerdefinierte Felder enthalten, z. B. eine Kursstufe oder ein Anwesenheitsdatum, die die Art der Verbindung weiter definieren.

>[!TIP]
>
>Importieren Sie benutzerdefinierte Objekte mit kommagetrennten Werten (CSV) in der Benutzeroberfläche, um ein Datenmuster zu testen und zu validieren. Laden Sie dann alle Dateien mit einer API hoch.

>[!CAUTION]
>
>Sie können benutzerdefinierte Objekte nicht wiederherstellen. Daher müssen Sie sie vor dem Löschen nicht mehr benötigen.

## Zugriff auf benutzerdefinierte Marketo-Objekte {#accessing-marketo-custom-objects}

1. Um benutzerdefinierte Marketo-Objekte zu erstellen oder zu bearbeiten, klicken Sie auf **Admin** und dann auf den Link **Marketo Benutzerdefinierte Objekte**.

   ![](assets/image2016-5-18-16-3a59-3a30.png)

1. Die benutzerdefinierten Marketo-Objekte zeigen Listen für alle benutzerdefinierten Objekte auf der rechten Seite an, jedoch nur für die genehmigten Objekte im Hauptraster.

   ![](assets/image2016-6-10-15-3a14-3a18.png)

1. Das Raster zeigt den Objektnamen, die Anzahl der Datensätze, die Anzahl der Felder und das Datum der letzten Aktualisierung an.

   >[!TIP]
   >
   >Marketo aktualisiert diese Felder automatisch, aber Sie können die Anzeige aktualisieren, indem Sie auf das Symbol in der Spalte &quot;Datensätze&quot;klicken.

1. Klicken Sie auf den Objektnamen auf der rechten Seite, um die Detailseite zu öffnen.

   ![](assets/image2016-6-10-15-3a15-3a29.png)

## Benutzerdefinierte Objekte der Ansicht, die einer Person {#view-custom-objects-associated-to-a-person} zugeordnet sind

Nachdem Sie die benutzerdefinierte Objektstruktur erstellt haben, werden die benutzerdefinierten Objekte beim Hochladen der spezifischen Objektdaten mithilfe des Linkfelds im benutzerdefinierten Objekt automatisch mit den Personen in der Datenbank verknüpft. Informationen zur Ansicht können Sie auf der Seite mit den Personendetails auf der Registerkarte &quot;Benutzerspezifische Objekte&quot;finden.

1. Gehen Sie zu **Datenbank**.

   ![](assets/db.png)

1. Öffnen Sie die Datenbank und klicken Sie auf die Registerkarte **Personen**. Klicken Sie bei gedrückter Dublette auf den Datensatz für eine Person, die Sie einem benutzerdefinierten Objekt zugeordnet haben.

   ![](assets/five.png)

1. Klicken Sie auf der Seite mit den Personendetails auf die Registerkarte **Benutzerspezifische Objekte**. Wählen Sie das Objekt aus der Dropdownliste aus.

   ![](assets/six.png)

1. Jetzt können Sie eine Liste aller benutzerspezifischen Objekte dieses Typs, die mit dieser Person verbunden sind, Ansicht vornehmen.

   ![](assets/seven.png)

## Verwenden benutzerdefinierter Objekte mit Firmen {#using-custom-objects-with-companies}

Ein benutzerdefiniertes Objekt, das mit der Firma verknüpft ist, funktioniert am besten, wenn Sie Firmen aus dem CRM-System synchronisieren oder explizit Firmen mit der API erstellen. Es wird außerdem empfohlen, die Firmen-ID als Linkfeld zu verwenden.

Wenn Sie mehrere Personen in Marketo haben, die Datensätze in CRM- oder Marketo-Nur-Datensätzen enthalten, wird ein benutzerdefiniertes Objekt, das mit einer Firma verknüpft ist, nicht mehr als einem einzelnen Datensatz zugeordnet. Dies liegt daran, dass eine Firma, die mehrere Personen darunter hat, nur dann unterstützt wird, wenn Firmen aus dem CRM synchronisiert werden oder wenn Sie eine API verwenden, um explizit Firmen zu erstellen.

Benutzerdefinierte Objekte können nur direkt mit einem einzelnen Datensatz verknüpft werden. Wenn Ihr benutzerdefinierter Objekttyp durch ein Feld &quot;Firma&quot;verknüpft ist, sollten Sie sicherstellen, dass Ihre Personendaten entweder einer Firma zugeordnet werden, indem Sie die Kontaktkonversion in Ihrem CRM verwenden oder das Feld externalCompanyId verwenden, wenn Sie Firmen mit den REST-APIs von Marketo verwalten. Bei Personendatensätzen, die nicht explizit mit Firmen verknüpft sind, werden mit Firma verknüpfte benutzerdefinierte Objekte zufällig mit einem einzigen Datensatz verknüpft, selbst wenn der Wert des Felds &quot;Firma&quot;für viele Personen freigegeben wird.

Weitere Informationen finden Sie unter [Benutzerspezifische Objektdaten importieren](/help/marketo/product-docs/administration/marketo-custom-objects/import-custom-object-data.md).

>[!MORELIKETHIS]
>
>* [Benutzerdefinierte Marketo-Objekte erstellen](/help/marketo/product-docs/administration/marketo-custom-objects/create-marketo-custom-objects.md)
>* [Benutzerdefiniertes Objekt genehmigen](/help/marketo/product-docs/administration/marketo-custom-objects/approve-a-custom-object.md)
>* [Bearbeiten und Löschen eines benutzerdefinierten Marketo-Objekts](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Benutzerdefinierte Objektfelder Hinzufügen Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Benutzerdefinierte Marketo-Objektfelder bearbeiten und löschen](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [Benutzerdefinierte Objektdaten importieren](/help/marketo/product-docs/administration/marketo-custom-objects/import-custom-object-data.md)

