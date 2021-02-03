---
unique-page-id: 37355758
description: Hinzufügen von Mitgliedern zu einem Ereignis-Programm - Marketing Docs - Produktdokumentation
title: Hinzufügen von Mitgliedern zu einem Ereignis-Programm
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---


# Hinzufügen von Mitgliedern zu einem Ereignis-Programm {#adding-members-to-an-event-program}

Dieser Artikel gilt nur für Benutzer, die Ereignis Cap oder Ereignis Goals verwenden.

>[!CAUTION]
>
>Wenn Sie eine Liste von Personen direkt in ein Ereignis-Programm importieren, wird verhindert, dass diese Datensätze in den eigentlichen Registrierungen im Bericht &quot;Zielverfolgung&quot;und im Bericht &quot;Fortschrittlichkeit bei Ereignissen&quot;gezählt werden. Befolgen Sie die unten stehenden Anweisungen, um sicherzustellen, dass Ihre Datensätze gezählt werden.

1. Erstellen und [Hinzufügen von Personen zu einer statischen Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md).

1. [Erstellen Sie eine intelligente Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md).

1. Suchen Sie in der Smart-Liste der Smart-Kampagne, die Sie in Schritt 2 erstellt haben, den Filter **Member of Liste** und fügen Sie ihn hinzu.

   ![](assets/three.png)

1. Suchen Sie die Liste, die Sie in Schritt 1 erstellt haben, und wählen Sie sie aus.

   ![](assets/four.png)

1. Suchen und fügen Sie im Fluss den Textfluss **Change Programm Status** hinzu.

   ![](assets/five.png)

1. Suchen und wählen Sie Ihr Ereignis-Programm aus.

   ![](assets/six.png)

1. Wählen Sie den gewünschten Status aus.

   ![](assets/seven.png)

1. Klicken Sie auf der Registerkarte Plan auf **Einmal ausführen**.

   ![](assets/eight.png)

1. Wählen Sie **Jetzt ausführen** und klicken Sie auf **Ausführen**.

   ![](assets/nine.png)

1. Nachdem die intelligente Kampagne ausgeführt wurde, werden die Mitglieder dem Programm hinzugefügt und zählen in den Berechnungen für die Zielverfolgung und die Ereignis-Cap-Progression.
