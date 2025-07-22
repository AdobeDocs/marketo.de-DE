---
unique-page-id: 10093192
description: Erstellen benutzerdefinierter Marketo-Objekte - Marketo-Dokumente - Produktdokumentation
title: Erstellen benutzerdefinierter Marketo-Objekte
exl-id: d68b41e1-a12b-436f-aad7-42c7264cd901
feature: Custom Objects
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '698'
ht-degree: 0%

---

# Erstellen benutzerdefinierter Marketo-Objekte {#create-marketo-custom-objects}

Verwenden Sie benutzerdefinierte Objekte in Marketo, um für Ihr Unternehmen spezifische Metriken zu verfolgen. Dies kann alles sein, von Autos bis hin zu Kursen - was auch immer Sie in Marketo modellieren möchten, um Ihre Kampagnen durchzuführen.

>[!NOTE]
>
>Sie können benutzerdefinierte Objekte so einrichten, dass sie 1:n oder n:n funktionieren. Sie erstellen das anfängliche -Objekt auf die gleiche Weise, aber die Schritte unterscheiden sich, wenn Sie dem -Objekt Felder hinzufügen. Weitere Informationen [ Sie unter „Grundlegendes ](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) benutzerdefinierten Marketo-Objekten“.

>[!NOTE]
>
>Sie können kein Link- oder Deduplizierungsfeld erstellen, bearbeiten oder löschen, nachdem das benutzerdefinierte Objekt genehmigt wurde.

## Erstellen eines benutzerdefinierten Objekts für eine Eins-zu-Viele-Struktur {#create-a-custom-object-for-a-one-to-many-structure}

Dieses Beispiel zeigt ein benutzerdefiniertes Auto-Objekt zur Verwendung in einer Eins-zu-Viele-Struktur. Später erstellen Sie ein benutzerdefiniertes Kursobjekt und ein Zwischenobjekt, das in einer n:n-Struktur verwendet werden kann.

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/create-marketo-custom-objects-1.png)

1. Klicken Sie auf **[!UICONTROL Benutzerdefinierte Marketo-Objekte]**.

   ![](assets/create-marketo-custom-objects-2.png)

1. Klicken Sie auf **[!UICONTROL Neues benutzerdefiniertes Objekt]**.

   ![](assets/create-marketo-custom-objects-3.png)

   >[!NOTE]
   >
   >Auf der Registerkarte [!UICONTROL Benutzerdefinierte Marketo]Objekte: werden alle benutzerdefinierten Objekte auf der rechten Seite sowie Details zu allen genehmigten Objekten angezeigt, einschließlich der Anzahl der Datensätze und Felder bei der letzten Aktualisierung.

1. Geben Sie einen [!UICONTROL Anzeigenamen] ein. Die [!UICONTROL API-Name] und [!UICONTROL Plural-Name] werden automatisch ausgefüllt. Geben Sie einen [!UICONTROL Beschreibung] ein (optional).

   ![](assets/create-marketo-custom-objects-4.png)

   >[!NOTE]
   >
   >Sie können diese Felder beim Erstellen bearbeiten, aber nach dem Speichern können Sie nur das Feld „Pluraler Name[!UICONTROL &#x200B; und &#x200B;] Regler **[!UICONTROL In Lead-Detail anzeigen]** bearbeiten.

1. Ziehen Sie den **[!UICONTROL „In Lead-Detail anzeigen]** auf den Regler, um **[!UICONTROL Anzeigen]** anzuzeigen, wenn Sie benutzerdefinierte Objektdaten auf der Seite „Datenbank“ anzeigen möchten. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/create-marketo-custom-objects-5.png)

1. Die Informationen zum benutzerdefinierten Objekt zeigen den eingegebenen Inhalt an. Beachten Sie, dass er den Status **[!UICONTROL Entwurf]** aufweist.

   ![](assets/create-marketo-custom-objects-6.png)

   Der nächste Schritt besteht darin, Felder hinzuzufügen [Ihr benutzerdefiniertes Objekt erstellen](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md).

   >[!NOTE]
   >
   >Sie können benutzerdefinierte Marketo-Objekte nur über einen Listen-Import oder die [API) ](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/rest-api).

## Erstellen eines benutzerdefinierten Objekts für eine Viele-zu-viele-Struktur {#create-a-custom-object-for-a-many-to-many-structure}

Dieses Beispiel zeigt ein benutzerdefiniertes Kursobjekt, das Sie zum Erstellen einer n:n-Beziehung zwischen Personen/Unternehmen und Kursen verwenden werden. Wenn Sie fertig sind, erstellen Sie ein Zwischenobjekt, um es mit Personen oder Unternehmen in Ihrer Datenbank zu verbinden.

>[!NOTE]
>
>Bei einer Viele-zu-viele-Beziehung müssen Sie keine Relation im benutzerdefinierten -Objekt erstellen. Stattdessen fügen Sie zwei Links zum Zwischenobjekt hinzu (siehe unten).

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/create-marketo-custom-objects-7.png)

1. Klicken Sie auf **[!UICONTROL Benutzerdefinierte Marketo-Objekte]**.

   ![](assets/create-marketo-custom-objects-8.png)

1. Klicken Sie auf **[!UICONTROL Neues benutzerdefiniertes Objekt]**.

   ![](assets/create-marketo-custom-objects-9.png)

1. Geben Sie einen [!UICONTROL Anzeigenamen] ein. Die [!UICONTROL API-Name] und [!UICONTROL Plural-Name] werden automatisch ausgefüllt. Geben Sie einen [!UICONTROL Beschreibung] ein (optional).

   ![](assets/create-marketo-custom-objects-10.png)

   >[!NOTE]
   >
   >Sie können diese Felder beim Erstellen bearbeiten, aber nach dem Speichern können Sie nur das Feld „Pluraler Name[!UICONTROL &#x200B; und &#x200B;] Regler **[!UICONTROL In Lead-Detail anzeigen]** bearbeiten.

1. Ziehen Sie den **[!UICONTROL „In Lead-Detail anzeigen]** auf den Regler, um **[!UICONTROL Anzeigen]** anzuzeigen, wenn Sie benutzerdefinierte Objektdaten auf der Seite „Datenbank“ anzeigen möchten. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/create-marketo-custom-objects-11.png)

1. Die Informationen zum benutzerdefinierten Objekt zeigen den eingegebenen Inhalt an. Beachten Sie, dass er den Status **[!UICONTROL Entwurf]** aufweist.

   ![](assets/create-marketo-custom-objects-12.png)

   >[!NOTE]
   >
   >Sie können benutzerdefinierte Marketo-Objekte nur über einen Listen-Import oder die [API) ](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/rest-api).

Im nächsten Schritt erstellen Sie Ihr Zwischenobjekt (siehe unten). Zuvor müssen Sie jedoch ein Feld erstellen, mit dem eine Verknüpfung hergestellt werden kann.

## Erstellen eines Zwischenobjekts {#create-an-intermediary-object}

Verwenden Sie ein Zwischenobjekt, um ein benutzerdefiniertes Objekt mit Personen oder Unternehmen zu verbinden. In diesem Beispiel wird es verwendet, um Kurse in Ihrem benutzerdefinierten Kursobjekt mit Personen oder Unternehmen in Ihrer Datenbank zu verbinden.

>[!NOTE]
>
>Für eine benutzerdefinierte Eins-zu-viele-Objektstruktur müssen Sie kein Zwischenobjekt erstellen.

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/create-marketo-custom-objects-13.png)

1. Klicken Sie auf **[!UICONTROL Benutzerdefinierte Marketo-Objekte]**.

   ![](assets/create-marketo-custom-objects-14.png)

1. Klicken Sie auf **[!UICONTROL Neues benutzerdefiniertes Objekt]**.

   ![](assets/create-marketo-custom-objects-15.png)

1. Geben Sie einen [!UICONTROL Anzeigenamen] ein. Die [!UICONTROL API-Name] und [!UICONTROL Plural-Name] werden automatisch ausgefüllt. Geben Sie einen [!UICONTROL Beschreibung] ein (optional).

   ![](assets/create-marketo-custom-objects-16.png)

   >[!NOTE]
   >
   >Sie können diese Felder beim Erstellen bearbeiten, aber nach dem Speichern können Sie nur das Feld „Pluraler Name[!UICONTROL &#x200B; und &#x200B;] Regler [!UICONTROL In Lead-Detail anzeigen] bearbeiten.

1. Ziehen Sie den **[!UICONTROL „In Lead-Detail anzeigen]** auf den Regler, um **Anzeigen** anzuzeigen, wenn Sie benutzerdefinierte Objektdaten auf der Seite „Datenbank“ anzeigen möchten. Klicken Sie auf **Speichern**.

   ![](assets/create-marketo-custom-objects-17.png)

1. Die Informationen zum benutzerdefinierten Objekt zeigen den eingegebenen Inhalt an. Beachten Sie, dass er den Status **[!UICONTROL Entwurf]** aufweist.

   Der nächste Schritt besteht darin, [Verknüpfungsfelder hinzufügen](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md) um Ihr Zwischenobjekt mit einer Person/Firma und einem benutzerdefinierten Objekt zu verbinden.

>[!MORELIKETHIS]
>
>* [Benutzerdefinierte Marketo-Objektfelder hinzufügen](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Benutzerdefinierte Objektverknüpfungsfelder für Marketo hinzufügen](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Grundlegendes zu benutzerdefinierten Marketo-Objekten](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
