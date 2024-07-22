---
unique-page-id: 6095029
description: Festlegen von Google AdWords-Konversionen im Umsatzmodell - Marketo Docs - Produktdokumentation
title: Festlegen von Google AdWords-Konversionen im Umsatzmodell
exl-id: dd1259fc-d3f2-44ec-8055-f75d55263b36
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 1%

---

# Festlegen von Google AdWords-Konversionen im Umsatzmodell {#set-google-adwords-conversions-in-the-revenue-model}

Verknüpfen Sie Ihr Google AdWords-Konto mit Marketo, um Offline-Konversionsdaten automatisch von Marketo in Google AdWords hochzuladen. Anschließend können Sie in der AdWords-Benutzeroberfläche einfach sehen, welche Klicks zu qualifizierten Leads, Chancen und neuen Kunden (oder welchen Umsatzstufen Sie verfolgen möchten) führten, nachdem Sie [benutzerdefinierte Spalten hinzufügen](https://support.google.com/adwords/answer/3073556) in AdWords hinzugefügt haben.

>[!NOTE]
>
>Dies ist eine Push-Integration von Marketo in Google AdWords. Konversionsdaten werden _nur_ in Ihrem Google AdWords-Portal angezeigt, _nicht in der Marketo-Benutzeroberfläche_.

Erfahren Sie mehr über die Funktion von [Google für den Offline-Konversionsimport](https://support.google.com/adwords/answer/2998031?hl=en). Ordnen Sie AdWords-Offline-Konversionen einer oder mehreren Phasen in einem Umsatzmodell zu. Es gibt drei Möglichkeiten, die Zuordnung vorzunehmen:

* AdWords-Conversion
* Staging-Aktion
* AdWords-Zuordnung

Sie können eine neue AdWords-Offline-Konversion aus Marketo erstellen, wenn Sie die Staging-Aktion verwenden.

>[!PREREQUISITES]
>
>[Hinzufügen von Google AdWords als LaunchPoint-Dienst](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md)

## Verwenden der AdWords-Konversion {#use-adwords-conversion}

1. Wechseln Sie zum Bereich **Analytics** .

   ![](assets/image2015-2-23-18-3a9-3a34.png)

1. Wählen Sie ein Modell aus.

   ![](assets/image2015-2-23-18-3a3-3a12.png)

1. Klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/image2015-3-10-15-3a3-3a20.png)

1. Wählen Sie die Umsatzstufe aus, die Sie einer AdWords-Konversion zuordnen möchten.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Wählen Sie die **AdWords Conversion** aus, die Sie Ihrer Marketo-Bühne zuordnen möchten.

   ![](assets/image2015-2-26-16-3a46-3a15.png)

   Gut! Ihre AdWords-Konversionsdaten werden zu dem von Ihnen ausgewählten Zeitpunkt in Ihre Google AdWords hochgeladen.

## Verwenden der Staging-Aktion {#use-stage-action}

Sie können eine AdWords-Konversion auch unter &quot;Staging-Aktionen&quot;zuordnen.

1. Wählen Sie den Schritt aus, den Sie einer AdWords-Konversion zuordnen möchten.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Wählen Sie unter der Dropdown-Liste **Staging-Aktionen** die Option **AdWords-Konversion festlegen** aus.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Wählen Sie eine **AdWords-Konversion** aus.

   ![](assets/image2015-2-26-16-3a54-3a47.png)

   **Tipp**: Wenn Sie keine AdWords-Konversionen haben, erstellen Sie eine, indem Sie auf **+Neue Konversion** klicken.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/image2015-2-26-16-3a56-3a2.png)

1. Nachdem Sie alle AdWords-Konversionen den Umsatzphasen zugeordnet haben, gehen Sie zurück zur Zusammenfassungsseite. Wählen Sie **Modellaktionen** und dann **Phasen genehmigen** aus.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## Pro Tipp: Neue Konversion hinzufügen {#pro-tip-add-a-new-conversion}

Pro Tipp! Eine neue AdWords-Offline-Konversion kann über Marketo erstellt werden.

>[!CAUTION]
>
>Bei neuen Konversionen, die aus Marketo erstellt wurden, ist die Einstellung &quot;Optimierung&quot;aktiviert. Das bedeutet, dass AdWords-Angebotsstrategien Ihre Angebote für diese Konversionen optimieren können. Sie können diese Einstellung in Ihrem AdWords-Konto ändern.

1. Wählen Sie unter der Dropdown-Liste **Staging-Aktionen** die Option **AdWords-Konversion festlegen** aus.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Wählen Sie **Neue Konversion** aus.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Geben Sie einen **Konversionsnamen** ein. Klicken Sie auf **Speichern**.

   ![](assets/image2015-2-26-21-3a24-3a7.png)

   Ausgezeichnet! Diese neue Konversion wird in Ihrem AdWords-Konto angezeigt.

## Verwenden der AdWords-Zuordnung {#use-adwords-mapping}

Sie können alle Ihre Modellphasen mit Ihrer AdWords-Konversion an einem Ort mithilfe von AdWords-Zuordnungen verknüpfen.

1. Wählen Sie **AdWords-Zuordnungen bearbeiten** aus.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Wählen Sie die gewünschte **AdWords Conversion** für jede Phase aus, die Sie verfolgen möchten.

   ![](assets/image2015-2-26-17-3a6-3a15.png)

1. Nachdem Sie Ihre Bühnen zugeordnet haben, klicken Sie auf **Speichern**.

   ![](assets/image2015-2-26-17-3a7-3a48.png)

1. Nachdem Sie alle AdWords-Konversionen den Umsatzphasen zugeordnet haben, gehen Sie zurück zur Zusammenfassungsseite. Wählen Sie **Modellaktionen** und dann **Phasen genehmigen** aus.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Um die Offline-Konversionsdaten anzuzeigen, müssen Sie sich bei Ihrem AdWords-Konto anmelden. Es wird empfohlen, die Funktion [Benutzerdefinierte Spalten](https://support.google.com/adwords/answer/3073556) zu verwenden, um Konversionszählungsspalten für jede Offline-Konversion zu erstellen, die Sie aus Marketo importieren.
