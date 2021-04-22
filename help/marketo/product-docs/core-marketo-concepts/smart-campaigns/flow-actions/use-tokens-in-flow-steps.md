---
unique-page-id: 1146995
description: Token in Flussschritten verwenden - Marketo Docs - Produktdokumentation
title: Tokens in Flussschritten verwenden
exl-id: 9b4c3d57-5906-4d7c-8215-4ba2271be3f8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 8%

---

# Token in Flussschritten {#use-tokens-in-flow-steps} verwenden

>[!AVAILABILITY]
>
>Nicht alle Kunden haben diese Funktion erworben. Detaillierte Informationen erhalten Sie vom zuständigen Vertriebsmitarbeiter.

>[!PREREQUISITES]
>
>[hinzufügen eines Flussschritts zu einer intelligenten Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md)

Ein Token ist eine Variable. Sie verwenden sie in E-Mails, Landingpages und intelligenten Kampagnen, um Ihr Leben zu vereinfachen. Sie können [Meine Token](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md) (benutzerdefinierte Token) in Flussschritten, Webhooks, E-Mails und Landingpages verwenden. Sie können Token verwenden, um variablen Inhalt in die folgenden Flussschritte einzuschließen:

* Datenwert ändern
* Programmmitgliedsdaten ändern
* Interessanter Moment
* Schritte zur Kampagne von Salesforce (Hinzufügen, Entfernen, Ändern des Status)
* Aufgabe erstellen
* Warnung senden (nur in Trigger-Kampagnen)

1. Geben Sie im Flussschritt `{{` ein, um Token-Kategorien abzurufen. ![](assets/image2014-9-22-14-3a3-3a17.png)

   >[!NOTE]
   >
   >Sehen Sie sich [Tokens Overview](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) für eine Liste verschiedener verfügbarer Token an.

1. Tippen Sie weiter, bis Sie das gewünschte Token gefunden haben, und klicken Sie auf die gewünschte Auswahl.

   ![](assets/image2014-9-22-14-3a3-3a48.png)

   >[!TIP]
   >
   >Es können mehrere Token in den Arbeitsschritten &quot;Interessanter Moment&quot;, &quot;Aufgabe erstellen&quot;und &quot;Warnhinweis senden&quot;verwendet werden.

   >[!NOTE]
   >
   >Benutzerdefinierte FeldToken für Programm-Member können verwendet werden in: Erstellen Sie Aufgaben, erstellen Sie Aufgaben in Microsoft, interessante Momente, ändern Sie die Aktionen zum Datenwertfluss und Webhooks.

   Cool! Die Daten werden beim Ausführen der intelligenten Kampagne aus dem Token gezogen.

   >[!MORELIKETHIS]
   >
   >* [Verwalten von My Tokens](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)
   >* [Meine Token in einem Programm](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md)

