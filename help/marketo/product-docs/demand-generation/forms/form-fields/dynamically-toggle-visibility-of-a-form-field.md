---
unique-page-id: 2949962
description: Dynamisches Umschalten der Sichtbarkeit eines Formularfelds - Marketing-Dokumente - Produktdokumentation
title: Dynamisches Umschalten zwischen Sichtbarkeit eines Formularfelds
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---


# Dynamisches Umschalten der Sichtbarkeit eines Formularfelds {#dynamically-toggle-visibility-of-a-form-field}

>[!PREREQUISITES]
>
>* [hinzufügen einer Länderauswahl in Ihr Formular](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)


Eine wirklich coole Funktion von Marketo Forms ist, dass Sie Formularfelder oder [Feldsätze](/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md) dynamisch ein- und ausblenden können.

>[!NOTE]
>
>**Beispiel**
>
>In diesem Beispiel sollten wir das Feld **Bundesland** ausblenden, es sei denn, **Land** ist als &quot;Vereinigte Staaten&quot;ausgewählt.

1. Gehen Sie zu **Marketing-Aktivitäten**.

   ![](assets/login-marketing-activities-8.png)

1. Wählen Sie Ihr Formular aus und klicken Sie auf **Formular bearbeiten**.

   ![](assets/editform-1.png)

1. Wählen Sie das Feld aus, das dynamisch ein-/ausgeblendet werden soll, und klicken Sie auf den Link für **Sichtbarkeitsregeln**.

   ![](assets/image2014-9-15-15-3a16-3a0.png)

1. Suchen und wählen Sie das Feld aus, um das Sie eine Bedingung erstellen möchten.

   ![](assets/image2014-9-15-15-3a16-3a12.png)

1. Wählen Sie den Operator aus.

   >[!TIP]
   >
   >Das ist cool, weil Sie unscharfe Übereinstimmungen wie &quot;Beginn mit&quot;wählen können.

   ![](assets/image2014-9-15-15-3a16-3a50.png)

1. Wählen Sie die zu suchenden Werte aus und klicken Sie dann außerhalb der Dropdownliste auf .

   ![](assets/image2014-9-15-15-3a17-3a4.png)

   >[!TIP]
   >
   >Sie können mehrere Werte auswählen, indem Sie darauf klicken, während die Dropdown-Liste geöffnet ist. Sie können beispielsweise &quot;USA&quot;und &quot;Kanada&quot;auswählen.

   >[!NOTE]
   >
   >Zuvor haben wir Land in einen Feldtyp mit Pick-Liste umgewandelt und [alle Länder als Werte](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md) hinzugefügt.

1. Klicken Sie auf **Speichern**.

   ![](assets/image2014-9-15-15-3a18-3a15.png)

Und das ist es! Wenn Benutzer dieses Formular nun ausfüllen und &quot;USA für Land&quot;auswählen, wird das Feld &quot;Bundesland&quot;mit den angegebenen Optionen dynamisch angezeigt.
