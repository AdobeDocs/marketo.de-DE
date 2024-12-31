---
unique-page-id: 7504923
description: Festlegen von Google AdWords-Konversionen im Umsatzmodell mit einem Managerkonto - Marketo-Dokumente - Produktdokumentation
title: Festlegen von Google AdWords-Konversionen im Umsatzmodell mit einem Manager-Konto
exl-id: 8c9f50cf-0a8b-4f9a-a0bd-bb57eeac24cf
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 0%

---

# Festlegen von Google AdWords-Konversionen im Umsatzmodell mit einem Manager-Konto {#set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account}

Verknüpfen Sie Ihr Google AdWords-Konto mit Marketo, um Offline-Konversionsdaten automatisch von Marketo in Google AdWords hochzuladen. In der AdWords-Benutzeroberfläche können Sie dann leicht erkennen, welche Klicks zu qualifizierten Leads, Chancen und neuen Kunden (oder welchen Umsatzstadien Sie nachverfolgen möchten) geführt haben, nachdem Sie in AdWords [benutzerdefinierte Spalten hinzufügen](https://support.google.com/adwords/answer/3073556) hinzugefügt haben.

Wenn Sie über mehrere Google AdWords-Konten verfügen, können Sie ein [Google AdWords Manager-Konto](https://www.google.com/adwords/manager-accounts/) (ehemals „Mein Client-Center„) verwenden, um sie in Marketo zu integrieren.

Sie können Offline-Konversionen von AdWords einem oder mehreren Phasen in einem Umsatzmodell zuordnen. Es gibt zwei Möglichkeiten:

* Bühnenaktion
* AdWords-Zuordnung

>[!PREREQUISITES]
>
>[Fügen Sie Google AdWords als Launchpoint-Service mit einem Manager-Konto hinzu](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md)

## Staging-Aktion verwenden {#use-stage-action}

Ordnen Sie eine AdWords-Konversion unter Staging-Aktionen zu.

1. Wählen Sie den Schritt aus, den Sie einer AdWords-Konversion zuordnen möchten.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Wählen Sie in **Dropdown** Liste „Staging-Aktionen“ die Option **AdWords-Konversion festlegen**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Legen Sie eine **AdWords-Konversion** fest.

   >[!NOTE]
   >
   >Für jedes untergeordnete Konto kann eine andere AdWords-Konversion ausgewählt werden.

   ![](assets/image2015-3-27-17-3a16-3a37.png)

   Tipp: Wenn Sie noch keine AdWords-Konversionen haben, erstellen Sie eine, indem Sie auf **+Neue Konversion klicken**.

   ![](assets/image2015-3-27-17-3a18-3a58.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/image2015-3-27-17-3a21-3a15.png)

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

   ![](assets/image2015-3-27-17-3a23-3a13.png)

1. Geben Sie einen **Konversionsnamen** ein. Klicken Sie auf **Speichern**.

   ![](assets/image2015-3-27-17-3a24-3a49.png)

   Ausgezeichnet! Diese neue Konversion wird in Ihrem AdWords-Konto angezeigt.

## AdWords-Zuordnung verwenden {#use-adwords-mapping}

Mit AdWords-Mappings können Sie alle Modellphasen mit Ihrer AdWords-Konversion an einem Ort verknüpfen.

1. Wählen Sie **AdWords-Zuordnungen bearbeiten** aus.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Wählen Sie für jeden Schritt **den Sie nachverfolgen möchten, das gewünschte** AdWords-Konto **und die gewünschte „AdWords-Konversion** aus.

   ![](assets/image2015-3-27-17-3a30-3a15.png)

1. Klicken Sie nach der Zuordnung Ihrer Stadien auf **Speichern**.

   ![](assets/image2015-3-27-17-3a30-3a48.png)

1. Nachdem Sie alle AdWords-Konversionen den Umsatzstadien zugeordnet haben, gehen Sie zurück zur Zusammenfassungsseite. Wählen Sie **Modellaktionen** und wählen Sie **Phasen genehmigen**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Um die Offline-Konversionsdaten anzeigen zu können, müssen Sie sich bei Ihrem AdWords-Konto anmelden. Es wird empfohlen, die Funktion [Benutzerdefinierte Spalten](https://support.google.com/adwords/answer/3073556) zu verwenden, um für jede Offline-Konversion, die Sie aus Marketo importieren, Spalten für die Konversionsanzahl zu erstellen.
