---
unique-page-id: 6095029
description: Google AdWords-Konvertierungen im Umsatzmodell - Marketing-Dokumente - Produktdokumentation festlegen
title: Google AdWords-Konversionen im Umsatzmodell festlegen
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---


# Google AdWords-Konversionen im Umsatzmodell {#set-google-adwords-conversions-in-the-revenue-model} festlegen

Verknüpfen Sie Ihr Google AdWords-Konto mit Marketo, um automatisch Offline-Konversionsdaten von Marketing zu Google AdWords hochzuladen. In der Benutzeroberfläche von AdWords können Sie dann einfach sehen, welche Klicks zu qualifizierten Interessenten, Chancen und neuen Kunden (oder welchen Umsatzstufen Sie verfolgen möchten) führten, nachdem Sie [benutzerdefinierte Spalten](https://support.google.com/adwords/answer/3073556) in AdWords hinzugefügt haben.

>[!NOTE]
>
>Dies ist eine Push-Integration von Marketo zu Google AdWords. Umrechnungsdaten werden in Ihrem Google AdWords-Portal nur *angezeigt,** nicht in der Benutzeroberfläche von Marketing. ***

Erfahren Sie mehr über die Google Offline-Konversions-Importfunktion[.  ](https://support.google.com/adwords/answer/2998031?hl=en)  Ordnen Sie AdWords-Offline-Konvertierungen einer oder mehreren Phasen in einem Umsatzmodell zu. Es gibt drei Möglichkeiten, die Zuordnung durchzuführen:

* AdWords-Konversion
* Aktion der Stufe
* AdWords-Zuordnung

Sie können eine neue AdWords-Offlinekonversion von Marketing erstellen, wenn Sie die Option &quot;Anzeigenaktion&quot;verwenden.

>[!PREREQUISITES]
>
>* [hinzufügen von Google AdWords als LaunchPoint-Dienst](../../../../product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md)

>



## AdWords-Konversion {#use-adwords-conversion} verwenden

1. Wechseln Sie zum Bereich **Analytics**.

   ![](assets/image2015-2-23-18-3a9-3a34.png)

1. Wählen Sie ein Modell aus.

   ![](assets/image2015-2-23-18-3a3-3a12.png)

1. Klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/image2015-3-10-15-3a3-3a20.png)

1. Wählen Sie die Umsatzstufe aus, die Sie einer AdWords-Konversion zuordnen möchten.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Wählen Sie **AdWords Conversion** aus, die Sie Ihrer Marketing-Bühne zuordnen möchten.

   ![](assets/image2015-2-26-16-3a46-3a15.png)

   Schön! Ihre AdWords-Konversionsdaten werden zu dem von Ihnen gewählten Zeitpunkt in Ihre Google AdWords-Version hochgeladen.

## Aktion der Stufe {#use-stage-action} verwenden

Sie können eine AdWords-Konvertierung auch unter &quot;Stage-Aktionen&quot;zuordnen.

1. Wählen Sie den Schritt aus, den Sie einer AdWords-Konvertierung zuordnen möchten.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Wählen Sie unter der Dropdownliste **Stage Actions** die Option **AdWords Conversion** festlegen.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Wählen Sie eine **AdWords Conversion**.

   ![](assets/image2015-2-26-16-3a54-3a47.png)

   **Tipp**: Wenn Sie keine AdWords-Konvertierungen haben, erstellen Sie eine, indem Sie auf  **+Neue Konversion** klicken.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/image2015-2-26-16-3a56-3a2.png)

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

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Geben Sie einen **Umrechnungsnamen** ein. Klicken Sie auf **Speichern**.

   ![](assets/image2015-2-26-21-3a24-3a7.png)

   Ausgezeichnet! Diese neue Konversion wird in Ihrem AdWords-Konto angezeigt.

## AdWords-Zuordnung verwenden {#use-adwords-mapping}

Mit AdWords-Zuordnungen können Sie alle Modellphasen an einem Ort mit Ihrer AdWords-Konversion verknüpfen.

1. Wählen Sie **AdWords-Zuordnungen bearbeiten**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Wählen Sie die gewünschte **AdWords Conversion** für jede Phase aus, die Sie verfolgen möchten.

   ![](assets/image2015-2-26-17-3a6-3a15.png)

1. Klicken Sie nach der Zuordnung Ihrer Schritte auf **Speichern**.

   ![](assets/image2015-2-26-17-3a7-3a48.png)

1. Nachdem Sie alle AdWords-Konvertierungen den Umsatzstufen zugeordnet haben, gehen Sie zurück zur Zusammenfassungsseite. Wählen Sie **Modellaktionen** und wählen Sie **Phasen genehmigen**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Zur Ansicht der Offline-Konversionsdaten müssen Sie sich bei Ihrem AdWords-Konto anmelden. Es wird empfohlen, die Funktion [Benutzerspezifische Spalten](https://support.google.com/adwords/answer/3073556) zu verwenden, um Konversionszählungsspalten für jede Offlinekonversion zu erstellen, die Sie aus Marketing importieren.
