---
unique-page-id: 4719302
description: Benutzerdefinierte Objektsynchronisierung ohne Englisch aktivieren - Marketing Docs - Produktdokumentation
title: Benutzerdefinierte Objektsynchronisierung für Nicht-Englisch aktivieren
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---


# Nicht-englischsprachige benutzerdefinierte Objektsynchronisierung aktivieren {#enable-non-english-custom-object-sync}

Wenn Ihr Marketo-Synchronisierungsbenutzer auf eine andere Sprache als Englisch eingestellt ist, wird möglicherweise ein Fehler ausgegeben, wenn versucht wird, eine benutzerdefinierte Objektsynchronisierung zu aktivieren.

## Der Fehler {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## Umschließen {#getting-around-it}

1. Melden Sie sich mit dem Marker bei Salesforce an, um den Benutzer zu synchronisieren.

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. Wechseln Sie unter dem Benutzernamen zu **Setup**.

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. Klicken Sie unter **Persönliche Informationen** auf **Meine persönlichen Informationen**.

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. Klicken Sie auf **Bearbeiten**.

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. Ändern Sie **Sprache** in **Englisch**.

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. Zurück in Marketo, unter **Admin > Salesforce > Objekte** klicken Sie auf **Schema aktualisieren**.

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. Dadurch werden die Objekte in englischer Liste gezogen. Wählen Sie jetzt das Objekt Ihrer Wahl aus und klicken Sie auf **Synchronisierung aktivieren**.

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. Beachten Sie, dass Ihr benutzerdefiniertes Objekt jetzt aktiviert und synchronisiert ist.

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. Gehen Sie nun zurück zu Salesforce und verwenden Sie die oben genannten Schritte, um den Synchronisierungsbenutzer wieder in Ihre bevorzugte Sprache zu ändern.

>[!NOTE]
>
>Vergessen Sie nicht, das Schema ein letztes Mal zu aktualisieren, um die Objekte in Ihrer Sprache zurückzuziehen.
