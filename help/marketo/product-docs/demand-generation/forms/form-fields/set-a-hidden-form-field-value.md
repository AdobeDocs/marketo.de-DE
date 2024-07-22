---
unique-page-id: 2359663
description: Festlegen eines Werts für ein ausgeblendetes Formularfeld - Marketo Docs - Produktdokumentation
title: Festlegen eines Werts für ein ausgeblendetes Formularfeld
exl-id: acec7de1-8567-42c0-a6ce-a91b0bf69f41
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 2%

---

# Festlegen eines Werts für ein ausgeblendetes Formularfeld {#set-a-hidden-form-field-value}

Ausgeblendete Felder werden normalerweise dynamisch ausgefüllt. Sie werden der Person, die das Formular ausfüllt, nicht angezeigt. So legen Sie den Wert fest.

>[!PREREQUISITES]
>
>[ Festlegen eines Formularfelds als ausgeblendet](/help/marketo/product-docs/demand-generation/forms/form-fields/set-a-form-field-as-hidden.md)

## Feld auswählen {#select-the-field}

1. Wählen Sie in Ihrem Formular das ausgeblendete Feld aus und klicken Sie auf **Bearbeiten** für **Autofill**.

   ![](assets/autofill.png)

## Standardwert verwenden {#use-default-value}

Durch die Auswahl von &quot;Use Default Value&quot;können Sie einen bestimmten Wert hartcodieren, der beim Senden dieses Formulars immer verwendet werden soll. Geben Sie den Standardwert ein und klicken Sie auf Speichern.

![](assets/image2014-9-15-13-3a5-3a27.png)

## URL-Parameter {#url-parameter}

Wenn Sie URL-Parameter (Abfragezeichenfolgen) von der Seite erfassen möchten, auf der sich die Person beim Ausfüllen des Formulars befindet, können Sie **URL-Parameter** verwenden, um Ihr ausgeblendetes Feld zu füllen.

>[!NOTE]
>
>Parameter sind eine Art Techie, nicht wahr? Wenn man sie erst einmal bekommt, sind sie mächtig. Diese [Wikipedia-Seite auf Abfragezeichenfolgen](https://en.wikipedia.org/wiki/Query_string) ist ein wenig hilfreich.

1. Wählen Sie **URL-Parameter** für **Werttyp abrufen** aus.

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. Geben Sie den **Parameternamen** ein und klicken Sie auf **Speichern**.

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>Sie können einen Standardwert eingeben, falls der URL-Parameter nicht gefunden wird.

## Cookie-Wert {#cookie-value}

Wenn Sie Daten in Cookies speichern, können Sie **Cookie-Wert** verwenden, um Daten beim Senden des Formulars abzurufen.

1. Wählen Sie **Cookie-Wert** für **Wert abrufen von** aus.

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. Geben Sie den gewünschten Cookie-Parameternamen ein und klicken Sie auf **Speichern**.

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >Sie können einen Standardwert eingeben, falls der Parameter/das Cookie nicht gefunden wird.

## Verweis-Parameter {#referrer-parameter}

Wenn Sie Daten von der Seite erfassen möchten, von der der Besucher vor dem Ausfüllen des Formulars kam, können Sie den Parameter **Referrer** verwenden.

1. Setzen Sie **Wert abrufen von** auf **Referrer-Parameter**.

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. Geben Sie den **Parameternamen** ein, den Sie aus der Referrer-URL entfernen möchten, und klicken Sie auf **Speichern**.

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >Sie können einen **Standardwert** eingeben, falls der Referrer-Parameter nicht gefunden wird.

1. Klicken Sie auf **Beenden**.

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. Klicken Sie auf **Genehmigen und schließen**.

   ![](assets/image2014-9-15-13-3a10-3a43.png)
