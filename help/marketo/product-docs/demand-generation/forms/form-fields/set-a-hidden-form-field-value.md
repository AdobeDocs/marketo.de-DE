---
unique-page-id: 2359663
description: Festlegen eines ausgeblendeten Formularfeldwerts - Marketo-Dokumente - Produktdokumentation
title: Festlegen eines Werts für ein ausgeblendetes Formularfeld
exl-id: acec7de1-8567-42c0-a6ce-a91b0bf69f41
feature: Forms
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 7%

---

# Festlegen eines Werts für ein ausgeblendetes Formularfeld {#set-a-hidden-form-field-value}

Ausgeblendete Felder werden in der Regel dynamisch ausgefüllt. Sie werden der Person, die das Formular ausfüllt, nicht angezeigt. So legen Sie den Wert fest.

>[!PREREQUISITES]
>
>[Formularfeld als ausgeblendet festlegen](/help/marketo/product-docs/demand-generation/forms/form-fields/set-a-form-field-as-hidden.md)

## Feld auswählen {#select-the-field}

1. Wählen Sie im Formular das ausgeblendete Feld aus und klicken Sie auf **[!UICONTROL Bearbeiten]** für **[!UICONTROL automatisches Ausfüllen]**.

   ![](assets/autofill.png)

## Standardwert verwenden {#use-default-value}

Durch Auswahl von **[!UICONTROL Standardwert]** können Sie einen bestimmten Wert hartcodieren, der beim Übermitteln dieses Formulars immer verwendet werden soll. Geben Sie den **[!UICONTROL Standardwert“ ein]** klicken Sie auf **[!UICONTROL Speichern]**.

![](assets/image2014-9-15-13-3a5-3a27.png)

## URL Parameter {#url-parameter}

Wenn Sie URL-Parameter (Abfragezeichenfolgen) von der Seite erfassen möchten, auf der sich die Person beim Ausfüllen des Formulars befindet, können Sie **[!UICONTROL URL-Parameter]** verwenden, um Ihr ausgeblendetes Feld auszufüllen.

>[!NOTE]
>
>Parameter sind irgendwie technisch, oder? Sobald man sie aber hat, sind sie mächtig. Diese [Wikipedia-Seite über Abfragezeichenfolgen](https://en.wikipedia.org/wiki/Query_string) ist einigermaßen hilfreich.

1. Wählen Sie **[!UICONTROL URL]** Parameter für **[!UICONTROL Werttyp abrufen]**.

   ![](assets/image2014-9-15-13-3a6-3a48.png)

1. Geben Sie den **[!UICONTROL Parameternamen]** ein und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2014-9-15-13-3a7-3a35.png)

>[!TIP]
>
>Sie können einen **[!UICONTROL Standardwert“ eingeben]** falls der URL-Parameter nicht gefunden wird.

## Cookie-Wert {#cookie-value}

Wenn Sie Daten in Cookies speichern, können Sie **[!UICONTROL Cookie-Wert]** verwenden, um Daten beim Senden des Formulars aufzunehmen.

1. Wählen Sie **[!UICONTROL Cookie-Wert]** für **[!UICONTROL Wert abrufen von]**.

   ![](assets/image2014-9-15-13-3a8-3a21.png)

1. Geben Sie das **[!UICONTROL Cookie (Parametername]** ein und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2014-9-15-13-3a8-3a43.png)

   >[!TIP]
   >
   >Sie können einen **[!UICONTROL Standardwert“ eingeben]** falls der Parameter/das Cookie nicht gefunden wird.

## Verweis-Parameter {#referrer-parameter}

Wenn Sie Daten von der Seite erfassen möchten, von der der Besucher kam, bevor Sie das Formular ausfüllen, können Sie **[!UICONTROL Referrer-Parameter]** verwenden.

1. Setzen Sie **[!UICONTROL Wert abrufen von]** auf **[!UICONTROL Referrer-Parameter]**.

   ![](assets/image2014-9-15-13-3a9-3a31.png)

1. Geben Sie den **[!UICONTROL Parameternamen]** ein, den Sie aus der Referrer-URL entfernen möchten, und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2014-9-15-13-3a9-3a56.png)

   >[!TIP]
   >
   >Sie können einen **[!UICONTROL Standardwert“ eingeben]** falls der Referrer-Parameter nicht gefunden wird.

1. Klicken Sie auf **[!UICONTROL Fertigstellen]**.

   ![](assets/image2014-9-15-13-3a10-3a26.png)

1. Klicken Sie **[!UICONTROL Genehmigen und schließen]**.

   ![](assets/image2014-9-15-13-3a10-3a43.png)
