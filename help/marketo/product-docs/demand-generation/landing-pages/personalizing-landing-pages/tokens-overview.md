---
unique-page-id: 2950799
description: Tokens - Übersicht - Marketo Docs - Produktdokumentation
title: Tokens - Übersicht
exl-id: d60816ce-33fb-4e18-8acd-71d4e90f47de
translation-type: tm+mt
source-git-commit: 4fc3cf6e6458f07df7cced9399831b8c6b50e0ad
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 1%

---

# Token-Übersicht {#tokens-overview}

Ein Token ist eine Variable, die in Marketo-Flussschritten für intelligente Kampagnen, E-Mails, Landingpages, Snippets und Web-Kampagnen verwendet werden kann.

## Standardwerte {#understanding-default-values}

Wenn Sie ein Token verwenden, möchten Sie auch einen Standardwert angeben. Dieser Text zeigt an, ob eine Person keinen Wert für das Feld hat, auf das Sie verweisen.

![](assets/image2014-12-2-13-3a16-3a48.png)

In diesem Beispiel lautet die E-Mail &quot;Grüße, (Vorname)&quot;oder &quot;Grüße, Erdling&quot;(Standardwert).

![](assets/two.png)

>[!CAUTION]
>
>Tokens funktionieren nicht im Preheader, wenn der E-Mail-Editor von Marketo verwendet wird. Um ein Token im Preheader zu verwenden, muss es über Ihren eigenen HTML in einer E-Mail-Vorlage erfolgen.

>[!NOTE]
>
>Diese Liste ist nicht erschöpfend. Token werden auch für jedes benutzerdefinierte Feld erstellt, das Sie in Marketo haben.

## Person Tokens {#person-tokens}

* `{{lead.Acquisition Date}}`
* `{{lead.Acquisition Program Name}}`
* `{{lead.Acquisition Program}}`
* `{{lead.Address}}`
* `{{lead.Anonymous IP}}`
* `{{lead.Black Listed}}`
* `{{lead.City}}`
* `{{lead.Country}}`
* `{{lead.Created At}}`
* `{{lead.Date of Birth}}`
* `{{lead.Department}}`
* `{{lead.Do Not Call}}`
* `{{lead.Do Not Call Reason}}`
* `{{lead.Email Address}}`
* `{{lead.Email Invalid}}`
* `{{lead.Email Invalid Cause}}`
* `{{lead.Fax Number}}`
* `{{lead.First Name}}`
* `{{lead.Full Name}}`
* `{{lead.Id}}`
* `{{lead.Inferred City}}`
* `{{lead.Inferred Company}}`
* `{{lead.Inferred Country}}`
* `{{lead.Inferred Metropolitan Area}}`
* `{{lead.Inferred Phone Area Code}}`
* `{{lead.Inferred Postal Code}}`
* `{{lead.Inferred State Region}}`
* `{{lead.Is Customer}}`
* `{{lead.Is Employee}}`
* `{{lead.Is Partner}}`
* `{{lead.Job Title}}`
* `{{lead.Last Name}}`
* `{{lead.Lead Source}}`
* `{{lead.Marketing Suspended}}`
* `{{lead.Middle Name}}`
* `{{lead.Mobile Phone Number}}`
* `{{lead.Original Referrer}}`
* `{{lead.Original Search Engine}}`
* `{{lead.Original Search Phrase}}`
* `{{lead.Original Source Info}}`
* `{{lead.Original Source Type}}`
* `{{lead.Person Notes}}`
* `{{lead.Phone Number}}`
* `{{lead.Registration Source Info}}`
* `{{lead.Registration Source Type}}`
* `{{lead.Salutation}}`
* `{{lead.SFDC Created Date}}`
* `{{lead.SFDC Is Deleted}}`
* `{{lead.SFDC Type}}`
* `{{lead.Unsubscribed}}`
* `{{lead.Unsubscribed Reason}}`
* `{{lead.Updated At}}`
* Benutzerdefinierte Personenfelder funktionieren auch, wenn Sie ihren Anzeigenamen verwenden, z. B. `{{lead.Custom Field Name}}`

## Firma Tokens {#company-tokens}

* `{{Company.Account Owner Email Address}}`
* `{{Company.Address}}`
* `{{Company.Annual Revenue}}`
* `{{Company.City}}`
* `{{Company.Company Name}}`
* `{{Company.Company Notes}}`
* `{{Company.Country}}`
* `{{Company.Industry}}`
* `{{Company.Main Phone}}`
* `{{Company.Num Employees}}`
* `{{Company.Parent Company Name}}`
* `{{Company.Postal Code}}`
* `{{Company.SFDC Account Num}}`
* `{{Company.SFDC Created Date}}`
* `{{Company.SFDC Type}}`
* `{{Company.SIC Code}}`
* `{{Company.Site}}`
* `{{Company.State}}`
* `{{Company.Website}}`
* Benutzerdefinierte Firmen funktionieren auch, wenn Sie den Anzeigenamen z. B. verwenden. `{{Company.Custom Field Name}}`

## Kampagne Tokens {#campaign-tokens}

* `{{campaign.name}}`
* `{{campaign.id}}`
* `{{campaign.description}}`

## System-Tokens {#system-tokens}

>[!NOTE]
>
>Weitere Informationen zu diesen Token finden Sie im Glossar [SystemToken](/help/marketo/product-docs/email-marketing/general/using-tokens/system-tokens-glossary.md).

* `{{system.date}}`
* `{{system.time}}`
* `{{system.dateTime}}`
* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

## Trigger-Tokens {#trigger-tokens}

* `{{trigger.Trigger Name}}`
* `{{trigger.Name}}`
* `{{trigger.Link}}`
* `{{trigger.Subject}}`
* `{{trigger.Category}}`
* `{{trigger.Details}}`
* `{{trigger.Web Page}}`
* `{{trigger.Client IP Address}}`
* `{{trigger.Sent By}}`
* `{{trigger.Received By}}`
* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!NOTE]
>
>Weitere Informationen zu [Token für interessante Momente](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md) finden Sie auf der Grundlage von Triggern, die in einer intelligenten Kampagne verwendet werden.

## Programm-Token {#program-tokens}

* `{{program.Name}}`
* `{{program.Description}}`
* `{{program.id}}`

## Meine Token {#my-tokens}

Meine Token werden in einem Programm definiert und beginnen mit `{{my.`, gefolgt vom Namen, den Sie für das Token erstellt haben. Erfahren Sie mehr über [Meine Token in einem Programm](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md).

## Member Token {#member-token}

Member Tokens werden verwendet, um eindeutige Werte von integrierten Servicepartnern einzufügen. Eine häufige Verwendung von Mitglieds-Tokens ist für eindeutige URLs für Webinar-Teilnehmer. Jede Person hat eine eindeutige URL, um auf das Webinar zuzugreifen, das mit einem `{{member.webinar url}}`-Token eingefügt werden kann. Das Token `{{member.webinar url}}` löst automatisch die vom Dienstleister generierte eindeutige Bestätigungs-URL der Person auf.

* `{{member.webinar url}}`

>[!CAUTION]
>
>Das Token `{{member.webinar url}}` wird nur gefüllt, wenn die intelligente Kampagne, die die E-Mail sendet, ein untergeordnetes Asset des Ereignis-Programms ist.
