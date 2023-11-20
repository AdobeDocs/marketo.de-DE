---
unique-page-id: 4719302
description: Benutzerdefinierte Objektsynchronisierung für Nicht-Englisch aktivieren - Marketo-Dokumente - Produktdokumentation
title: Aktivieren der nicht englischsprachigen benutzerdefinierten Objektsynchronisierung
exl-id: 5d1c5b52-5323-4f68-847b-7d24e6acd6c4
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 1%

---

# Aktivieren der nicht englischsprachigen benutzerdefinierten Objektsynchronisierung {#enable-non-english-custom-object-sync}

Wenn Ihr Marketo-Synchronisierungsbenutzer auf eine andere Sprache als Englisch festgelegt ist, tritt möglicherweise ein Fehler auf, wenn Sie versuchen, eine benutzerdefinierte Objektsynchronisierung zu aktivieren.

## Der Fehler {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## Umgehen {#getting-around-it}

1. Anmelden bei [!DNL Salesforce] Verwenden des Markets zum Synchronisieren von Benutzern.

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. Navigieren Sie unter dem Benutzernamen zu **[!UICONTROL Einrichtung]**.

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. under **[!UICONTROL Persönliche Informationen]** klicken **[!UICONTROL Meine personenbezogenen Daten]**.

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. Klicks **[!UICONTROL Bearbeiten]**.

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. Ändern Sie die **[!UICONTROL Sprache]** nach **[!UICONTROL englisch]**.

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. Zurück in Marketo, unter **[!UICONTROL Admin]** > **[!UICONTROL Salesforce]** > **[!UICONTROL Objekte]** klicken **[!UICONTROL Schema aktualisieren]**.

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. Dadurch wird die Objektliste in englischer Sprache abgerufen. Wählen Sie nun das Objekt Ihrer Wahl aus und klicken Sie auf **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. Beachten Sie, dass Ihr benutzerdefiniertes Objekt jetzt aktiviert und synchronisiert ist.

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. Gehen Sie zurück zu Salesforce und verwenden Sie die oben genannten Schritte, um den Synchronisierungsbenutzer wieder in Ihre bevorzugte Sprache zu ändern.

>[!NOTE]
>
>Vergessen Sie nicht, das Schema ein letztes Mal zu aktualisieren, um die Objekte in Ihrer Sprache zurückzuziehen.
