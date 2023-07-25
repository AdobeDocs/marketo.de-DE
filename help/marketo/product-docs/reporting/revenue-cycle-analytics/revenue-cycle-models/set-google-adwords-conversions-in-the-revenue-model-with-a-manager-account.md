---
unique-page-id: 7504923
description: Festlegen von Google AdWords-Konversionen im Umsatzmodell mit einem Manager-Konto - Marketo Docs - Produktdokumentation
title: Festlegen von Google AdWords-Konversionen im Umsatzmodell mit einem Manager-Konto
exl-id: 8c9f50cf-0a8b-4f9a-a0bd-bb57eeac24cf
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# Festlegen von Google AdWords-Konversionen im Umsatzmodell mit einem Manager-Konto {#set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account}

Verknüpfen Sie Ihr Google AdWords-Konto mit Marketo, um Offline-Konversionsdaten automatisch von Marketo in Google AdWords hochzuladen. Anschließend können Sie in der AdWords-Benutzeroberfläche einfach sehen, welche Klicks zu qualifizierten Leads, Chancen und neuen Kunden (oder welchen Umsatzstufen Sie verfolgen möchten) geführt haben, nachdem Sie [Benutzerdefinierte Spalten hinzufügen](https://support.google.com/adwords/answer/3073556) in AdWords.

Wenn Sie über mehrere Google Adwords -Konten verfügen, können Sie eine [Google AdWords Manager-Konto](https://www.google.com/adwords/manager-accounts/) (ehemals &quot;My Client Center&quot;), um sie in Marketo zu integrieren.

Sie können AdWords-Offline-Konversionen einer oder mehreren Phasen in einem Umsatzmodell zuordnen. Es gibt zwei Möglichkeiten:

* Staging-Aktion
* AdWords-Zuordnung

>[!PREREQUISITES]
>
>[Hinzufügen von Google AdWords als Startpunktdienst mit einem Manager-Konto](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md)

## Verwenden der Staging-Aktion {#use-stage-action}

Ordnen Sie eine AdWords-Konversion unter &quot;Staging-Aktionen&quot;zu.

1. Wählen Sie den Schritt aus, den Sie einer AdWords-Konversion zuordnen möchten.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Unter dem **Staging-Aktionen** Dropdown-Liste auswählen **AdWords-Konversion festlegen**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Festlegen einer **AdWords-Konversion**.

   >[!NOTE]
   >
   >Für jedes untergeordnete Konto kann eine andere AdWords-Konversion ausgewählt werden.

   ![](assets/image2015-3-27-17-3a16-3a37.png)

   Tipp: Wenn Sie keine AdWords-Konversionen haben, erstellen Sie eine, indem Sie auf **+Neue Konversion**.

   ![](assets/image2015-3-27-17-3a18-3a58.png)

1. Klicken **Speichern**.

   ![](assets/image2015-3-27-17-3a21-3a15.png)

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

   ![](assets/image2015-3-27-17-3a23-3a13.png)

1. Geben Sie einen **Konversionsname**. Klicken **Speichern**.

   ![](assets/image2015-3-27-17-3a24-3a49.png)

   Ausgezeichnet! Diese neue Konversion wird in Ihrem AdWords-Konto angezeigt.

## Verwenden der AdWords-Zuordnung {#use-adwords-mapping}

Sie können alle Ihre Modellphasen mit Ihrer AdWords-Konversion an einem Ort mithilfe von AdWords-Zuordnungen verknüpfen.

1. Auswählen **Bearbeiten von AdWords-Zuordnungen**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Wählen Sie die gewünschte **AdWords-Konto** und gewünscht **AdWords-Konversion** für jede Phase, die Sie verfolgen möchten.

   ![](assets/image2015-3-27-17-3a30-3a15.png)

1. Nachdem Sie Ihre Bühnen zugeordnet haben, klicken Sie auf **Speichern**.

   ![](assets/image2015-3-27-17-3a30-3a48.png)

1. Nachdem Sie alle AdWords-Konversionen den Umsatzphasen zugeordnet haben, gehen Sie zurück zur Zusammenfassungsseite. Auswählen **Modellaktionen** und wählen Sie **Phasen genehmigen**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Um die Offline-Konversionsdaten anzuzeigen, müssen Sie sich bei Ihrem AdWords-Konto anmelden. Es wird empfohlen, die [Funktion &quot;Benutzerdefinierte Spalten&quot;](https://support.google.com/adwords/answer/3073556) , um Spalten zur Konversionszählung für jede Offline-Konversion zu erstellen, die Sie aus Marketo importieren.
