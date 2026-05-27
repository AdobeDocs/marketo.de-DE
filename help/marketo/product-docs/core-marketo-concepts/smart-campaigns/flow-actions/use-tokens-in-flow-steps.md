---
unique-page-id: 1146995
description: Erfahren Sie, wie Sie Token in Flussschritten verwenden. Fügen Sie dynamische Werte in den Inhalt der Flussschritte und in E-Mails ein.
title: Verwenden von Token in Flussschritten
exl-id: 9b4c3d57-5906-4d7c-8215-4ba2271be3f8
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/0b1iseuF-rKtBcS2qPRdwnPPRYJxUNG9hzlJQxNJQdI
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
subfeature_v2:
  - id: ad89fb33-8541-4339-afe7-bb13d1633714
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 200
ht-degree: 10%

---

# Verwenden von Token in Flussschritten {#use-tokens-in-flow-steps}

>[!PREREQUISITES]
>
>[Hinzufügen eines Flussschritts zu einer Smart-Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}

Ein Token ist eine Variable. Sie können ihn in E-Mails, Landingpages und intelligenten Kampagnen verwenden, um Ihnen das Leben zu erleichtern. Sie können [Meine Token](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md){target="_blank"} (benutzerdefinierte Token) in Flussschritten, Webhooks, E-Mails und Landingpages verwenden. Sie können Token verwenden, um Variableninhalte in diese Flussschritte einzuschließen:

* Datenwert ändern
* Ändern von Programmmitgliedsdaten
* Interessanter Moment
* [!DNL Salesforce] Kampagnenschritte (hinzufügen, entfernen, Status ändern)
* Erstellen von Aufgaben
* Warnhinweis senden (nur in Trigger-Kampagnen)

1. Beginnen Sie im Flussschritt mit der Eingabe von `{{`, um Token-Kategorien abzurufen.

   ![](assets/use-tokens-in-flow-steps-1.png)

   >[!NOTE]
   >
   >Unter [Token-Übersicht](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"} finden Sie eine Liste mehrerer verfügbarer Token.

1. Tippen Sie so lange, bis Sie das gewünschte Token gefunden haben, und klicken Sie zum Auswählen darauf.

   ![](assets/use-tokens-in-flow-steps-2.png)

   >[!TIP]
   >
   >In den Schritten „Interessanter Moment“, „Aufgabe erstellen“ und „Warnhinweis senden“ können mehrere Token verwendet werden.

   >[!NOTE]
   >
   >Benutzerdefinierte Feld-Token für Programmteilnehmer können in folgenden Bereichen verwendet werden: Erstellen einer Aufgabe, Erstellen einer Aufgabe in Microsoft, Interessante Momente, Ändern von Datenwerten, Flussaktionen und Webhooks.

   Die Daten werden aus dem Token abgerufen, wenn die Smart Campaign ausgeführt wird.

   >[!MORELIKETHIS]
   >
   >* [Meine Token verwalten](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"}
   >* [Verstehen meiner Token in einem Programm](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md){target="_blank"}
