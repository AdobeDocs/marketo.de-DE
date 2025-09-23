---
unique-page-id: 6095029
description: Set [!DNL Google AdWords] Conversions im Umsatzmodell - Marketo-Dokumente - Produktdokumentation
title: Set [!DNL Google AdWords] Conversions im Umsatzmodell
exl-id: dd1259fc-d3f2-44ec-8055-f75d55263b36
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---

# Festlegen [!DNL Google AdWords] Konversionen im Umsatzmodell {#set-google-adwords-conversions-in-the-revenue-model}

Verknüpfen Sie Ihr [!DNL Google AdWords] mit Marketo, um Offline-Konversionsdaten automatisch von Marketo in [!DNL Google AdWords] hochzuladen. In der [!DNL AdWords]-Benutzeroberfläche können Sie dann leicht erkennen, welche Klicks zu qualifizierten Leads, Chancen und neuen Kunden geführt haben (oder welche Umsatzphasen Sie verfolgen möchten), nachdem Sie [benutzerdefinierte Spalten hinzufügen](https://support.google.com/adwords/answer/3073556) in [!DNL AdWords] hinzugefügt haben.

>[!NOTE]
>
>Hierbei handelt es sich um eine Push-Integration von Marketo in [!DNL Google AdWords]. Konversionsdaten werden _nur_ in Ihrem [!DNL Google AdWords]-Portal angezeigt, _nicht in der Marketo-_.

Google Erfahren Sie mehr über die Offline-Konversions-Importfunktion von [](https://support.google.com/adwords/answer/2998031?hl=en). Ordnen Sie [!DNL AdWords] Offline-Konversionen einem oder mehreren Phasen in einem Umsatzmodell zu. Es gibt drei Möglichkeiten für die Zuordnung:

* [!DNL AdWords]
* Bühnenaktion
* [!DNL AdWords]

Sie können eine neue [!DNL AdWords] Offline-Konversion aus Marketo erstellen, wenn Sie Staging-Aktion verwenden.

>[!PREREQUISITES]
>
>[Add [!DNL Google AdWords] as a LaunchPoint Service](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md)

## [!DNL AdWords] verwenden {#use-adwords-conversion}

1. Wechseln Sie zum Bereich **[!UICONTROL Analytics]**.

   ![](assets/image2015-2-23-18-3a9-3a34.png)

1. Modell auswählen.

   ![](assets/image2015-2-23-18-3a3-3a12.png)

1. Klicken Sie **[!UICONTROL Entwurf bearbeiten]**.

   ![](assets/image2015-3-10-15-3a3-3a20.png)

1. Wählen Sie die Umsatzstufe aus, die Sie einer [!DNL AdWords] Konversion zuordnen möchten.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Wählen Sie die **[!UICONTROL AdWords-Konversion]** aus, die Sie Ihrem Marketo-Stadium zuordnen möchten.

   ![](assets/image2015-2-26-16-3a46-3a15.png)

   Schön! Ihre [!DNL AdWords]-Konversionsdaten werden mit der von Ihnen ausgewählten Kadenz in Ihre [!DNL Google AdWords] hochgeladen.

## Staging-Aktion verwenden {#use-stage-action}

Sie können auch eine AdWords Konversion unter &quot;**[!UICONTROL &quot;]**.

1. Wählen Sie den Schritt aus, den Sie einer [!DNL AdWords]-Konversion zuordnen möchten.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Wählen Sie in **[!UICONTROL Dropdown]** Liste „Staging-Aktionen“ die Option **[!UICONTROL AdWords-Konversion festlegen]**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Wählen Sie eine **[!UICONTROL AdWords-Konversion]** aus.

   ![](assets/image2015-2-26-16-3a54-3a47.png)

   **Tipp**: Wenn Sie keine [!DNL AdWords] Konversionen haben, erstellen Sie eine, indem Sie auf **[!UICONTROL +Neue Konvertierung klicken]**.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2015-2-26-16-3a56-3a2.png)

1. Wenn Sie alle Ihre [!DNL AdWords] Konversionen den Umsatzstadien zugeordnet haben, kehren Sie zur Zusammenfassungsseite zurück. Wählen Sie **[!UICONTROL Modellaktionen]** und wählen Sie **[!UICONTROL Phasen genehmigen]**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## Profi-Tipp: Neue Konversion hinzufügen {#pro-tip-add-a-new-conversion}

Pro Tipp! Aus Marketo kann eine neue [!DNL AdWords] Offline-Konversion erstellt werden.

>[!CAUTION]
>
>Bei neuen Konversionen, die aus Marketo erstellt wurden, ist die Einstellung „Optimierung“ aktiviert. Dies bedeutet, dass [!DNL AdWords] Angebotsstrategien Ihre Angebote für diese Konversionen optimieren können. Sie können diese Einstellung in Ihrem [!DNL AdWords] ändern.

1. Wählen Sie in **[!UICONTROL Dropdown]** Liste „Staging-Aktionen“ die Option **[!UICONTROL AdWords-Konversion festlegen]**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Wählen Sie **[!UICONTROL Neue Konversion]** aus.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Geben Sie einen **[!UICONTROL Konversionsnamen]** ein. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2015-2-26-21-3a24-3a7.png)

   Ausgezeichnet! Diese neue Konversion wird in Ihrem [!DNL AdWords]-Konto angezeigt.

## [!DNL AdWords] verwenden {#use-adwords-mapping}

Sie können alle Ihre Modellphasen mit Ihrer [!UICONTROL AdWords-Konversion] über [!DNL AdWords] Mappings an einem Ort verknüpfen.

1. Wählen Sie **[!UICONTROL AdWords-Zuordnungen bearbeiten]** aus.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Wählen Sie die gewünschte **[!UICONTROL AdWords-Konversion]** für jeden Schritt aus, den Sie verfolgen möchten.

   ![](assets/image2015-2-26-17-3a6-3a15.png)

1. Klicken Sie nach der Zuordnung Ihrer Stadien auf **[!UICONTROL Speichern]**.

   ![](assets/image2015-2-26-17-3a7-3a48.png)

1. Wenn Sie alle Ihre [!DNL AdWords] Konversionen den Umsatzstadien zugeordnet haben, kehren Sie zur Zusammenfassungsseite zurück. Wählen Sie **[!UICONTROL Modellaktionen]** und wählen Sie **[!UICONTROL Phasen genehmigen]**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Um die Offline-Konversionsdaten anzuzeigen, müssen Sie sich bei Ihrem [!DNL AdWords]-Konto anmelden. Es wird empfohlen, die Funktion [Benutzerdefinierte Spalten](https://support.google.com/adwords/answer/3073556) zu verwenden, um für jede Offline-Konversion, die Sie aus Marketo importieren, Spalten für die Konversionsanzahl zu erstellen.
