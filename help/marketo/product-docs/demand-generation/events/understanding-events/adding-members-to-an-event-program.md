---
unique-page-id: 37355758
description: Hinzufügen von Mitgliedern zu einem Veranstaltungsprogramm - Marketo-Dokumente - Produktdokumentation
title: Hinzufügen von Mitgliedern zu einem Veranstaltungsprogramm
exl-id: 05bd4807-3ab8-452d-a389-b22477cf7445
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---

# Hinzufügen von Mitgliedern zu einem Veranstaltungsprogramm {#adding-members-to-an-event-program}

Dieser Artikel gilt nur für Benutzer, die Event-Begrenzungs- oder Event-Ziele verwenden.

>[!CAUTION]
>
>Wenn Sie eine Liste von Personen direkt in ein Veranstaltungsprogramm importieren, werden diese Datensätze bei den tatsächlichen Registrierungen im Zielverfolgungsbericht und im Ereignisbegrenzungs-Fortschrittsbericht nicht gezählt. Folgen Sie den unten stehenden Anweisungen, um sicherzustellen, dass Ihre Datensätze gezählt werden.

1. Erstellen und [Hinzufügen von Personen zu einer statischen Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md).

1. [Erstellen Sie eine intelligente Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md).

1. Suchen Sie in der Smart List der Smart Campaign, die Sie in Schritt 2 erstellt haben, den Filter **Member of List** und fügen Sie ihn hinzu.

   ![](assets/three.png)

1. Suchen Sie die in Schritt 1 erstellte Liste und wählen Sie sie aus.

   ![](assets/four.png)

1. Suchen Sie im Fluss den Flussschritt **Programmstatus ändern** und fügen Sie ihn hinzu.

   ![](assets/five.png)

1. Suchen und wählen Sie Ihr Veranstaltungsprogramm.

   ![](assets/six.png)

1. Wählen Sie den gewünschten Status aus.

   ![](assets/seven.png)

1. Klicken Sie auf der Registerkarte Zeitplan auf **Einmal ausführen**.

   ![](assets/eight.png)

1. Wählen Sie **Jetzt ausführen** und klicken Sie auf **Ausführen**.

   ![](assets/nine.png)

1. Nach der Ausführung der intelligenten Kampagne werden die Mitglieder zum Programm hinzugefügt und in den Berechnungen für die Zielverfolgung und die Ereignisbegrenzungsprogression gezählt.
