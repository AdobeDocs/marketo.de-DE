---
unique-page-id: 10094188
description: Benutzerdefiniertes Objekt genehmigen - Marketing Docs - Produktdokumentation
title: Benutzerdefiniertes Objekt genehmigen
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# Benutzerdefiniertes Objekt genehmigen {#approve-a-custom-object}

Sie müssen ein benutzerdefiniertes Objekt genehmigen, bevor Sie es verwenden können. Der Prozess unterscheidet sich geringfügig von den neuen benutzerdefinierten Objekten und Objekten, die Sie bearbeitet haben.

## Neues benutzerdefiniertes Objekt genehmigen {#approve-a-new-custom-object}

Sie haben ein ganz neues benutzerdefiniertes Objekt erstellt. Hier ist, wie man es genehmigt.

1. Klicken Sie in Admin auf **Zu benutzerdefinierten Objekten** markieren und wählen Sie ein Objekt mit dem Status &quot;Entwurf&quot;aus.

   ![](assets/one.png)

1. Klicken Sie auf die Dropdown-Liste &quot; **Benutzerdefinierte Objektaktionen** &quot;und wählen Sie &quot;Objekt **genehmigen&quot;**.

   ![](assets/two.png)

1. Der Status ändert sich in Genehmigt.

   ![](assets/three.png)

   >[!NOTE]
   >
   >Ein benutzerdefiniertes Objekt, das in einer *Eins-zu-viele-Struktur* verwendet wird, muss mindestens ein dedupliziertes Feld, ein Verknüpfungsfeld, einen verknüpften Objektnamen und einen verknüpften Feldnamen haben, damit die Genehmigung erteilt werden kann.
   >
   >
   >Ein benutzerdefiniertes Objekt, das in einer *Viele-zu-viele-Struktur* verwendet wird, **benötigt bei der Genehmigung des Objekts kein** Verknüpfungsfeld, keinen verknüpften Objektnamen oder keinen verknüpften Feldnamen (da es im Zwischenobjekt lebt).
   >
   >
   >Ein benutzerdefiniertes Objekt, das als *Zwischenobjekt* verwendet wird, erfordert ein Verknüpfungsfeld, einen verknüpften Objektnamen und einen verknüpften Feldnamen, **erfordert jedoch kein** Deduplizierungsfeld.
   >
   >
   >Weitere Informationen finden Sie unter Informationen [zu benutzerdefinierten Objekten](understanding-marketo-custom-objects.md) .

Das ist&#39;s! Jetzt können Sie Ihr benutzerdefiniertes Objekt in den Einschränkungen Ihrer Filter und Auslöser auswählen, die in Ihren Kampagnen verwendet werden sollen.

## Bearbeiten eines benutzerdefinierten Objekts genehmigen {#approve-an-edited-custom-object}

Nachdem Sie ein genehmigtes benutzerdefiniertes Objekt bearbeitet haben, müssen Sie den Entwurf genehmigen, um das benutzerdefinierte Objekt in den Status &quot;Genehmigt&quot;zurückzugeben.

1. Wenn Sie ein bereits genehmigtes benutzerdefiniertes Objekt bearbeiten, erhält es den Status &quot;Genehmigt mit Entwurf&quot;.

   ![](assets/four.png)

1. Wenn Sie bereit sind, den Entwurf zu genehmigen, klicken Sie auf die Dropdown-Liste &quot; **Benutzerdefinierte Objektaktionen** &quot;und wählen Sie &quot;Objekt **genehmigen&quot;**.

   ![](assets/five-1.png)

1. Eine Vorschau zeigt die Elemente an, die im Entwurf geändert wurden. Klicken Sie auf **Genehmigen**.

   ![](assets/six-1.png)

