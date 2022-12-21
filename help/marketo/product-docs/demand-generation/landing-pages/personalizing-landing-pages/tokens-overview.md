---
unique-page-id: 2950799
description: Token-Übersicht - Marketo-Dokumente - Produktdokumentation
title: Token-Übersicht
exl-id: d60816ce-33fb-4e18-8acd-71d4e90f47de
source-git-commit: 4fc3cf6e6458f07df7cced9399831b8c6b50e0ad
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 1%

---

# Token-Übersicht {#tokens-overview}

Ein Token ist eine Variable, die in Marketo-Schritten zum Fluss intelligenter Kampagnen, E-Mails, Landingpages, Snippets und Webkampagnen verwendet werden kann.

## Grundlegendes zu Standardwerten {#understanding-default-values}

Wenn Sie ein Token verwenden, möchten Sie auch einen Standardwert bereitstellen. Dies ist der Text, der anzeigt, ob eine Person keinen Wert für das Feld hat, auf das Sie verweisen.

![](assets/image2014-12-2-13-3a16-3a48.png)

In diesem Beispiel lautet die E-Mail &quot;Grußformeln, (Vorname)&quot;oder &quot;Grußformeln, Erdling&quot;(Standardwert).

![](assets/two.png)

>[!CAUTION]
>
>Token funktionieren im Preheader nicht, wenn der E-Mail-Editor von Marketo verwendet wird. Um ein Token im Preheader zu verwenden, muss es über Ihre eigene HTML in einer E-Mail-Vorlage sein.

>[!NOTE]
>
>Diese Liste ist nicht vollständig. Token werden auch für jedes benutzerdefinierte Feld erstellt, das Sie in Marketo haben.

## Personen-Token {#person-tokens}

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
* Benutzerdefinierte Personenfelder funktionieren auch, wenn Sie beispielsweise ihren Anzeigenamen verwenden. `{{lead.Custom Field Name}}`

## Firmen-Token {#company-tokens}

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
* Benutzerdefinierte Unternehmensfelder funktionieren auch, wenn Sie z. B. ihren Anzeigenamen verwenden. `{{Company.Custom Field Name}}`

## Kampagnen-Token {#campaign-tokens}

* `{{campaign.name}}`
* `{{campaign.id}}`
* `{{campaign.description}}`

## System-Token {#system-tokens}

>[!NOTE]
>
>Weitere Informationen zu diesen Token finden Sie im Abschnitt [Glossar zu System-Token](/help/marketo/product-docs/email-marketing/general/using-tokens/system-tokens-glossary.md).

* `{{system.date}}`
* `{{system.time}}`
* `{{system.dateTime}}`
* `{{system.forwardToFriendLink}}`
* `{{system.unsubscribeLink}}`
* `{{system.viewAsWebpageLink}}`

## Trigger-Token {#trigger-tokens}

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
>Weitere Informationen finden Sie unter [Token für interessante Momente](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md) basierend auf Triggern, die in einer Smart-Kampagne verwendet werden.

## Programm-Token {#program-tokens}

* `{{program.Name}}`
* `{{program.Description}}`
* `{{program.id}}`

## Meine Token {#my-tokens}

Meine Token werden in einem Programm definiert und beginnen mit `{{my.` gefolgt von dem Namen, den Sie für das Token erstellt haben. Weitere Informationen [Meine Token in einem Programm](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md).

## Member Token {#member-token}

Member Tokens werden verwendet, um eindeutige Werte von integrierten Servicepartnern einzufügen. Eine gängige Verwendung von Mitglieds-Token ist für eindeutige URLs für Webinar-Teilnehmer. Jede Person verfügt über eine eindeutige URL für den Zugriff auf das Webinar, die mithilfe einer `{{member.webinar url}}` Token. Die `{{member.webinar url}}` -Token löst automatisch die eindeutige Bestätigungs-URL der Person auf, die vom Dienstleister generiert wurde.

* `{{member.webinar url}}`

>[!CAUTION]
>
>Die `{{member.webinar url}}` Token wird nur dann aufgefüllt, wenn die Smart-Kampagne, die die E-Mail sendet, ein untergeordnetes Asset des Ereignisprogramms ist.
