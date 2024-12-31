---
unique-page-id: 6095029
description: Festlegen von Google AdWords-Konversionen im Umsatzmodell - Marketo-Dokumente - Produktdokumentation
title: Festlegen von Google AdWords-Konversionen im Umsatzmodell
exl-id: dd1259fc-d3f2-44ec-8055-f75d55263b36
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 1%

---

# Festlegen von Google AdWords-Konversionen im Umsatzmodell {#set-google-adwords-conversions-in-the-revenue-model}

Verknüpfen Sie Ihr Google AdWords-Konto mit Marketo, um Offline-Konversionsdaten automatisch von Marketo in Google AdWords hochzuladen. In der AdWords-Benutzeroberfläche können Sie dann leicht erkennen, welche Klicks zu qualifizierten Leads, Chancen und neuen Kunden (oder welchen Umsatzstadien Sie nachverfolgen möchten) geführt haben, nachdem Sie in AdWords [benutzerdefinierte Spalten hinzufügen](https://support.google.com/adwords/answer/3073556) hinzugefügt haben.

>[!NOTE]
>
>Dies ist eine Push-Integration von Marketo in Google AdWords. Konversionsdaten werden _nur_ in Ihrem Google AdWords-Portal angezeigt, _nicht in der Marketo-Benutzeroberfläche_.

Google Erfahren Sie mehr über die Offline-Konversions-Importfunktion von [](https://support.google.com/adwords/answer/2998031?hl=en). Ordnen Sie Offline-Konversionen von AdWords einem oder mehreren Phasen in einem Umsatzmodell zu. Es gibt drei Möglichkeiten für die Zuordnung:

* AdWords-Conversion
* Bühnenaktion
* AdWords-Zuordnung

Sie können eine neue AdWords-Offline-Konversion aus Marketo erstellen, wenn Sie Staging-Aktion verwenden.

>[!PREREQUISITES]
>
>[Hinzufügen von Google AdWords als LaunchPoint-Service](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md)

## AdWords-Konversion verwenden {#use-adwords-conversion}

1. Wechseln Sie zum Bereich **Analytics**.

   ![](assets/image2015-2-23-18-3a9-3a34.png)

1. Modell auswählen.

   ![](assets/image2015-2-23-18-3a3-3a12.png)

1. Klicken Sie **Entwurf bearbeiten**.

   ![](assets/image2015-3-10-15-3a3-3a20.png)

1. Wählen Sie die Umsatzstufe aus, die Sie einer AdWords-Konversion zuordnen möchten.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Wählen Sie die **AdWords-Konversion** aus, die Sie Ihrem Marketo-Stadium zuordnen möchten.

   ![](assets/image2015-2-26-16-3a46-3a15.png)

   Schön! Ihre AdWords-Konversionsdaten werden mit der von Ihnen gewählten Kadenz in Ihre Google AdWords hochgeladen.

## Staging-Aktion verwenden {#use-stage-action}

Sie können auch eine AdWords-Konversion unter „Staging-Aktionen“ zuordnen.

1. Wählen Sie den Schritt aus, den Sie einer AdWords-Konversion zuordnen möchten.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Wählen Sie in **Dropdown** Liste „Staging-Aktionen“ die Option **AdWords-Konversion festlegen**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Wählen Sie eine **AdWords-Konversion** aus.

   ![](assets/image2015-2-26-16-3a54-3a47.png)

   **Tipp**: Wenn Sie noch keine AdWords-Konversionen haben, erstellen Sie eine, indem Sie auf **+Neue Konversion klicken**.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/image2015-2-26-16-3a56-3a2.png)

1. Nachdem Sie alle AdWords-Konversionen den Umsatzstadien zugeordnet haben, gehen Sie zurück zur Zusammenfassungsseite. Wählen Sie **Modellaktionen** und wählen Sie **Phasen genehmigen**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## Profi-Tipp: Neue Konversion hinzufügen {#pro-tip-add-a-new-conversion}

Pro Tipp! Aus Marketo kann eine neue AdWords-Offline-Konversion erstellt werden.

>[!CAUTION]
>
>Bei neuen Konversionen, die aus Marketo erstellt wurden, ist die Einstellung „Optimierung“ aktiviert. Dies bedeutet, dass AdWords-Bid-Strategien Ihre Angebote für diese Konversionen optimieren können. Sie können diese Einstellung über Ihr AdWords-Konto ändern.

1. Wählen Sie in **Dropdown** Liste „Staging-Aktionen“ die Option **AdWords-Konversion festlegen**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Wählen Sie **Neue Konversion** aus.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Geben Sie einen **Konversionsnamen** ein. Klicken Sie auf **Speichern**.

   ![](assets/image2015-2-26-21-3a24-3a7.png)

   Ausgezeichnet! Diese neue Konversion wird in Ihrem AdWords-Konto angezeigt.

## AdWords-Zuordnung verwenden {#use-adwords-mapping}

Mit AdWords-Mappings können Sie alle Modellphasen mit Ihrer AdWords-Konversion an einem Ort verknüpfen.

1. Wählen Sie **AdWords-Zuordnungen bearbeiten** aus.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Wählen Sie die gewünschte **AdWords-Konversion** für jeden Schritt aus, den Sie verfolgen möchten.

   ![](assets/image2015-2-26-17-3a6-3a15.png)

1. Klicken Sie nach der Zuordnung Ihrer Stadien auf **Speichern**.

   ![](assets/image2015-2-26-17-3a7-3a48.png)

1. Nachdem Sie alle AdWords-Konversionen den Umsatzstadien zugeordnet haben, gehen Sie zurück zur Zusammenfassungsseite. Wählen Sie **Modellaktionen** und wählen Sie **Phasen genehmigen**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Um die Offline-Konversionsdaten anzeigen zu können, müssen Sie sich bei Ihrem AdWords-Konto anmelden. Es wird empfohlen, die Funktion [Benutzerdefinierte Spalten](https://support.google.com/adwords/answer/3073556) zu verwenden, um für jede Offline-Konversion, die Sie aus Marketo importieren, Spalten für die Konversionsanzahl zu erstellen.
