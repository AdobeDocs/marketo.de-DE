---
unique-page-id: 10093192
description: Erstellen benutzerdefinierter Marketo-Objekte - Marketo-Dokumente - Produktdokumentation
title: Erstellen benutzerdefinierter Marketo-Objekte
exl-id: d68b41e1-a12b-436f-aad7-42c7264cd901
feature: Custom Objects
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 0%

---

# Erstellen benutzerdefinierter Marketo-Objekte {#create-marketo-custom-objects}

Verwenden Sie benutzerdefinierte Objekte in Marketo, um geschäftsspezifische Metriken zu verfolgen. Dies kann alles sein, von Autos bis zu Kursen - egal, was Sie in Marketo für Ihre Kampagnen modellieren möchten.

>[!NOTE]
>
>Sie können benutzerdefinierte Objekte so einrichten, dass sie 1:n oder n:n funktionieren. Sie erstellen das anfängliche Objekt auf die gleiche Weise, aber die Schritte unterscheiden sich, wenn Sie dem Objekt Felder hinzufügen. Weitere Informationen finden Sie unter [Grundlegendes zu benutzerdefinierten Marketo-Objekten](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) .

>[!NOTE]
>
>Sobald das benutzerdefinierte Objekt genehmigt wurde, können Sie keine Link- oder Deduplizierungsfelder erstellen, bearbeiten oder löschen.

## Erstellen eines benutzerdefinierten Objekts für eine 1:n-Struktur {#create-a-custom-object-for-a-one-to-many-structure}

In diesem Beispiel wird ein benutzerdefiniertes Objekt vom Typ Auto zur Verwendung in einer 1:n-Struktur gezeigt. Später erstellen Sie ein benutzerdefiniertes Kursobjekt und ein zwischengeschaltetes Objekt, das in einer n:n-Struktur verwendet werden kann.

1. Wechseln Sie zum Bereich **[!UICONTROL Admin]** .

   ![](assets/create-marketo-custom-objects-1.png)

1. Klicken Sie auf **[!UICONTROL Marketo Custom Objects]**.

   ![](assets/create-marketo-custom-objects-2.png)

1. Klicken Sie auf **[!UICONTROL Neues benutzerdefiniertes Objekt]**.

   ![](assets/create-marketo-custom-objects-3.png)

   >[!NOTE]
   >
   >Auf der Registerkarte [!UICONTROL Benutzerdefinierte Marketo-Objekte] werden alle benutzerdefinierten Objekte auf der rechten Seite sowie Details zu allen genehmigten Objekten angezeigt, einschließlich der Anzahl der Datensätze und Felder bei der letzten Aktualisierung.

1. Geben Sie einen [!UICONTROL Anzeigenamen] ein. Der [!UICONTROL API-Name] und der [!UICONTROL Plural-Name] werden automatisch ausgefüllt. Geben Sie eine [!UICONTROL Beschreibung] ein (optional).

   ![](assets/create-marketo-custom-objects-4.png)

   >[!NOTE]
   >
   >Sie können diese Felder bearbeiten, wenn Sie sie erstellen, aber nachdem sie gespeichert wurden, können Sie nur das Feld [!UICONTROL Plural Name] und den Schieberegler **[!UICONTROL In Lead-Detail anzeigen]** bearbeiten.

1. Ziehen Sie den Schieberegler **[!UICONTROL Im Lead-Detail anzeigen]** nach oben, um den Schieberegler **[!UICONTROL Anzeigen]** anzuzeigen, wenn Sie benutzerdefinierte Objektdaten auf der Datenbankseite anzeigen möchten. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/create-marketo-custom-objects-5.png)

1. Die benutzerdefinierten Objektinformationen zeigen den eingegebenen Inhalt an. Beachten Sie, dass es sich im Status Entwurf befindet.

   ![](assets/create-marketo-custom-objects-6.png)

   Der nächste Schritt besteht darin, Felder zu [ hinzuzufügen, um Ihr benutzerdefiniertes Objekt zu erstellen](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md).

   >[!NOTE]
   >
   >Sie können benutzerdefinierte Marketo-Objekte nur über einen Listenimport oder die [API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api) füllen.

## Erstellen eines benutzerdefinierten Objekts für eine Viele-zu-viele-Struktur {#create-a-custom-object-for-a-many-to-many-structure}

Dieses Beispiel zeigt ein benutzerdefiniertes Kursobjekt, mit dem Sie eine n:n-Beziehung zwischen Personen/Unternehmen und Kursen erstellen können. Wenn Sie fertig sind, erstellen Sie ein Zwischenobjekt, um es mit Personen oder Unternehmen in Ihrer Datenbank zu verbinden.

>[!NOTE]
>
>Für eine n:n-Beziehung müssen Sie keine Verknüpfung im benutzerdefinierten Objekt erstellen. Stattdessen fügen Sie dem zwischengeschalteten Objekt zwei Links hinzu (siehe unten).

1. Wechseln Sie zum Bereich **[!UICONTROL Admin]** .

   ![](assets/create-marketo-custom-objects-7.png)

1. Klicken Sie auf **[!UICONTROL Marketo Custom Objects]**.

   ![](assets/create-marketo-custom-objects-8.png)

1. Klicken Sie auf **[!UICONTROL Neues benutzerdefiniertes Objekt]**.

   ![](assets/create-marketo-custom-objects-9.png)

1. Geben Sie einen [!UICONTROL Anzeigenamen] ein. Der [!UICONTROL API-Name] und der [!UICONTROL Plural-Name] werden automatisch ausgefüllt. Geben Sie eine [!UICONTROL Beschreibung] ein (optional).

   ![](assets/create-marketo-custom-objects-10.png)

   >[!NOTE]
   >
   >Sie können diese Felder bearbeiten, wenn Sie sie erstellen, aber nachdem sie gespeichert wurden, können Sie nur das Feld [!UICONTROL Plural Name] und den Schieberegler **[!UICONTROL In Lead-Detail anzeigen]** bearbeiten.

1. Ziehen Sie den Schieberegler **[!UICONTROL Im Lead-Detail anzeigen]** nach oben, um den Schieberegler **[!UICONTROL Anzeigen]** anzuzeigen, wenn Sie benutzerdefinierte Objektdaten auf der Datenbankseite anzeigen möchten. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/create-marketo-custom-objects-11.png)

1. Die benutzerdefinierten Objektinformationen zeigen den eingegebenen Inhalt an. Beachten Sie, dass es sich im Status Entwurf befindet.

   ![](assets/create-marketo-custom-objects-12.png)

   >[!NOTE]
   >
   >Sie können benutzerdefinierte Marketo-Objekte nur über einen Listenimport oder die [API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/rest-api) füllen.

Der nächste Schritt besteht darin, Ihr Zwischenobjekt zu erstellen (siehe unten). Zuvor müssen Sie jedoch ein Feld erstellen, zu dem eine Verknüpfung hergestellt werden soll.

## Zwischenobjekt erstellen {#create-an-intermediary-object}

Verwenden Sie ein zwischengeschaltetes Objekt, um ein benutzerdefiniertes Objekt mit Personen oder Unternehmen zu verbinden. In diesem Beispiel wird es verwendet, um Kurse in Ihrem Kurs benutzerdefiniertes Objekt mit Personen oder Unternehmen in Ihrer Datenbank zu verbinden.

>[!NOTE]
>
>Es ist nicht erforderlich, ein Zwischenobjekt für eine 1:n-benutzerdefinierte Objektstruktur zu erstellen.

1. Wechseln Sie zum Bereich **[!UICONTROL Admin]** .

   ![](assets/create-marketo-custom-objects-13.png)

1. Klicken Sie auf **[!UICONTROL Marketo Custom Objects]**.

   ![](assets/create-marketo-custom-objects-14.png)

1. Klicken Sie auf **[!UICONTROL Neues benutzerdefiniertes Objekt]**.

   ![](assets/create-marketo-custom-objects-15.png)

1. Geben Sie einen [!UICONTROL Anzeigenamen] ein. Der [!UICONTROL API-Name] und der [!UICONTROL Plural-Name] werden automatisch ausgefüllt. Geben Sie eine [!UICONTROL Beschreibung] ein (optional).

   ![](assets/create-marketo-custom-objects-16.png)

   >[!NOTE]
   >
   >Sie können diese Felder bearbeiten, wenn Sie sie erstellen, aber nachdem sie gespeichert wurden, können Sie nur das Feld [!UICONTROL Plural Name] und den Schieberegler [!UICONTROL In Lead-Detail anzeigen] bearbeiten.

1. Ziehen Sie den Schieberegler **[!UICONTROL Im Lead-Detail anzeigen]** nach oben, um den Schieberegler **Anzeigen** anzuzeigen, wenn Sie benutzerdefinierte Objektdaten auf der Datenbankseite anzeigen möchten. Klicken Sie auf **Speichern**.

   ![](assets/create-marketo-custom-objects-17.png)

1. Die benutzerdefinierten Objektinformationen zeigen den eingegebenen Inhalt an. Beachten Sie, dass es sich im Status Entwurf befindet.

   Der nächste Schritt besteht darin, dass Sie [Verknüpfungsfelder hinzufügen](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md), um Ihr Zwischenobjekt mit einer Person/Firma und einem benutzerdefinierten Objekt zu verbinden.

>[!MORELIKETHIS]
>
>* [Benutzerdefinierte Marketo-Objektfelder hinzufügen](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Benutzerdefinierte Marketo-Objektverknüpfungsfelder hinzufügen](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Grundlegendes zu benutzerdefinierten Marketo-Objekten](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
