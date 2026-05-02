---
unique-page-id: 557322
description: Erfahren Sie, wie Sie einen einzelnen Flussschritt aus einer Smart-Liste ausführen. Führt eine Flussaktion für ausgewählte Personen aus der Liste aus.
title: Ausführen eines einzelnen Flussschritts aus einer intelligenten Liste
exl-id: 1ac5795b-1906-4f94-bd0a-570d55c9357b
feature: Smart Lists
source-git-commit: 60c5603fa29bb1039b9d477633beb2c6f5c63486
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 9%

---

# Ausführen eines einzelnen Flussschritts aus einer intelligenten Liste {#run-a-single-flow-step-from-a-smart-list}

Wenn Sie einen einmaligen Flussschritt ausführen möchten, können Sie in einer Smart-Liste einen einzelnen Flussschritt verwenden, anstatt eine gesamte Smart-Kampagne zu erstellen.

>[!PREREQUISITES]
>
>[Erstellen einer Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}

1. Navigieren Sie zu **[!UICONTROL Marketing-Aktivitäten]**.

   ![](assets/run-a-single-flow-step-from-a-smart-list-1.png)

1. Wählen Sie eine Liste oder Smart-Liste mit Personen aus und wechseln Sie dann zur Registerkarte **[!UICONTROL Personen]**.

   ![](assets/run-a-single-flow-step-from-a-smart-list-2.png)

   >[!TIP]
   >
   >Sowohl statische Listen als auch Smart Lists verfügen über diese Funktion.

1. Klicken Sie **[!UICONTROL Alle auswählen]**. Sie können auch **Strg/Befehl** verwenden und auf einige Datensätze klicken, um sie manuell auszuwählen.

   ![](assets/run-a-single-flow-step-from-a-smart-list-3.png)

   >[!NOTE]
   >
   >Wenn sich die Ergebnisse über mehrere Seiten erstrecken, werden durch Klicken auf **[!UICONTROL Alle auswählen]** alle Personen auf allen Seiten ausgewählt.

1. Wählen **[!UICONTROL unter]** den gewünschten Flussschritt aus. In diesem Beispiel wird [Datenwert ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} verwendet.

   ![](assets/run-a-single-flow-step-from-a-smart-list-4.png)

1. Suchen Sie ein „Attribut **[!UICONTROL und wählen Sie es]**. In diesem Beispiel nehmen wir alle Personen, die den Bundesstaat „Kalifornien“ haben, und ändern ihn in „CA“.

   ![](assets/run-a-single-flow-step-from-a-smart-list-5.png)

1. Einen neuen Wert eingeben. Klicken Sie **[!UICONTROL Jetzt ausführen]**.

   ![](assets/run-a-single-flow-step-from-a-smart-list-6.png)

1. Wenn Sie Datenwerte für eine große Anzahl von Personen ändern, müssen Sie die Änderung möglicherweise bestätigen, indem Sie die Zahl eingeben. Klicken Sie **[!UICONTROL Los]**.

   ![](assets/run-a-single-flow-step-from-a-smart-list-7.png)

Der Status des einzelnen Flussschritts wird in der oberen rechten Ecke angezeigt.

![](assets/run-a-single-flow-step-from-a-smart-list-8.png)

Wenn sie abgeschlossen ist, aktualisieren Sie die Liste und Sie sehen die aktualisierten Informationen.
