---
unique-page-id: 2949962
description: Dynamisches Umschalten der Sichtbarkeit eines Formularfelds - Marketing-Dokumente - Produktdokumentation
title: Dynamisches Umschalten zwischen Sichtbarkeit eines Formularfelds
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---


# Dynamisches Umschalten zwischen Sichtbarkeit eines Formularfelds {#dynamically-toggle-visibility-of-a-form-field}

>[!PREREQUISITES]
>
>* [hinzufügen einer Länderauswahl in Ihr Formular](../../../../product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)

>



Eine wirklich coole Funktion von Marketo Forms ist, dass Sie Formularfelder oder [Feldsätze](add-a-fieldset-to-a-form.md)dynamisch ein-/ausblenden können.

>[!NOTE]
>
>**Beispiel**
>
>In diesem Beispiel sollten wir das Feld &quot; **Bundesland** &quot;ausblenden, es sei denn, das Feld &quot; **Land** &quot;wurde als &quot;Vereinigte Staaten&quot;ausgewählt.

1. Gehen Sie zu **Marketing** - **Aktivitäten**.

   ![](assets/login-marketing-activities-8.png)

1. Wählen Sie das Formular aus und klicken Sie auf **Bearbeiten** des **Formulars**.

   ![](assets/editform-1.png)

1. Wählen Sie das Feld aus, das dynamisch ein-/ausgeblendet werden soll, und klicken Sie auf den Link für **Sichtbarkeitsregeln** ****.

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
   >Zuvor haben wir Country in einen Feldtyp mit Pick-Liste konvertiert und alle Länder als  [hinzugefügt](../../../../product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md).

1. Klicken Sie auf **Speichern**.

   ![](assets/image2014-9-15-15-3a18-3a15.png)

Und das ist es! Wenn Benutzer dieses Formular nun ausfüllen und &quot;USA für Land&quot;auswählen, wird das Feld &quot;Bundesland&quot;mit den angegebenen Optionen dynamisch angezeigt.

>[!NOTE]
>
>**Tieftauchen**
>
>Möchten Sie mehr über [Formulare](http://docs.marketo.com/display/docs/forms)erfahren?

