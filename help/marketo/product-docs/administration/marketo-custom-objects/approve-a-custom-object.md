---
unique-page-id: 10094188
description: Genehmigen eines benutzerdefinierten Objekts - Marketo-Dokumente - Produktdokumentation
title: Genehmigen eines benutzerdefinierten Objekts
exl-id: 8bae94df-91fe-4722-8c75-c26df882c65d
feature: Custom Objects
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 1%

---

# Genehmigen eines benutzerdefinierten Objekts {#approve-a-custom-object}

Sie müssen ein benutzerdefiniertes Objekt genehmigen, bevor Sie es verwenden können. Der Prozess unterscheidet sich geringfügig von neuen benutzerdefinierten Objekten und Objekten, die Sie bearbeitet haben.

## Genehmigen eines neuen benutzerdefinierten Objekts {#approve-a-new-custom-object}

Sie haben ein ganz neues benutzerdefiniertes Objekt erstellt. So kann man es genehmigen.

1. Navigieren Sie zum **[!UICONTROL Admin]**-Bereich.

   ![](assets/approve-a-custom-object-1.png)

1. Klicks **[!UICONTROL Benutzerdefinierte Marketo-Objekte]**.

   ![](assets/approve-a-custom-object-2.png)

1. Wählen Sie ein Objekt mit dem Status Entwurf aus.

   ![](assets/approve-a-custom-object-3.png)

1. Klicken Sie auf **[!UICONTROL Benutzerdefinierte Objektaktionen]** und wählen Sie **[!UICONTROL Objekt genehmigen]**.

   ![](assets/approve-a-custom-object-4.png)

1. Der Status ändert sich in [!UICONTROL Genehmigt].

   ![](assets/approve-a-custom-object-5.png)

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

1. Wenn Sie ein bereits genehmigtes benutzerdefiniertes Objekt bearbeiten, erhält es eine [!UICONTROL Genehmigt mit Entwurf] state.

   ![](assets/approve-a-custom-object-6.png)

1. Wenn Sie bereit sind, den Entwurf zu genehmigen, klicken Sie auf die Schaltfläche **[!UICONTROL Benutzerdefinierte Objektaktionen]** und wählen Sie **[!UICONTROL Objekt genehmigen]**.

   ![](assets/approve-a-custom-object-7.png)

1. Eine Vorschau zeigt die Elemente an, die im Entwurf geändert wurden. Klicks **[!UICONTROL Genehmigen]**.

   ![](assets/approve-a-custom-object-8.png)
