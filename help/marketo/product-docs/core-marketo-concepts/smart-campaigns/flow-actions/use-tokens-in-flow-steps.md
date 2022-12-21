---
unique-page-id: 1146995
description: Verwenden von Token in Flussschritten - Marketo Docs - Produktdokumentation
title: Verwenden von Token in Flussschritten
exl-id: 9b4c3d57-5906-4d7c-8215-4ba2271be3f8
source-git-commit: 46812deb41ed56328a4a64fbd36340d13c50dde4
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 6%

---

# Verwenden von Token in Flussschritten {#use-tokens-in-flow-steps}

>[!PREREQUISITES]
>
>[Hinzufügen eines Flussschritts zu einer Smart-Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)

Ein Token ist eine Variable. Sie können sie in E-Mails, Landingpages und intelligenten Kampagnen verwenden, um Ihr Leben zu vereinfachen. Sie können [Meine Token](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md) (benutzerdefinierte Token) in Flussprofilen, Webhooks, E-Mails und Landingpages. Sie können Token verwenden, um Variableninhalte in diese Flussschritte einzuschließen:

* Datenwert ändern
* Programmmitgliedsdaten ändern
* Interessanter Moment
* Salesforce Campaign-Schritte (Hinzufügen, Entfernen, Ändern des Status)
* Aufgabe erstellen
* Warnhinweis senden (nur in Trigger-Kampagnen)

1. Beginnen Sie im Flussschritt mit der Eingabe von `{{` , um Tokenkategorien abzurufen.

   ![](assets/image2014-9-22-14-3a3-3a17.png)

   >[!NOTE]
   >
   >Checkout [Token-Übersicht](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) für eine Liste verschiedener verfügbarer Token.

1. Fahren Sie mit der Eingabe fort, bis Sie das gewünschte Token finden und klicken Sie zur Auswahl.

   ![](assets/image2014-9-22-14-3a3-3a48.png)

   >[!TIP]
   >
   >Es können mehrere Token in den Schritten &quot;Interessanter Moment&quot;, &quot;Aufgabe erstellen&quot;und &quot;Warnhinweisfluss senden&quot;verwendet werden.

   >[!NOTE]
   >
   >Benutzerdefinierte Feld-Token für Programmmitglieder können in folgenden Bereichen verwendet werden: Erstellen von Aufgaben, Erstellen von Aufgaben in Microsoft, interessante Momente, Ändern von Datenwertflussaktionen und Webhooks.

   Cool! Die Daten werden beim Ausführen der Smart-Kampagne aus dem Token abgerufen.

   >[!MORELIKETHIS]
   >
   >* [Verwalten von My Tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)
   >* [Grundlegendes zu meinen Token in einem Programm](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md)

