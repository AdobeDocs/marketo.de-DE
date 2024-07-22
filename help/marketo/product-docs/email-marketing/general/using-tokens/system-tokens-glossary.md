---
unique-page-id: 1147344
description: System Tokens-Glossar - Marketo Docs - Produktdokumentation
title: Glossar zu System-Token
exl-id: 8a7694af-4edb-4b32-b408-19d2e7bd596e
feature: Tokens
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# Glossar zu System-Token {#system-tokens-glossary}

Neben Personen-Token können Sie auch einige wirklich coole System-Token verwenden. Hier sind sie.

>[!NOTE]
>
>Die Zeitzoneneinstellungen Ihres Kontos wirken sich auf die Ausführung von Datums- und Uhrzeit-Token aus.

## system.date {#system-date}

Das `{{system.date}}`-Token gibt das aktuelle Datum zur Laufzeit wie folgt aus: **8. August 2013**

**Funktioniert in:**

* Flussschritt [Datenwert ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}
* Flussschritt [interessanter Moment](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"}
* Workflow-Schritt [Aufgabe erstellen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}
* Der Textkörper einer E-Mail oder Vorlage

## system.time {#system-time}

Das `{{system.time}}` -Token gibt die aktuelle Zeit zur Laufzeit wie folgt aus: **04:34 PM (GMT -0700)**

**Funktioniert in:**

* Flussschritt [Datenwert ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}
* Flussschritt [interessanter Moment](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"}
* Workflow-Schritt [Aufgabe erstellen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}
* Der Textkörper einer E-Mail oder Vorlage

## system.dateTime {#system-datetime}

Das `{{system.dateTime}}` -Token gibt das aktuelle Datum und die aktuelle Uhrzeit zur Laufzeit wie folgt wieder: **2013-08-08 16:36:13**

**Funktioniert in:**

* Flussschritt [Datenwert ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"}
* Flussschritt [interessanter Moment](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"}
* Workflow-Schritt [Aufgabe erstellen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"}
* Der Textkörper einer E-Mail oder Vorlage

## system.forwardToFriendLink {#system-forwardtofriendlink}

Mit dem `{{system.forwardToFriendLink}}` -Token können Sie die Platzierung des [&#39;Weiterleiten an einen Freunde-Link&#39; in E-Mails](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/forward-to-a-friend-link-in-emails.md){target="_blank"} steuern.

**Funktioniert in:**

* [Hinzufügen eines System-Tokens als Link in einer E-Mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} oder Vorlage

## system.unsubscribeLink {#system-unsubscribelink}

Mit dem Token `{{system.unsubscribeLink}}` können Sie die Platzierung des Abmelde-Links in einer E-Mail steuern.

**Funktioniert in:**

* [Hinzufügen eines System-Tokens als Link in einer E-Mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} oder Vorlage

## system.viewAsWebpageLink {#system-viewaswebpagelink}

Mit dem `{{system.viewAsWebpageLink}}` -Token können Sie die Platzierung des Links Als Webseite anzeigen in einer E-Mail steuern.

**Funktioniert mit:**

* [Hinzufügen eines System-Tokens als Link in einer E-Mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} oder Vorlage
