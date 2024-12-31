---
unique-page-id: 4719302
description: Aktivieren der Synchronisierung nicht englischer benutzerdefinierter Objekte - Marketo-Dokumente - Produktdokumentation
title: Aktivieren der Synchronisierung benutzerdefinierter Objekte in anderen Sprachen
exl-id: 5d1c5b52-5323-4f68-847b-7d24e6acd6c4
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 2%

---

# Aktivieren der Synchronisierung benutzerdefinierter Objekte in anderen Sprachen {#enable-non-english-custom-object-sync}

Wenn Ihr Marketo-Synchronisierungsbenutzer auf eine andere Sprache als Englisch eingestellt ist, kann beim Versuch, eine benutzerdefinierte Objektsynchronisierung zu aktivieren, ein Fehler auftreten.

## Der Fehler {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## Um ihn herumzukommen {#getting-around-it}

1. Melden Sie sich mit dem Marketo Sync-Benutzer bei [!DNL Salesforce] an.

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. Wechseln Sie unter dem Benutzernamen zu **[!UICONTROL Setup]**.

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. Klicken **[!UICONTROL unter &quot;]**&quot; auf **[!UICONTROL Meine persönlichen Informationen]**.

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. Klicken Sie auf **[!UICONTROL Bearbeiten]**.

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. Ändern Sie **[!UICONTROL Sprache]** in **[!UICONTROL Englisch]**.

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. Zurück in Marketo, klicken **[!UICONTROL unter]** > **[!UICONTROL Salesforce]** > **[!UICONTROL Objekte]** auf **[!UICONTROL Schema aktualisieren]**.

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. Dadurch wird die Objektliste in englischer Sprache angezeigt. Wählen Sie nun das gewünschte Objekt aus und klicken Sie auf **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. Beachten Sie, dass Ihr benutzerdefiniertes Objekt jetzt aktiviert ist und synchronisiert wird.

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. Gehen Sie nun zurück zu Salesforce und ändern Sie mithilfe der oben genannten Schritte den Synchronisierungsbenutzer wieder in Ihre bevorzugte Sprache.

>[!NOTE]
>
>Vergessen Sie nicht, das Schema ein letztes Mal zu aktualisieren, um die Objekte in Ihrer Sprache zurückzuholen.
