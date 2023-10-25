---
unique-page-id: 557322
description: Führen Sie einen Einzelflussschritt von einer intelligenten Liste aus - Marketo-Dokumente - Produktdokumentation
title: Ausführen eines einzelnen Flussschritts aus einer intelligenten Liste
exl-id: 1ac5795b-1906-4f94-bd0a-570d55c9357b
feature: Smart Lists
source-git-commit: 8a5903fa5313e34f448f833f20ab8e3624cf23e6
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 1%

---

# Ausführen eines einzelnen Flussschritts aus einer intelligenten Liste {#run-a-single-flow-step-from-a-smart-list}

Wenn Sie einen einmaligen Flussschritt ausführen möchten, können Sie einen einzelnen Flussschritt in einer Smart-Liste verwenden, anstatt eine gesamte Smart-Kampagne zu erstellen.

>[!PREREQUISITES]
>
>[Erstellen einer Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}

1. Navigieren Sie zu **[!UICONTROL Marketingaktivitäten]**.

   ![](assets/login-marketing-activities-1.png)

1. Wählen Sie eine Liste oder Smart-Liste mit Personen darin aus und navigieren Sie dann zum **[!UICONTROL Personen]** Registerkarte.

   ![](assets/smartlistpeopletab-hands.png)

   >[!TIP]
   >
   >Sowohl statische Listen als auch Smart-Listen verfügen über diese Funktion.

1. Klicks **[!UICONTROL Alle auswählen]**. Sie können auch **Strg/Befehl** und klicken Sie auf , um einige Datensätze manuell auszuwählen.

   ![](assets/smartlist-selectallhand.png)

   >[!NOTE]
   >
   >Wenn sich die Ergebnisse über mehrere Seiten erstrecken, klicken Sie auf **[!UICONTROL Alle auswählen]** werden alle Personen auf allen Seiten ausgewählt.

1. under **[!UICONTROL Personenaktionen]** wählen Sie den gewünschten Flussschritt aus. In diesem Beispiel verwenden wir [Datenwert ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}.

   ![](assets/personactions-hands.png)

1. Suchen und Auswählen einer **[!UICONTROL Attribut]**. In diesem Beispiel nehmen wir alle Personen mit dem Status &quot;Kalifornien&quot;und ändern es in &quot;CA&quot;.

   ![](assets/runaction-hands.png)

1. Neuen Wert eingeben. Klicks **[!UICONTROL Jetzt ausführen]**.

   ![](assets/runactionnewvalue-hands.png)

1. Wenn Sie Datenwerte für eine große Anzahl von Personen ändern, müssen Sie die Änderung möglicherweise bestätigen, indem Sie die Zahl eingeben. Klicks **[!UICONTROL Los]**.

   ![](assets/changedatavalue.jpg)

Fantastische Arbeit! Der Status des einzelnen Flussschritts wird oben rechts angezeigt.

![](assets/completesingleflowaction.jpg)

Wenn die Liste fertig ist, aktualisieren Sie sie und Sie sehen die aktualisierten Informationen.
