---
unique-page-id: 2949962
description: Dynamisches Umschalten der Sichtbarkeit eines Formularfelds - Marketo-Dokumente - Produktdokumentation
title: Dynamisches Umschalten der Sichtbarkeit eines Formularfelds
exl-id: 51b9283d-bfa1-4535-89ba-96c0ae2ea909
feature: Forms
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 1%

---

# Dynamisches Umschalten der Sichtbarkeit eines Formularfelds {#dynamically-toggle-visibility-of-a-form-field}

>[!PREREQUISITES]
>
>* [Fügen Sie Ihrem Formular eine Länderauswahlliste hinzu](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)

Eine wirklich coole Funktion von Marketo forms ist, dass Sie Formularfelder oder [Feldsätze](/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md) dynamisch ein-/ausblenden können.

>[!NOTE]
>
>**Beispiel**
>
>In diesem Beispiel wird das Feld **Bundesland** ausgeblendet, es sei denn, **Land** ist als &quot;USA&quot;ausgewählt.

1. Wechseln Sie zu **Marketingaktivitäten**.

   ![](assets/login-marketing-activities-8.png)

1. Wählen Sie das Formular aus und klicken Sie auf **Formular bearbeiten**.

   ![](assets/editform-1.png)

1. Wählen Sie das Feld aus, das Sie dynamisch ausblenden/anzeigen möchten, und klicken Sie auf den Link für **Sichtbarkeitsregeln**.

   ![](assets/image2014-9-15-15-3a16-3a0.png)

1. Suchen und wählen Sie das Feld aus, um das Sie eine Bedingung erstellen möchten.

   ![](assets/image2014-9-15-15-3a16-3a12.png)

1. Wählen Sie den Operator aus.

   >[!TIP]
   >
   >Das ist cool, weil Sie unscharfe Übereinstimmungen wie &quot;beginnt mit&quot;wählen können.

   ![](assets/image2014-9-15-15-3a16-3a50.png)

1. Wählen Sie die Werte aus, nach denen gesucht werden soll, und klicken Sie dann außerhalb der Dropdown-Liste auf .

   ![](assets/image2014-9-15-15-3a17-3a4.png)

   >[!TIP]
   >
   >Sie können mehrere Werte auswählen, indem Sie darauf klicken, während die Dropdown-Liste geöffnet ist. Sie können beispielsweise &quot;USA&quot;und &quot;Kanada&quot;auswählen.

   >[!NOTE]
   >
   >Zuvor haben wir Land in einen Feldtyp vom Typ &quot;Auswahlliste&quot;konvertiert und [alle Länder als Werte hinzugefügt](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md).

1. Klicken Sie auf **Speichern**.

   ![](assets/image2014-9-15-15-3a18-3a15.png)

Und das ist es! Wenn Sie nun dieses Formular ausfüllen und &quot;USA für Land&quot;auswählen, wird das Feld &quot;Bundesland&quot;mit den angegebenen Optionen dynamisch angezeigt.

>[!IMPORTANT]
>
>Das Verhalten von Formularfeldern funktioniert nahtlos, wenn Feldwerte über ein benutzerdefiniertes Skript mithilfe von [API-Funktionen](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/forms-api-reference){target="_blank"} in Forms 2.0 festgelegt/aktualisiert werden.
>
>Bedingte Felder funktionieren möglicherweise nicht wie erwartet, wenn Feldwerte von anderen externen Skripten als der Forms 2.0 JavaScript API geändert werden.
