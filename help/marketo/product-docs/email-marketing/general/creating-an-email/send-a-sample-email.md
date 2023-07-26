---
unique-page-id: 1147352
description: Beispiel-E-Mail senden - Marketo-Dokumente - Produktdokumentation
title: Senden einer Beispiel-E-Mail
exl-id: b8f845e8-5c5e-463d-9d60-9c8103cec5ac
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---

# Senden einer Beispiel-E-Mail {#send-a-sample-email}

Es ist schnell und einfach, Muster einer E-Mail zu senden. Informationen zum Senden einer E-Mail mit dynamischen Inhalten finden Sie unter [Vorschau einer E-Mail mit dynamischem Inhalt](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/preview-an-email-with-dynamic-content.md).

>[!NOTE]
>
>Sie müssen über die **Auf Datenbank zugreifen - Ausführen von Einzelflussaktionen** Berechtigung zum Senden von Beispiel-E-Mails.

## Senden einer Beispiel-E-Mail {#send-a-sample-email-1}

1. Suchen und wählen Sie Ihre E-Mail aus. Klicken Sie auf **E-Mail-Aktionen** und wählen Sie **Beispiel senden**.\
   ![](assets/one-281-29.jpg)

   >[!NOTE]
   >
   >Meine Token werden in den für das E-Mail-Programm geeigneten Wert aufgelöst.

1. Geben Sie eine oder mehrere E-Mail-Adressen für den Versand ein. Trennen Sie mehrere E-Mail-Adressen durch Kommas. Klicks **Senden** wann geschehen.

   ![](assets/two.png)

   >[!IMPORTANT]
   >
   >Wenn Sie mehrere E-Mail-Adressen eingeben, sind alle für jeden Empfänger sichtbar. Der erste angegebene Empfänger ist der Hauptempfänger und jede nachfolgende E-Mail-Adresse ist ein CC-Empfänger.

   >[!TIP]
   >
   >Wenn Sie Token als bestimmte Person auflösen möchten, wählen Sie diese Person in der **Personen-Dropdown** in Schritt 2.

## Beispiel-E-Mail bei Bearbeitung senden {#send-a-sample-email-while-editing}

1. Suchen Sie Ihre E-Mail, wählen Sie sie aus und klicken Sie auf **Entwurf bearbeiten** Registerkarte.

   ![](assets/three-281-29.jpg)

1. Klicks **E-Mail-Aktionen** auswählen **Beispiel senden**.

   ![](assets/four.png)

1. Geben Sie eine E-Mail-Adresse für den Versand ein und klicken Sie auf **Senden**.

   ![](assets/two.png)

   >[!NOTE]
   >
   >Das Feld Trigger gilt nur für Benutzer, die [email, Skript](https://developers.marketo.com/documentation/velocity-script/).

## Senden einer Beispiel-E-Mail anhand eines Segments {#send-a-sample-email-based-on-a-segment}

>[!PREREQUISITES]
>
>[Anwenden der Segmentierung auf Ihre E-Mail](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/using-dynamic-content-in-an-email.md).

1. Suchen Sie Ihre E-Mail, wählen Sie sie aus und klicken Sie auf **Entwurf bearbeiten** Registerkarte.

   ![](assets/three-281-29.jpg)

1. Klicks **Vorschau**.

   ![](assets/1.png)

1. Klicken Sie auf **Anzeigen nach** und wählen Sie **Segmentierung**.

   ![](assets/2.png)

1. Eine Dropdown-Liste mit verfügbaren Segmenten wird angezeigt. Klicken Sie darauf und wählen Sie die gewünschte aus.

   ![](assets/3.png)

1. Verwenden Sie die Pfeile, um durch Ihre Optionen zu scrollen (in diesem Fall haben wir die Betreffzeile dynamisch geändert).

   ![](assets/4.png)

1. Klicks **Beispiel senden** , um eine Test-E-Mail Ihres Segments zu erhalten.

   ![](assets/5.png)

   >[!TIP]
   >
   >Im Bearbeitungsmodus Ihrer E-Mail können Sie auch eine auf einem Segment basierende Beispiel-E-Mail senden. Klicken Sie auf **E-Mail-Aktionen** Dropdown-Liste auswählen **Beispiel senden** und wählen Sie dann Ihr Segment aus.

Es ist sehr wichtig, Ihre Inhalte vor dem Start einer Kampagne zu evaluieren. Mess zweimal, schneide mal!
