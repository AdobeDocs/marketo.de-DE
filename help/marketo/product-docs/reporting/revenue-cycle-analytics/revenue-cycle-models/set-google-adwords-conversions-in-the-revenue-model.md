---
unique-page-id: 6095029
description: Festlegen von Google AdWords-Konversionen im Umsatzmodell - Marketo Docs - Produktdokumentation
title: Festlegen von Google AdWords-Konversionen im Umsatzmodell
exl-id: dd1259fc-d3f2-44ec-8055-f75d55263b36
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---

# Festlegen von Google AdWords-Konversionen im Umsatzmodell {#set-google-adwords-conversions-in-the-revenue-model}

Verknüpfen Sie Ihr Google AdWords-Konto mit Marketo, um Offline-Konversionsdaten automatisch von Marketo in Google AdWords hochzuladen. Anschließend können Sie in der AdWords-Benutzeroberfläche einfach sehen, welche Klicks zu qualifizierten Leads, Chancen und neuen Kunden (oder welchen Umsatzstufen Sie verfolgen möchten) geführt haben, nachdem Sie [Benutzerdefinierte Spalten hinzufügen](https://support.google.com/adwords/answer/3073556) in AdWords.

>[!NOTE]
>
>Dies ist eine Push-Integration von Marketo in Google AdWords. Konversionsdaten werden angezeigt _only_ in Ihrem Google AdWords-Portal, _nicht in der Marketo-Benutzeroberfläche_.

Weitere Informationen [Google-Funktion zum Offline-Konversionsimport](https://support.google.com/adwords/answer/2998031?hl=en). Ordnen Sie AdWords-Offline-Konversionen einer oder mehreren Phasen in einem Umsatzmodell zu. Es gibt drei Möglichkeiten, die Zuordnung vorzunehmen:

* AdWords-Conversion
* Staging-Aktion
* AdWords-Zuordnung

Sie können eine neue AdWords-Offline-Konversion aus Marketo erstellen, wenn Sie die Staging-Aktion verwenden.

>[!PREREQUISITES]
>
>[Hinzufügen von Google AdWords als LaunchPoint-Dienst](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md)

## Verwenden der AdWords-Konversion {#use-adwords-conversion}

1. Navigieren Sie zu **Analytics** Bereich.

   ![](assets/image2015-2-23-18-3a9-3a34.png)

1. Wählen Sie ein Modell aus.

   ![](assets/image2015-2-23-18-3a3-3a12.png)

1. Klicken **Entwurf bearbeiten**.

   ![](assets/image2015-3-10-15-3a3-3a20.png)

1. Wählen Sie die Umsatzstufe aus, die Sie einer AdWords-Konversion zuordnen möchten.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Wählen Sie die **AdWords-Konversion** Sie möchten Ihrer Marketo-Bühne zuordnen.

   ![](assets/image2015-2-26-16-3a46-3a15.png)

   Gut! Ihre AdWords-Konversionsdaten werden zu dem von Ihnen ausgewählten Zeitpunkt in Ihre Google AdWords hochgeladen.

## Verwenden der Staging-Aktion {#use-stage-action}

Sie können eine AdWords-Konversion auch unter &quot;Staging-Aktionen&quot;zuordnen.

1. Wählen Sie den Schritt aus, den Sie einer AdWords-Konversion zuordnen möchten.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Unter dem **Staging-Aktionen** Dropdown-Liste auswählen **AdWords-Konversion festlegen**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Wählen Sie eine **AdWords-Konversion**.

   ![](assets/image2015-2-26-16-3a54-3a47.png)

   **Tipp**: Wenn Sie keine AdWords-Konversionen haben, erstellen Sie eine, indem Sie auf **+Neue Konversion**.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Klicken **Speichern**.

   ![](assets/image2015-2-26-16-3a56-3a2.png)

1. Nachdem Sie alle AdWords-Konversionen den Umsatzphasen zugeordnet haben, gehen Sie zurück zur Zusammenfassungsseite. Auswählen **Modellaktionen** und wählen Sie **Phasen genehmigen**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## Professioneller Tipp: Neue Konversion hinzufügen {#pro-tip-add-a-new-conversion}

Pro Tipp! Eine neue AdWords-Offline-Konversion kann über Marketo erstellt werden.

>[!CAUTION]
>
>Bei neuen Konversionen, die aus Marketo erstellt wurden, ist die Einstellung &quot;Optimierung&quot;aktiviert. Das bedeutet, dass AdWords-Angebotsstrategien Ihre Angebote für diese Konversionen optimieren können. Sie können diese Einstellung in Ihrem AdWords-Konto ändern.

1. Unter dem **Staging-Aktionen** Dropdown-Liste auswählen **AdWords-Konversion festlegen**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Auswählen **Neue Konversion**.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Geben Sie einen **Konversionsname**. Klicken **Speichern**.

   ![](assets/image2015-2-26-21-3a24-3a7.png)

   Ausgezeichnet! Diese neue Konversion wird in Ihrem AdWords-Konto angezeigt.

## Verwenden der AdWords-Zuordnung {#use-adwords-mapping}

Sie können alle Ihre Modellphasen mit Ihrer AdWords-Konversion an einem Ort mithilfe von AdWords-Zuordnungen verknüpfen.

1. Auswählen **Bearbeiten von AdWords-Zuordnungen**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Wählen Sie die gewünschte **AdWords-Konversion** für jede Phase, die Sie verfolgen möchten.

   ![](assets/image2015-2-26-17-3a6-3a15.png)

1. Nachdem Sie Ihre Bühnen zugeordnet haben, klicken Sie auf **Speichern**.

   ![](assets/image2015-2-26-17-3a7-3a48.png)

1. Nachdem Sie alle AdWords-Konversionen den Umsatzphasen zugeordnet haben, gehen Sie zurück zur Zusammenfassungsseite. Auswählen **Modellaktionen** und wählen Sie **Phasen genehmigen**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Um die Offline-Konversionsdaten anzuzeigen, müssen Sie sich bei Ihrem AdWords-Konto anmelden. Es wird empfohlen, die [Funktion &quot;Benutzerdefinierte Spalten&quot;](https://support.google.com/adwords/answer/3073556) , um Spalten zur Konversionszählung für jede Offline-Konversion zu erstellen, die Sie aus Marketo importieren.
