---
unique-page-id: 557322
description: Führen Sie einen Einzelflussschritt von einer intelligenten Liste aus - Marketo Docs - Produktdokumentation
title: Ausführen eines einzelnen Flussschritts aus einer intelligenten Liste
exl-id: 1ac5795b-1906-4f94-bd0a-570d55c9357b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 1%

---

# Ausführen eines Einzelflussschritts von einer intelligenten Liste {#run-a-single-flow-step-from-a-smart-list}

Wenn Sie einen einzigen Flussschritt ausführen möchten, können Sie einen einzelnen Flussschritt innerhalb einer intelligenten Liste verwenden, anstatt eine ganze intelligente Kampagne zu erstellen.

>[!PREREQUISITES]
>
>[Erstellen einer intelligenten Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. Gehen Sie zu **Marketing-Aktivitäten**.

   ![](assets/login-marketing-activities-1.png)

1. Wählen Sie eine Liste oder eine intelligente Liste mit den darin enthaltenen Personen aus und gehen Sie dann zur Registerkarte **Personen**.

   ![](assets/smartlistpeopletab-hands.png)

   >[!TIP]
   >
   >Diese Funktion ist sowohl für statische Listen als auch für intelligente Listen verfügbar.

1. Klicken Sie auf **Alle auswählen**. Sie können auch **Strg/Cmd** verwenden und auf klicken, um einige Datensätze manuell auszuwählen.

   ![](assets/smartlist-selectallhand.png)

   >[!NOTE]
   >
   >Wenn sich die Ergebnisse über mehrere Seiten erstrecken, werden durch Klicken auf **Alle auswählen** alle Personen auf allen Seiten ausgewählt.

1. Wählen Sie unter **Person** **Aktionen** den gewünschten Flussschritt aus. In diesem Beispiel verwenden wir [Datenwert ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md).

   ![](assets/personactions-hands.png)

1. Suchen und wählen Sie ein **Attribut**. In diesem Beispiel nehmen wir alle Leute, die &quot;Kalifornien&quot;haben, und ändern es in &quot;CA&quot;.

   ![](assets/runaction-hands.png)

1. Neuen Wert eingeben. Klicken Sie auf **Jetzt ausführen**.

   ![](assets/runactionnewvalue-hands.png)

1. Wenn Sie Datenwerte für eine große Anzahl von Personen ändern, müssen Sie die Änderung möglicherweise bestätigen, indem Sie die Zahl eingeben. Klicken Sie auf **Gehen Sie zu**.

   ![](assets/changedatavalue.jpg)

Fantastische Arbeit! Der Status des einzelnen Flussschritts wird oben rechts angezeigt.

![](assets/completesingleflowaction.jpg)

Wenn die Liste abgeschlossen ist, aktualisieren Sie sie und Sie sehen die aktualisierten Informationen.
