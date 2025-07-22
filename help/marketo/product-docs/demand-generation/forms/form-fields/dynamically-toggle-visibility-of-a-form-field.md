---
unique-page-id: 2949962
description: 'Dynamisches Umschalten der Sichtbarkeit eines Formularfelds: Marketo-Dokumente - Produktdokumentation'
title: Dynamisches Umschalten der Sichtbarkeit eines Formularfelds
exl-id: 51b9283d-bfa1-4535-89ba-96c0ae2ea909
feature: Forms
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 2%

---

# Dynamisches Umschalten der Sichtbarkeit eines Formularfelds {#dynamically-toggle-visibility-of-a-form-field}

>[!PREREQUISITES]
>
>* [Fügen Sie Ihrem Formular eine Länder-Auswahlliste hinzu](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)

Eine wirklich coole Funktion von Marketo Forms ist, dass Sie Formularfelder oder [Feldsätze“ dynamisch ](/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md)/anzeigen können.

>[!NOTE]
>
>**Beispiel**
>
>Blenden wir in diesem Beispiel das Feld &quot;**&quot; aus** es sei denn **„Land** ist als „Vereinigte Staaten“ ausgewählt.

1. Navigieren Sie **[!UICONTROL Marketing-Aktivitäten]**.

   ![](assets/login-marketing-activities-8.png)

1. Wählen Sie Ihr Formular aus und klicken Sie auf **[!UICONTROL Formular bearbeiten]**.

   ![](assets/editform-1.png)

1. Wählen Sie das Feld aus, das Sie dynamisch ein- oder ausblenden möchten, und klicken Sie auf den Link für **[!UICONTROL Sichtbarkeitsregeln]**.

   ![](assets/image2014-9-15-15-3a16-3a0.png)

1. Suchen Sie das Feld, um das Sie eine Bedingung erstellen möchten, und wählen Sie es aus.

   ![](assets/image2014-9-15-15-3a16-3a12.png)

1. Wählen Sie den Operator aus.

   >[!TIP]
   >
   >Dies ist cool, weil Sie unscharfe Übereinstimmungen wie &quot;[!UICONTROL Beginnt mit“ ] können.

   ![](assets/image2014-9-15-15-3a16-3a50.png)

1. Wählen Sie die zu suchenden Werte aus und klicken Sie dann außerhalb der Dropdown-Liste.

   ![](assets/image2014-9-15-15-3a17-3a4.png)

   >[!TIP]
   >
   >Sie können mehrere Werte auswählen, indem Sie darauf klicken, während die Dropdown-Liste geöffnet ist. Sie können beispielsweise auf Vereinigte Staaten und Kanada klicken.

   >[!NOTE]
   >
   >Wir haben „Land“ zuvor in einen Auswahllisten-Feldtyp konvertiert und [alle Länder als Werte hinzugefügt](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md).

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2014-9-15-15-3a18-3a15.png)

Und das war&#39;s! Wenn Personen dieses Formular ausfüllen und „USA für Land“ auswählen, wird das Feld „Bundesstaat“ dynamisch mit den angegebenen Auswahlmöglichkeiten angezeigt.

>[!IMPORTANT]
>
>Das Verhalten von Formularfeldern funktioniert nahtlos, wenn Feldwerte mithilfe von benutzerdefinierten Skripten (API[Funktionen) in Forms 2.0 ](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/forms-api-reference){target="_blank"}/aktualisiert werden.
>
>Bedingte Felder funktionieren möglicherweise nicht wie erwartet, wenn Feldwerte durch andere externe Skripte als die Forms 2.0 JavaScript-API geändert werden.
