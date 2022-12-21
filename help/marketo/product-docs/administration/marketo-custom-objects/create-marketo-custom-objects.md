---
unique-page-id: 10093192
description: Erstellen benutzerdefinierter Marketo-Objekte - Marketo-Dokumente - Produktdokumentation
title: Erstellen benutzerdefinierter Marketo-Objekte
exl-id: d68b41e1-a12b-436f-aad7-42c7264cd901
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---

# Erstellen benutzerdefinierter Marketo-Objekte {#create-marketo-custom-objects}

Verwenden Sie benutzerdefinierte Objekte in Marketo, um geschäftsspezifische Metriken zu verfolgen. Dies kann alles sein, von Autos bis zu Kursen - egal, was Sie in Marketo für Ihre Kampagnen modellieren möchten.

>[!NOTE]
>
>Sie können benutzerdefinierte Objekte so einrichten, dass sie 1:n oder n:n funktionieren. Sie erstellen das anfängliche Objekt auf die gleiche Weise, aber die Schritte unterscheiden sich, wenn Sie dem Objekt Felder hinzufügen. Siehe  [Grundlegendes zu benutzerdefinierten Marketo-Objekten](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) für weitere Informationen.

>[!NOTE]
>
>Sobald das benutzerdefinierte Objekt genehmigt wurde, können Sie keine Link- oder Deduplizierungsfelder erstellen, bearbeiten oder löschen.

## Erstellen eines benutzerdefinierten Objekts für eine 1:n-Struktur {#create-a-custom-object-for-a-one-to-many-structure}

In diesem Beispiel wird ein benutzerdefiniertes Objekt vom Typ Auto zur Verwendung in einer 1:n-Struktur gezeigt. Später erstellen Sie ein benutzerdefiniertes Kursobjekt und ein zwischengeschaltetes Objekt, das in einer n:n-Struktur verwendet werden kann.

1. Klicken **Admin** und in **Datenbankverwaltung** select **Benutzerdefinierte Marketo-Objekte**.

   ![](assets/image2016-1-18-13-3a12-3a19.png)

1. Klicken **Neues benutzerdefiniertes Objekt**.

   ![](assets/image2016-5-18-16-3a28-3a4.png)

   >[!NOTE]
   >
   >Auf der Registerkarte &quot;Benutzerdefinierte Marketo-Objekte&quot;werden alle benutzerdefinierten Objekte auf der rechten Seite sowie Details zu allen genehmigten Objekten angezeigt, einschließlich der Anzahl der Datensätze und Felder bei der letzten Aktualisierung.

1. Geben Sie einen Anzeigenamen ein. Der API-Name und der Plural-Name werden automatisch ausgefüllt. Geben Sie eine Beschreibung ein (optional).

   ![](assets/image2015-9-15-16-3a29-3a17.png)

   >[!NOTE]
   >
   >Sie können diese Felder beim Erstellen bearbeiten. Nach dem Speichern können Sie jedoch nur das Feld Plural-Name und die **In Lead-Detail anzeigen** festlegen.

1. Ziehen Sie die **In Lead-Detail anzeigen** Anzeige-Regler **Anzeigen** , wenn Sie benutzerdefinierte Objektdaten auf der Seite &quot;Lead-Datenbank&quot;anzeigen möchten. Klicken **Speichern**.

   ![](assets/image2015-9-15-16-3a32-3a2.png)

1. Die benutzerdefinierten Objektinformationen zeigen den eingegebenen Inhalt an. Beachten Sie, dass es sich im Status Entwurf befindet.

   ![](assets/image2015-9-15-16-3a38-3a22.png)

   Der nächste Schritt besteht darin, Felder hinzuzufügen [Erstellen eines benutzerdefinierten Objekts](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md).

   >[!NOTE]
   >
   >Sie können benutzerdefinierte Marketo-Objekte nur über einen Listenimport oder die [API](https://developers.marketo.com/documentation/rest/).

## Erstellen eines benutzerdefinierten Objekts für eine Viele-zu-viele-Struktur {#create-a-custom-object-for-a-many-to-many-structure}

Dieses Beispiel zeigt ein benutzerdefiniertes Kursobjekt, mit dem Sie eine n:n-Beziehung zwischen Personen/Unternehmen und Kursen erstellen können. Wenn Sie fertig sind, erstellen Sie ein Zwischenobjekt, um es mit Personen oder Unternehmen in Ihrer Datenbank zu verbinden.

>[!NOTE]
>
>Für eine n:n-Beziehung müssen Sie keine Verknüpfung im benutzerdefinierten Objekt erstellen. Stattdessen fügen Sie dem zwischengeschalteten Objekt zwei Links hinzu (siehe unten).

1. Klicken **Admin** und in **Datenbankverwaltung** select **Benutzerdefinierte Marketo-Objekte**.

   ![](assets/image2016-1-18-13-3a16-3a25.png)

1. Klicken **Neues benutzerdefiniertes Objekt**.

   ![](assets/image2016-5-18-16-3a32-3a42.png)

1. Geben Sie einen Anzeigenamen ein. Der API-Name und der Plural-Name werden automatisch ausgefüllt. Geben Sie eine Beschreibung ein (optional).

   ![](assets/image2016-1-14-13-3a38-3a46.png)

   >[!NOTE]
   >
   >Sie können diese Felder beim Erstellen bearbeiten. Nach dem Speichern können Sie jedoch nur das Feld Plural-Name und die **In Lead-Detail anzeigen** festlegen.

1. Ziehen Sie die **In Lead-Detail anzeigen** Anzeige-Regler **Anzeigen** , wenn Sie benutzerdefinierte Objektdaten auf der Seite &quot;Lead-Datenbank&quot;anzeigen möchten. Klicken **Speichern**.

   ![](assets/image2016-1-14-13-3a42-3a56.png)

1. Die benutzerdefinierten Objektinformationen zeigen den eingegebenen Inhalt an. Beachten Sie, dass es sich im Status Entwurf befindet.

   ![](assets/image2016-1-18-8-3a38-3a58.png)

   >[!NOTE]
   >
   >Sie können benutzerdefinierte Marketo-Objekte nur über einen Listenimport oder die [API](https://developers.marketo.com/documentation/rest/).

Der nächste Schritt besteht darin, Ihr Zwischenobjekt zu erstellen (siehe unten). Zuvor müssen Sie jedoch ein Feld erstellen, zu dem eine Verknüpfung hergestellt werden soll.

## Zwischenobjekt erstellen {#create-an-intermediary-object}

Verwenden Sie ein zwischengeschaltetes Objekt, um ein benutzerdefiniertes Objekt mit Personen oder Unternehmen zu verbinden. In diesem Beispiel wird es verwendet, um Kurse in Ihrem Kurs benutzerdefiniertes Objekt mit Personen oder Unternehmen in Ihrer Datenbank zu verbinden.

>[!NOTE]
>
>Es ist nicht erforderlich, ein Zwischenobjekt für eine 1:n-benutzerdefinierte Objektstruktur zu erstellen.

1. Klicken **Admin** und in **Datenbankverwaltung** auswählen **Benutzerdefinierte Marketo-Objekte**.

   ![](assets/image2016-1-18-13-3a17-3a40.png)

1. Klicken **Neues benutzerdefiniertes Objekt**.

   ![](assets/image2016-5-18-16-3a33-3a16.png)

1. Geben Sie einen Anzeigenamen ein. Der API-Name und der Plural-Name werden automatisch ausgefüllt. Geben Sie eine Beschreibung ein (optional).

   ![](assets/image2016-1-14-14-3a10-3a44.png)

   >[!NOTE]
   >
   >Sie können diese Felder beim Erstellen bearbeiten. Nach dem Speichern können Sie jedoch nur das Feld Plural-Name und den Regler In Lead-Detail anzeigen bearbeiten.

1. Ziehen Sie die **In Lead-Detail anzeigen** Anzeige-Regler **Anzeigen** , wenn Sie benutzerdefinierte Objektdaten auf der Seite &quot;Lead-Datenbank&quot;anzeigen möchten. Klicken **Speichern**.

   ![](assets/image2016-1-14-14-3a12-3a49.png)

1. Die benutzerdefinierten Objektinformationen zeigen den eingegebenen Inhalt an. Beachten Sie, dass es sich im Status Entwurf befindet.

   Der nächste Schritt ist, dass Sie [Verknüpfungsfelder hinzufügen](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md) , um Ihr zwischengeschaltetes Objekt mit einer Person/Firma und einem benutzerdefinierten Objekt zu verbinden.

>[!MORELIKETHIS]
>
>* [Benutzerdefinierte Marketo-Objektfelder hinzufügen](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Benutzerdefinierte Marketo-Objektverknüpfungsfelder hinzufügen](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Grundlegendes zu benutzerdefinierten Marketo-Objekten](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

