---
unique-page-id: 1147344
description: System Tokens-Glossar - Marketo Docs - Produktdokumentation
title: Glossar zu System-Token
exl-id: 8a7694af-4edb-4b32-b408-19d2e7bd596e
feature: Tokens
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# Glossar zu System-Token {#system-tokens-glossary}

Neben Personen-Token können Sie auch einige wirklich coole System-Token verwenden. Hier sind sie.

>[!NOTE]
>
>Die Zeitzoneneinstellungen Ihres Kontos wirken sich auf die Ausführung von Datums- und Uhrzeit-Token aus.

## system.date {#system-date}

Die `{{system.date}}` -Token rendert das aktuelle Datum zur Laufzeit wie folgt: **8. August 2013**

**Funktioniert in:**

* [Datenwert ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} Flussschritt
* [Interessanter Moment](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"} Flussschritt
* [Aufgabe erstellen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} Flussschritt
* Der Textkörper einer E-Mail oder Vorlage

## system.time {#system-time}

Die `{{system.time}}` -Token rendert die aktuelle Zeit zur Laufzeit wie folgt: **16:34 (GMT -0700)**

**Funktioniert in:**

* [Datenwert ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} Flussschritt
* [Interessanter Moment](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"} Flussschritt
* [Aufgabe erstellen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} Flussschritt
* Der Textkörper einer E-Mail oder Vorlage

## system.dateTime {#system-datetime}

Die `{{system.dateTime}}` -Token rendert das aktuelle Datum und die aktuelle Uhrzeit zur Laufzeit wie folgt: **08.08.2013 16:36:13**

**Funktioniert in:**

* [Datenwert ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} Flussschritt
* [Interessanter Moment](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"} Flussschritt
* [Aufgabe erstellen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} Flussschritt
* Der Textkörper einer E-Mail oder Vorlage

## system.forwardToFriendLink {#system-forwardtofriendlink}

Die `{{system.forwardToFriendLink}}` Mit token können Sie die Platzierung der [&quot;Weiterleiten an einen Freunde-Link&quot;in E-Mails](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/forward-to-a-friend-link-in-emails.md){target="_blank"}.

**Funktioniert in:**

* [Hinzufügen eines System-Tokens als Link in einer E-Mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} oder Vorlage

## system.unsubscribeLink {#system-unsubscribelink}

Die `{{system.unsubscribeLink}}` Mit token können Sie die Platzierung des Abmelde-Links in einer E-Mail steuern.

**Funktioniert in:**

* [Hinzufügen eines System-Tokens als Link in einer E-Mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} oder Vorlage

## system.viewAsWebpageLink {#system-viewaswebpagelink}

Die `{{system.viewAsWebpageLink}}` Mit dem -Token können Sie die Platzierung des Links Als Webseite anzeigen in einer E-Mail steuern.

**Funktioniert mit:**

* [Hinzufügen eines System-Tokens als Link in einer E-Mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} oder Vorlage
