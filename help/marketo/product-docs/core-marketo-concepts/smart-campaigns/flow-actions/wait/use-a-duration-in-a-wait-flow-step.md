---
unique-page-id: 1146978
description: Verwenden einer Dauer in einem Warteflussschritt - Marketo Docs - Produktdokumentation
title: Verwenden einer Dauer in einem Warteflussschritt
exl-id: 7b13d225-78ba-4ef1-9ff5-0f6acde6e5ff
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# Verwenden einer Dauer in einem Warteflussschritt {#use-a-duration-in-a-wait-flow-step}

Mit dem Schritt Wartefluss können Sie das Journey einer Person für eine bestimmte Dauer durch eine intelligente Kampagne anhalten. Sie können auch Kriterien für den Wochentag und die Uhrzeit des Endes festlegen.

1. In Ihrer intelligenten Kampagne **Fluss** Registerkarte, ziehen Sie über die **Warten** Flussschritt.

   ![](assets/image2014-9-22-11-3a53-3a57.png)

1. Geben Sie an, wie lange Sie anhalten möchten.

   ![](assets/image2014-9-22-11-3a54-3a0.png)

1. Das ist es! Der Fluss wird für die angegebene Dauer angehalten. Für erweiterte Optionen klicken Sie auf das Zahnradsymbol rechts.

   ![](assets/image2014-9-22-11-3a54-3a7.png)

1. Geben Sie den Wochentag an, an dem der Warteschritt enden soll.

   ![](assets/image2014-9-22-11-3a54-3a10.png)

1. Geben Sie optional die Zeit an. Klicks **Speichern**.

   ![](assets/image2014-9-22-11-3a54-3a35.png)

   >[!NOTE]
   >
   >**Beispiel**
   >
   >Eine Person Trigger am Freitag um 17 Uhr eine Smart-Kampagne. Der Warteschritt ist fortgeschritten: 48 Stunden und muss am Montag um 9 Uhr enden.
   >
   >Das Ergebnis wäre, dass die Person im Fluss fortfahren würde **Montag, 9 Uhr**. Dies ist das erste M-F-Datum nach 48 Stunden.

   >[!NOTE]
   >
   >Dauer, Datum, Uhrzeit und Tage basieren alle auf der Zeitzone Ihres Abonnements.

   >[!MORELIKETHIS]
   >
   >* [Verwenden eines bestimmten Datums in einem Warteflussschritt](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
   >* [Verwenden eines Datums-Tokens in einem Warteflussschritt](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)
