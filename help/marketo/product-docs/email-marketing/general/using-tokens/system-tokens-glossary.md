---
unique-page-id: 1147344
description: Glossar zu System-Token - Marketo-Dokumente - Produktdokumentation
title: Glossar zu System-Token
exl-id: 8a7694af-4edb-4b32-b408-19d2e7bd596e
feature: Tokens
source-git-commit: bf420edcc79aa551e286302fa002df9162371873
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 2%

---

# Glossar zu System-Token {#system-tokens-glossary}

Zusätzlich zu Personen-Token können Sie einige wirklich coole System-Token verwenden. Hier sind sie.

>[!NOTE]
>
>Die Einstellungen der Zeitzone Ihres Kontos wirken sich darauf aus, wann Datums- und Uhrzeit-Token ausgeführt werden.

## system.date {#system-date}

Das `{{system.date}}`-Token rendert das aktuelle Datum zur Laufzeit wie folgt: **8. August 2013**

**Funktioniert in:**

* [Datenwert ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} Flussschritt
* [Interessanter Moment](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"} Flussschritt
* [Aufgabe erstellen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} Flussschritt
* Der Textkörper einer E-Mail oder Vorlage

## system.time {#system-time}

Das `{{system.time}}`-Token rendert die aktuelle Uhrzeit zur Laufzeit wie folgt: **04:34 PM (GMT -0700)**

**Funktioniert in:**

* [Datenwert ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} Flussschritt
* [Interessanter Moment](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"} Flussschritt
* [Aufgabe erstellen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} Flussschritt
* Der Textkörper einer E-Mail oder Vorlage

## system.dateTime {#system-datetime}

Das `{{system.dateTime}}`-Token rendert das aktuelle Datum und die aktuelle Uhrzeit zur Laufzeit wie folgt: **2013-08-08 16:36:13**

**Funktioniert in:**

* [Datenwert ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} Flussschritt
* [Interessanter Moment](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"} Flussschritt
* [Aufgabe erstellen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} Flussschritt
* Der Textkörper einer E-Mail oder Vorlage

## system.unsubscribeLink {#system-unsubscribelink}

Mit dem `{{system.unsubscribeLink}}`-Token können Sie die Platzierung des Abmelde-Links in einer E-Mail steuern.

**Funktioniert in:**

* [Hinzufügen eines System-Tokens als Link in einer E](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"}Mail oder Vorlage

## system.viewAsWebpageLink {#system-viewaswebpagelink}

Mit dem `{{system.viewAsWebpageLink}}`-Token können Sie die Platzierung des Links Als Web-Seite anzeigen in einer E-Mail steuern.

**Funktioniert mit:**

* [Hinzufügen eines System-Tokens als Link in einer E](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"}Mail oder Vorlage
