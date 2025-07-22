---
unique-page-id: 7504923
description: Set [!DNL Google AdWords] Conversions im Umsatzmodell mit einem Manager-Konto - Marketo-Dokumente - Produktdokumentation
title: Festlegen  [!DNL Google AdWords]  Konversionen im Umsatzmodell mit einem Manager-Konto
exl-id: 8c9f50cf-0a8b-4f9a-a0bd-bb57eeac24cf
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Festlegen [!DNL Google AdWords] Konversionen im Umsatzmodell mit einem Manager-Konto {#set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account}

Verknüpfen Sie Ihr [!DNL Google AdWords] mit Marketo, um Offline-Konversionsdaten automatisch von Marketo in [!DNL Google AdWords] hochzuladen. In der [!DNL AdWords]-Benutzeroberfläche können Sie dann leicht erkennen, welche Klicks zu qualifizierten Leads, Chancen und neuen Kunden geführt haben (oder welche Umsatzphasen Sie verfolgen möchten), nachdem Sie [benutzerdefinierte Spalten hinzufügen](https://support.google.com/adwords/answer/3073556) in [!DNL AdWords] hinzugefügt haben.

Wenn Sie über mehrere [!DNL Google Adwords] verfügen, können Sie ein [[!DNL Google AdWords] Manager-Konto](https://www.google.com/adwords/manager-accounts/) (ehemals „Mein Client-Center„) verwenden, um sie in Marketo zu integrieren.

Sie können [!DNL AdWords] Offline-Konversionen einem oder mehreren Phasen in einem Umsatzmodell zuordnen. Es gibt zwei Möglichkeiten:

* Bühnenaktion
* [!DNL AdWords]

>[!PREREQUISITES]
>
>[Add [!DNL Google AdWords] as a Launchpoint Service mit einem Manager-Konto](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md)

## Staging-Aktion verwenden {#use-stage-action}

Ordnen Sie eine [!DNL AdWords] Konversion unter Staging-Aktionen zu.

1. Wählen Sie den Schritt aus, den Sie einer [!DNL AdWords]-Konversion zuordnen möchten.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Wählen Sie in **[!UICONTROL Dropdown]** Liste „Staging-Aktionen“ die Option **[!UICONTROL AdWords-Konversion festlegen]**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Legen Sie eine **[!DNL AdWords]fest**.

   >[!NOTE]
   >
   >Für jedes untergeordnete Konto kann eine andere [!DNL AdWords] ausgewählt werden.

   ![](assets/image2015-3-27-17-3a16-3a37.png)

   Tipp: Wenn Sie noch keine [!DNL AdWords] Konversionen haben, erstellen Sie eine, indem Sie auf **[!UICONTROL +Neue Konversion klicken]**.

   ![](assets/image2015-3-27-17-3a18-3a58.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2015-3-27-17-3a21-3a15.png)

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

   ![](assets/image2015-3-27-17-3a23-3a13.png)

1. Geben Sie einen **Konversionsnamen** ein. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2015-3-27-17-3a24-3a49.png)

   Ausgezeichnet! Diese neue Konversion wird in Ihrem [!DNL AdWords]-Konto angezeigt.

## [!DNL AdWords] verwenden {#use-adwords-mapping}

Sie können alle Modellphasen mit Ihrer [!DNL AdWords]-Konversion an einem Ort verknüpfen, indem Sie [!DNL AdWords] Zuordnungen verwenden.

1. Wählen Sie **[!UICONTROL AdWords-Zuordnungen bearbeiten]** aus.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Wählen Sie für jeden Schritt **[!DNL AdWords]den Sie nachverfolgen möchten, das gewünschte** und **[!DNL AdWords]gewünschte** Conversion aus.

   ![](assets/image2015-3-27-17-3a30-3a15.png)

1. Klicken Sie nach der Zuordnung Ihrer Stadien auf **[!UICONTROL Speichern]**.

   ![](assets/image2015-3-27-17-3a30-3a48.png)

1. Wenn Sie alle Ihre [!DNL AdWords] Konversionen den Umsatzstadien zugeordnet haben, kehren Sie zur Zusammenfassungsseite zurück. Wählen Sie **[!UICONTROL Modellaktionen]** und wählen Sie **[!UICONTROL Phasen genehmigen]**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Um die Offline-Konversionsdaten anzuzeigen, müssen Sie sich bei Ihrem [!DNL AdWords]-Konto anmelden. Es wird empfohlen, die Funktion [Benutzerdefinierte Spalten](https://support.google.com/adwords/answer/3073556) zu verwenden, um für jede Offline-Konversion, die Sie aus Marketo importieren, Spalten für die Konversionsanzahl zu erstellen.
