---
unique-page-id: 10094188
description: Genehmigen neuer oder bearbeiteter benutzerdefinierter Objekte in Admin, einschließlich Anforderungen für 1:n-, n:n- und dazwischenliegende Objekte.
title: Genehmigen eines benutzerdefinierten Objekts
exl-id: 8bae94df-91fe-4722-8c75-c26df882c65d
feature: Custom Objects
TQID: https://experienceleague.adobe.com/CH2VbeVfaADWe4rVfRwgM3nrKXw85eMYbgCa99gTPFY
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 303
ht-degree: 2%

---

# Genehmigen eines benutzerdefinierten Objekts {#approve-a-custom-object}

Sie müssen ein benutzerdefiniertes Objekt genehmigen, bevor Sie es verwenden können. Der Prozess unterscheidet sich geringfügig von dem für neue benutzerdefinierte Objekte und für Objekte, die Sie bearbeitet haben.

## Genehmigen eines neuen benutzerdefinierten Objekts {#approve-a-new-custom-object}

Ein neues benutzerdefiniertes Objekt wurde erstellt. Gehen Sie wie folgt vor, um ihn zu genehmigen.

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/approve-a-custom-object-1.png)

1. Klicken Sie auf **[!UICONTROL Benutzerdefinierte Marketo-Objekte]**.

   ![](assets/approve-a-custom-object-2.png)

1. Wählen Sie ein Objekt aus, das sich im Status Entwurf befindet.

   ![](assets/approve-a-custom-object-3.png)

1. Klicken Sie auf **[!UICONTROL Dropdown-Liste Benutzerdefinierte]** und wählen Sie **[!UICONTROL Objekt genehmigen]**.

   ![](assets/approve-a-custom-object-4.png)

1. Der Status ändert sich in [!UICONTROL Genehmigt].

   ![](assets/approve-a-custom-object-5.png)

   >[!NOTE]
   >
   >Ein benutzerdefiniertes Objekt, das in einer _1:n-Struktur_ verwendet wird, muss mindestens ein Deduplizierungsfeld, ein Verknüpfungsfeld, einen verknüpften Objektnamen und einen verknüpften Feldnamen aufweisen, damit es genehmigt werden kann.
   >
   >Ein benutzerdefiniertes Objekt, das in einer _n:n-Struktur_ verwendet **,** bei der Genehmigung ein Verknüpfungsfeld, einen verknüpften Objektnamen oder einen verknüpften Feldnamen (da sie sich im Zwischenobjekt befinden).
   >
   >Ein benutzerdefiniertes Objekt, das als _Zwischenobjekt_ verwendet wird, erfordert ein Verknüpfungsfeld, einen verknüpften Objektnamen und einen verknüpften Feldnamen, **jedoch** Deduplizierungsfeld.
   >
   >Weitere Informationen [ Sie unter „Grundlegendes ](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) benutzerdefinierten Marketo-Objekten“.

Jetzt können Sie Ihr benutzerdefiniertes Objekt in den Einschränkungen Ihrer Filter und Trigger auswählen, die in Ihren Kampagnen verwendet werden sollen.

## Genehmigen eines bearbeiteten benutzerdefinierten Objekts {#approve-an-edited-custom-object}

Nachdem Sie ein genehmigtes benutzerdefiniertes Objekt bearbeitet haben, müssen Sie den Entwurf genehmigen, um das benutzerdefinierte Objekt in einen genehmigten Status zurückzuversetzen.

1. Wenn Sie ein bereits genehmigtes benutzerdefiniertes Objekt bearbeiten, erhält es den Status [!UICONTROL Genehmigt mit Entwurf].

   ![](assets/approve-a-custom-object-6.png)

1. Wenn Sie bereit sind, den Entwurf zu genehmigen, klicken Sie auf **[!UICONTROL Dropdown-Liste Benutzerdefinierte]** und wählen Sie **[!UICONTROL Objekt genehmigen]**.

   ![](assets/approve-a-custom-object-7.png)

1. Eine Vorschau zeigt die Elemente an, die im Entwurf geändert wurden. Klicken Sie **[!UICONTROL Genehmigen]**.

   ![](assets/approve-a-custom-object-8.png)
