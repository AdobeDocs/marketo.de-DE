---
unique-page-id: 10094188
description: Genehmigen eines benutzerdefinierten Objekts - Marketo-Dokumente - Produktdokumentation
title: Genehmigen eines benutzerdefinierten Objekts
exl-id: 8bae94df-91fe-4722-8c75-c26df882c65d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# Genehmigen eines benutzerdefinierten Objekts {#approve-a-custom-object}

Sie müssen ein benutzerdefiniertes Objekt genehmigen, bevor Sie es verwenden können. Der Prozess unterscheidet sich geringfügig von neuen benutzerdefinierten Objekten und Objekten, die Sie bearbeitet haben.

## Genehmigen eines neuen benutzerdefinierten Objekts {#approve-a-new-custom-object}

Sie haben ein ganz neues benutzerdefiniertes Objekt erstellt. So kann man es genehmigen.

1. Klicken Sie in Admin auf **Benutzerdefinierte Marketo-Objekte** und wählen Sie ein Objekt mit dem Status Entwurf aus.

   ![](assets/one.png)

1. Klicken Sie auf **Benutzerdefinierte Objektaktionen** und wählen Sie **Objekt genehmigen**.

   ![](assets/two.png)

1. Der Status ändert sich in Genehmigt .

   ![](assets/three.png)

   >[!NOTE]
   >
   >Ein benutzerdefiniertes Objekt, das in einer _Eins-zu-viele-Struktur_ muss über mindestens ein dedupliziertes Feld, ein Verknüpfungsfeld, einen verknüpften Objektnamen und einen verknüpften Feldnamen verfügen, der genehmigt werden soll.
   >
   >Ein benutzerdefiniertes Objekt, das in einer _Viele-zu-viele-Struktur_ **nicht** bei der Validierung ein Verknüpfungsfeld, einen verknüpften Objektnamen oder einen verknüpften Feldnamen benötigen (da sie sich im Intermediarobjekt befinden).
   >
   >Ein benutzerdefiniertes Objekt, das als _zwischengeschaltetes Objekt_ erfordert ein Verknüpfungsfeld, einen verknüpften Objektnamen und einen verknüpften Feldnamen, aber **nicht** erfordert ein dedupliziertes Feld.
   >
   >Siehe [Grundlegendes zu benutzerdefinierten Marketo-Objekten](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) für weitere Informationen.

Das ist es! Jetzt können Sie Ihr benutzerdefiniertes Objekt in den Begrenzungen Ihrer Filter und Trigger auswählen, die in Ihren Kampagnen verwendet werden sollen.

## Genehmigen eines bearbeiteten benutzerdefinierten Objekts {#approve-an-edited-custom-object}

Nachdem Sie ein genehmigtes benutzerdefiniertes Objekt bearbeitet haben, müssen Sie den Entwurf genehmigen, um das benutzerdefinierte Objekt in den Status &quot;Genehmigt&quot;zurückzugeben.

1. Wenn Sie ein bereits genehmigtes benutzerdefiniertes Objekt bearbeiten, erhält es den Status Genehmigt mit Entwurf .

   ![](assets/four.png)

1. Wenn Sie bereit sind, den Entwurf zu genehmigen, klicken Sie auf die Schaltfläche **Benutzerdefinierte Objektaktionen** und wählen Sie **Objekt genehmigen**.

   ![](assets/five-1.png)

1. Eine Vorschau zeigt die Elemente an, die im Entwurf geändert wurden. Klicken **Genehmigen**.

   ![](assets/six-1.png)
