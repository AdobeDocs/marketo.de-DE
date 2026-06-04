---
unique-page-id: 4719302
description: Erfahren Sie, wie Sie die Synchronisierung benutzerdefinierter Objekte aktivieren, wenn der Marketo-Synchronisierungsbenutzer eine andere Sprache als Englisch verwendet. Legen Sie in Salesforce die Synchronisierungsbenutzersprache auf Englisch fest und aktualisieren Sie das Schema.
title: Aktivieren der Synchronisierung benutzerdefinierter Objekte in anderen Sprachen als Englisch
exl-id: 5d1c5b52-5323-4f68-847b-7d24e6acd6c4
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/kPzDEdjDnDAvuJmCtPj0I2Lfl63Lset00t-LwB8DDhI
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: 67c57a9162946c4b9c424ab3fd445b70e90b530a
workflow-type: tm+mt
source-wordcount: 195
ht-degree: 9%

---

# Aktivieren der Synchronisierung benutzerdefinierter Objekte in anderen Sprachen als Englisch {#enable-non-english-custom-object-sync}

Wenn Ihr Marketo-Synchronisierungsbenutzer auf eine andere Sprache als Englisch eingestellt ist, kann beim Versuch, eine benutzerdefinierte Objektsynchronisierung zu aktivieren, ein Fehler auftreten.

![](assets/image2014-12-10-13-3a17-3a51.png)

## Fehlerbehebung {#how-to-fix}

1. Melden Sie sich mit dem Marketo Sync-Benutzer bei [!DNL Salesforce] an.

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. Klicken Sie auf die Dropdown-Liste Benutzername und wählen Sie **[!UICONTROL Setup]**.

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. Klicken **[!UICONTROL unter &quot;]**&quot; auf **[!UICONTROL Meine persönlichen Informationen]**.

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. Klicken Sie auf **[!UICONTROL Bearbeiten]**.

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. Ändern Sie **[!UICONTROL Sprache]** in **[!UICONTROL Englisch]**.

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. Scrollen Sie in Ihrem [Adobe](https://account.adobe.com/profile){target="_blank"}Kontoprofil nach unten zu **[!UICONTROL Bevorzugte Sprachen]** und stellen Sie sicher, dass Ihre erste Sprache auf Englisch eingestellt ist.

   ![](assets/enable-non-english-custom-object-sync-step-6.5.png)

1. Navigieren Sie in Marketo Engage zu **[!UICONTROL Admin]** > **[!UICONTROL Salesforce]** > **[!UICONTROL Objekte]**. Klicken Sie **[!UICONTROL Schema aktualisieren]**.

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. Dadurch wird die Objektliste in englischer Sprache abgerufen. Wählen Sie das gewünschte Objekt aus und klicken Sie auf **[!UICONTROL Synchronisierung aktivieren]**.

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. Das benutzerdefinierte Objekt ist jetzt aktiviert und wird synchronisiert.

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. Kehren Sie zu [!DNL Salesforce] zurück und ändern Sie mithilfe der oben genannten Schritte den Synchronisierungsbenutzer wieder in Ihre bevorzugte Sprache.

>[!NOTE]
>
>Aktualisieren Sie das Schema ein letztes Mal, um die Objekte in Ihrer Sprache zurückzuholen.
