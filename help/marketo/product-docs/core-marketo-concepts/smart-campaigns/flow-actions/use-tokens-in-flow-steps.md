---
unique-page-id: 1146995
description: Verwenden von Token in Flussschritten - Marketo Docs - Produktdokumentation
title: Verwenden von Token in Flussschritten
exl-id: 9b4c3d57-5906-4d7c-8215-4ba2271be3f8
feature: Smart Campaigns
source-git-commit: 12f2399859c784095cc2c1df772c66c649106ba3
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 5%

---

# Verwenden von Token in Flussschritten {#use-tokens-in-flow-steps}

>[!PREREQUISITES]
>
>[Hinzufügen eines Flussschritts zu einer Smart-Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md){target="_blank"}

Ein Token ist eine Variable. Sie können sie in E-Mails, Landingpages und Smart-Kampagnen verwenden, um Ihr Leben zu vereinfachen. Sie können [My Tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md){target="_blank"} (benutzerdefinierte Token) in Flussprofilen, Webhooks, E-Mails und Landingpages verwenden. Sie können Token verwenden, um Variableninhalte in diese Flussschritte einzuschließen:

* Datenwert ändern
* Programmmitgliedsdaten ändern
* Interessanter Moment
* Salesforce Campaign-Schritte (Hinzufügen, Entfernen, Ändern des Status)
* Aufgabe erstellen
* Warnhinweis senden (nur in Trigger-Kampagnen)

1. Geben Sie im Flussschritt `{{` ein, um Tokenkategorien abzurufen.

   ![](assets/use-tokens-in-flow-steps-1.png)

   >[!NOTE]
   >
   >Unter [Token-Übersicht](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"} finden Sie eine Liste verschiedener verfügbarer Token.

1. Fahren Sie mit der Eingabe fort, bis Sie das gewünschte Token finden und klicken Sie zur Auswahl.

   ![](assets/use-tokens-in-flow-steps-2.png)

   >[!TIP]
   >
   >Es können mehrere Token in den Schritten &quot;Interessanter Moment&quot;, &quot;Aufgabe erstellen&quot;und &quot;Warnhinweisfluss senden&quot;verwendet werden.

   >[!NOTE]
   >
   >Benutzerdefinierte Feld-Token für Programmmitglieder können in folgenden Bereichen verwendet werden: Aufgabe erstellen, Aufgabe in Microsoft erstellen, interessante Momente, Fluss-Aktionen für Datenwerte ändern und Webhooks.

   Cool! Die Daten werden beim Ausführen der Smart-Kampagne aus dem Token abgerufen.

   >[!MORELIKETHIS]
   >
   >* [Verwalten meiner Token](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"}
   >* [Grundlegendes zu meinen Token in einem Programm](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md){target="_blank"}
