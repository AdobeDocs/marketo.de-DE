---
unique-page-id: 4719302
description: Benutzerdefinierte Objektsynchronisierung für Nicht-Englisch aktivieren - Marketo-Dokumente - Produktdokumentation
title: Aktivieren der nicht englischsprachigen benutzerdefinierten Objektsynchronisierung
exl-id: 5d1c5b52-5323-4f68-847b-7d24e6acd6c4
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---

# Aktivieren der nicht englischsprachigen benutzerdefinierten Objektsynchronisierung {#enable-non-english-custom-object-sync}

Wenn Ihr Marketo-Synchronisierungsbenutzer auf eine andere Sprache als Englisch festgelegt ist, tritt möglicherweise ein Fehler auf, wenn Sie versuchen, eine benutzerdefinierte Objektsynchronisierung zu aktivieren.

## Der Fehler {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## Umgehen {#getting-around-it}

1. Melden Sie sich mit dem Marketo zur Benutzersynchronisierung bei Salesforce an.

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. Navigieren Sie unter dem Benutzernamen zu **Einrichtung**.

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. under **Persönliche Informationen** klicken **Meine personenbezogenen Daten**.

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. Klicks **Bearbeiten**.

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. Ändern Sie die **Sprache** nach **englisch**.

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. Klicks **Speichern**.

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. Zurück in Marketo, unter **Admin > Salesforce > Objekte** click **Schema aktualisieren**.

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. Dadurch wird die Objektliste in englischer Sprache abgerufen. Wählen Sie nun das Objekt Ihrer Wahl aus und klicken Sie auf **Synchronisierung aktivieren**.

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. Beachten Sie, dass Ihr benutzerdefiniertes Objekt jetzt aktiviert ist und synchronisiert wird.

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. Gehen Sie zurück zu Salesforce und verwenden Sie die oben genannten Schritte, um den Synchronisierungsbenutzer wieder in Ihre bevorzugte Sprache zu ändern.

>[!NOTE]
>
>Vergessen Sie nicht, das Schema ein letztes Mal zu aktualisieren, um die Objekte in Ihrer Sprache zurückzuziehen.
