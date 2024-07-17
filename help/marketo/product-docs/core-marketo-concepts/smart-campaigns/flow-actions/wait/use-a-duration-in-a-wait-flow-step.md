---
unique-page-id: 1146978
description: Verwenden einer Dauer in einem Warteflussschritt - Marketo Docs - Produktdokumentation
title: Verwenden einer Dauer in einem Warteflussschritt
exl-id: 7b13d225-78ba-4ef1-9ff5-0f6acde6e5ff
feature: Smart Campaigns
source-git-commit: 12f2399859c784095cc2c1df772c66c649106ba3
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 1%

---

# Verwenden einer Dauer in einem Warteflussschritt {#use-a-duration-in-a-wait-flow-step}

Mit dem Schritt Wartefluss können Sie das Journey einer Person über eine Smart-Kampagne für eine bestimmte Dauer anhalten. Sie können auch Kriterien für den Wochentag und die Uhrzeit des Endes festlegen.

1. Ziehen Sie in der Registerkarte **[!UICONTROL Fluss]** Ihrer Smart-Kampagne über den Flussschritt **[!UICONTROL Warten]**.

   ![](assets/use-a-duration-in-a-wait-flow-step-1.png)

1. Geben Sie an, wie lange Sie anhalten möchten.

   ![](assets/use-a-duration-in-a-wait-flow-step-2.png)

1. Das ist es! Der Fluss wird für die angegebene Dauer angehalten. Für erweiterte Optionen klicken Sie auf das Zahnradsymbol rechts.

   ![](assets/use-a-duration-in-a-wait-flow-step-3.png)

1. Geben Sie den Wochentag an, an dem der Warteschritt enden soll.

   ![](assets/use-a-duration-in-a-wait-flow-step-4.png)

1. Geben Sie optional die Zeit an. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/use-a-duration-in-a-wait-flow-step-5.png)

   >[!NOTE]
   >
   >**Beispiel**
   >
   >Eine Person Trigger am Freitag um 17 Uhr eine Smart-Kampagne. Der Warteschritt ist fortgeschritten: 48 Stunden und muss am Montag um 9 Uhr enden.
   >
   >Das Ergebnis wäre, dass die Person am **Montag, 9.00 Uhr** im Fluss bleiben würde. Dies ist das erste M-F-Datum nach 48 Stunden.

   >[!NOTE]
   >
   >Dauer, Datum, Uhrzeit und Tage basieren alle auf der Zeitzone Ihres Abonnements.

   >[!MORELIKETHIS]
   >
   >* [Verwenden eines bestimmten Datums in einem Warteflussschritt](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md){target="_blank"}
   >* [Verwenden eines Datums-Tokens in einem Warteflussschritt](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md){target="_blank"}
