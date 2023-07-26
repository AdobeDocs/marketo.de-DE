---
unique-page-id: 37355758
description: Hinzufügen von Mitgliedern zu einem Ereignisprogramm - Marketo-Dokumente - Produktdokumentation
title: Hinzufügen von Mitgliedern zu einem Veranstaltungsprogramm
exl-id: 05bd4807-3ab8-452d-a389-b22477cf7445
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---

# Hinzufügen von Mitgliedern zu einem Veranstaltungsprogramm {#adding-members-to-an-event-program}

Dieser Artikel gilt nur für Benutzer, die Event Cap oder Event Goals verwenden.

>[!CAUTION]
>
>Durch den Import einer Personenliste direkt in ein Ereignisprogramm wird verhindert, dass diese Datensätze in den eigentlichen Registrierungen im Zielverfolgungsbericht und im Bericht zur Event Cap-Progression gezählt werden. Befolgen Sie die nachstehenden Anweisungen, um sicherzustellen, dass Ihre Datensätze gezählt werden.

1. Erstellen und [Personen zu einer statischen Liste hinzufügen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md).

1. [Erstellen einer Smart-Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md).

1. Suchen und fügen Sie in der Smart-Liste der Smart-Kampagne, die Sie in Schritt 2 erstellt haben, die **Mitglied der Liste** Filter.

   ![](assets/three.png)

1. Suchen und wählen Sie die Liste aus, die Sie in Schritt 1 erstellt haben.

   ![](assets/four.png)

1. Suchen Sie im Fluss nach und fügen Sie die **Ändern des Programmstatus** Flussschritt.

   ![](assets/five.png)

1. Suchen und wählen Sie Ihr Veranstaltungsprogramm aus.

   ![](assets/six.png)

1. Wählen Sie den gewünschten Status aus.

   ![](assets/seven.png)

1. Klicken Sie im Tab Planung auf **Einmal ausführen**.

   ![](assets/eight.png)

1. Auswählen **Jetzt ausführen** und klicken **Ausführen**.

   ![](assets/nine.png)

1. Nachdem die intelligente Kampagne ausgeführt wurde, werden die Mitglieder zum Programm hinzugefügt und in den Berechnungen Zielverfolgung und Ereignis-Begrenzung berücksichtigt.
