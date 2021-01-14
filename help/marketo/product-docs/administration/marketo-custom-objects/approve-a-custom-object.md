---
unique-page-id: 10094188
description: Benutzerdefiniertes Objekt genehmigen - Marketing Docs - Produktdokumentation
title: Benutzerdefiniertes Objekt genehmigen
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# Benutzerdefiniertes Objekt {#approve-a-custom-object} genehmigen

Sie müssen ein benutzerdefiniertes Objekt genehmigen, bevor Sie es verwenden können. Der Prozess unterscheidet sich geringfügig von den neuen benutzerdefinierten Objekten und Objekten, die Sie bearbeitet haben.

## Neues benutzerdefiniertes Objekt {#approve-a-new-custom-object} genehmigen

Sie haben ein ganz neues benutzerdefiniertes Objekt erstellt. Hier ist, wie man es genehmigt.

1. Klicken Sie in Admin auf **Benutzerdefinierte Objekte** markieren und wählen Sie ein Objekt mit dem Status &quot;Entwurf&quot;aus.

   ![](assets/one.png)

1. Klicken Sie auf die Dropdownliste **Benutzerspezifische Objektaktionen** und wählen Sie **Objekt genehmigen**.

   ![](assets/two.png)

1. Der Status ändert sich in Genehmigt.

   ![](assets/three.png)

   >[!NOTE]
   >
   >Ein benutzerdefiniertes Objekt, das in einer _1-zu-n-Struktur_ verwendet wird, muss mindestens ein dedupliziertes Feld, ein Verknüpfungsfeld, einen verknüpften Objektnamen und einen verknüpften Feldnamen haben, um genehmigt zu werden.
   >
   >Ein benutzerdefiniertes Objekt, das in einer _Viele-zu-viele-Struktur_ **verwendet wird, benötigt bei der Genehmigung des Objekts kein Verknüpfungsfeld, einen verknüpften Objektnamen oder einen verknüpften Feldnamen (da diese im Zwischenobjekt leben).**
   >
   >Ein benutzerdefiniertes Objekt, das als _intermediäres Objekt_ verwendet wird, erfordert ein Verknüpfungsfeld, einen verknüpften Objektnamen und einen verknüpften Feldnamen, **erfordert jedoch kein dedupliziertes Feld.**
   >
   >Weitere Informationen finden Sie unter [Informationen zu &quot;Markieren zu benutzerdefinierten Objekten](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)&quot;.

Das ist&#39;s! Jetzt können Sie Ihr benutzerdefiniertes Objekt in den Einschränkungen Ihrer Filter und Trigger auswählen, die Sie in Ihren Kampagnen verwenden möchten.

## Genehmigen eines bearbeiteten benutzerdefinierten Objekts {#approve-an-edited-custom-object}

Nachdem Sie ein genehmigtes benutzerdefiniertes Objekt bearbeitet haben, müssen Sie den Entwurf genehmigen, um das benutzerdefinierte Objekt in den Status &quot;Genehmigt&quot;zurückzugeben.

1. Wenn Sie ein bereits genehmigtes benutzerdefiniertes Objekt bearbeiten, erhält es den Status &quot;Genehmigt mit Entwurf&quot;.

   ![](assets/four.png)

1. Wenn Sie bereit sind, den Entwurf zu genehmigen, klicken Sie auf die Dropdownliste **Benutzerspezifische Objektaktionen** und wählen Sie **Objekt genehmigen**.

   ![](assets/five-1.png)

1. Eine Vorschau zeigt die Elemente an, die im Entwurf geändert wurden. Klicken Sie auf **Genehmigen**.

   ![](assets/six-1.png)
