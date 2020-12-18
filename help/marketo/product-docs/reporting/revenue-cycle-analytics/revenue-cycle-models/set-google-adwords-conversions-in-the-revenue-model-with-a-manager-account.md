---
unique-page-id: 7504923
description: Google AdWords-Konvertierungen im Umsatzmodell mit einem Manager-Konto - Marketing Docs - Produktdokumentation festlegen
title: Google AdWords-Konversionen im Umsatzmodell mit einem Manager-Konto festlegen
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---


# Google AdWords-Konversionen im Umsatzmodell mit einem Manager-Konto {#set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account} festlegen

Verknüpfen Sie Ihr Google AdWords-Konto mit Marketo, um automatisch Offline-Konversionsdaten von Marketing zu Google AdWords hochzuladen. In der Benutzeroberfläche von AdWords können Sie dann einfach sehen, welche Klicks zu qualifizierten Interessenten, Chancen und neuen Kunden (oder welchen Umsatzstufen Sie verfolgen möchten) führten, nachdem Sie [benutzerdefinierte Spalten](https://support.google.com/adwords/answer/3073556) in AdWords hinzugefügt haben.

Wenn Sie über mehrere Google Adwords-Konten verfügen, können Sie ein [Google AdWords Manager-Konto](https://www.google.com/adwords/manager-accounts/) (früher &quot;Mein Client-Center&quot;genannt) verwenden, um diese in Marketing zu integrieren.

Sie können AdWords-Offline-Konvertierungen einer oder mehreren Phasen in einem Umsatzmodell zuordnen. Es gibt zwei Möglichkeiten:

* Aktion der Stufe
* AdWords-Zuordnung

>[!PREREQUISITES]
>
>* [hinzufügen von Google AdWords als Startpunktdienst mit einem Managerkonto](../../../../product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md)

>



## Aktion der Stufe {#use-stage-action} verwenden

Ordnen Sie eine AdWords-Konversion unter &quot;Stage-Aktionen&quot;zu.

1. Wählen Sie den Schritt aus, den Sie einer AdWords-Konvertierung zuordnen möchten.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Wählen Sie unter der Dropdownliste **Stage Actions** die Option **AdWords Conversion** festlegen.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Legen Sie eine **AdWords-Konversion** fest.

   >[!NOTE]
   >
   >Für jedes untergeordnete Konto kann eine andere AdWords-Konversion ausgewählt werden.

   ![](assets/image2015-3-27-17-3a16-3a37.png)

   Tipp: Wenn Sie keine AdWords-Konvertierungen haben, erstellen Sie eine, indem Sie auf **+Neue Konversion** klicken.

   ![](assets/image2015-3-27-17-3a18-3a58.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/image2015-3-27-17-3a21-3a15.png)

1. Nachdem Sie alle AdWords-Konvertierungen den Umsatzstufen zugeordnet haben, gehen Sie zurück zur Zusammenfassungsseite. Wählen Sie **Modellaktionen** und wählen Sie **Phasen genehmigen**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## Pro Tipp: hinzufügen einer neuen Konversion {#pro-tip-add-a-new-conversion}

Pro Tipp! Eine neue AdWords-Offline-Konversion kann von Marketing erstellt werden.

>[!CAUTION]
>
>Bei neuen Konvertierungen, die von Marketing erstellt wurden, ist die Einstellung &quot;Optimierung&quot;aktiviert. Das bedeutet, dass AdWords-Angebotsstrategien Ihre Angebote für diese Konversionen optimieren können. Sie können diese Einstellung in Ihrem AdWords-Konto ändern.

1. Wählen Sie unter der Dropdownliste **Stage Actions** die Option **AdWords Conversion** festlegen.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Wählen Sie **Neue Konversion**.

   ** ![](assets/image2015-3-27-17-3a23-3a13.png)

   **

1. Geben Sie einen **Umrechnungsnamen** ein. Klicken Sie auf **Speichern**.

   ![](assets/image2015-3-27-17-3a24-3a49.png)

   Ausgezeichnet! Diese neue Konversion wird in Ihrem AdWords-Konto angezeigt.

## AdWords-Zuordnung verwenden {#use-adwords-mapping}

Mit AdWords-Zuordnungen können Sie alle Modellphasen an einem Ort mit Ihrer AdWords-Konversion verknüpfen.

1. Wählen Sie **AdWords-Zuordnungen bearbeiten**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Wählen Sie das gewünschte **AdWords-Konto** aus und wünschen Sie **AdWords Conversion** für jede Phase, die Sie verfolgen möchten.

   ![](assets/image2015-3-27-17-3a30-3a15.png)

1. Klicken Sie nach der Zuordnung Ihrer Schritte auf **Speichern**.

   ![](assets/image2015-3-27-17-3a30-3a48.png)

1. Nachdem Sie alle AdWords-Konvertierungen den Umsatzstufen zugeordnet haben, gehen Sie zurück zur Zusammenfassungsseite. Wählen Sie **Modellaktionen** und wählen Sie **Phasen genehmigen**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Zur Ansicht der Offline-Konversionsdaten müssen Sie sich bei Ihrem AdWords-Konto anmelden. Es wird empfohlen, die Funktion [Benutzerspezifische Spalten](https://support.google.com/adwords/answer/3073556) zu verwenden, um Konversionszählungsspalten für jede Offlinekonversion zu erstellen, die Sie aus Marketing importieren.
