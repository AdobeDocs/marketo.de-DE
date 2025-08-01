---
unique-page-id: 2950799
description: Token-Übersicht - Marketo-Dokumente - Produktdokumentation
title: Token-Übersicht
exl-id: d60816ce-33fb-4e18-8acd-71d4e90f47de
feature: Landing Pages
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 0%

---

# Token-Übersicht {#tokens-overview}

Ein Token ist eine Variable, die in Marketo Smart Campaign-Flussschritten, E-Mails, Landingpages, Snippets und Web-Kampagnen verwendet werden kann.

## Grundlegendes zu Standardwerten {#understanding-default-values}

Wenn Sie ein Token verwenden, möchten Sie auch einen Standardwert angeben. Dies ist der Text, der anzeigt, wenn eine Person keinen Wert für das Feld hat, auf das Sie verweisen.

![](assets/image2014-12-2-13-3a16-3a48.png)

In diesem Beispiel lautet die E-Mail „Grußformeln, (Vorname)“ oder „Grußformeln, Erdling“ (Standardwert).

![](assets/two.png)

>[!CAUTION]
>
>Token funktionieren nicht im Preheader, wenn Sie den E-Mail-Editor von Marketo verwenden. Um ein Token im Preheader zu verwenden, muss dies über Ihre eigene HTML in einer E-Mail-Vorlage erfolgen.

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
* Benutzerdefinierte Personenfelder funktionieren auch, wenn Sie ihren Anzeigenamen verwenden, z. B. `{{lead.Custom Field Name}}`

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
* Benutzerdefinierte Unternehmensfelder funktionieren auch, wenn Sie ihren Anzeigenamen verwenden (z. B. `{{Company.Custom Field Name}}`

## Kampagnen-Token {#campaign-tokens}

* `{{campaign.name}}`
* `{{campaign.id}}`
* `{{campaign.description}}`

## System-Token {#system-tokens}

>[!NOTE]
>
>Weitere Informationen zu diesen Token finden Sie im [Glossar zu System-Token](/help/marketo/product-docs/email-marketing/general/using-tokens/system-tokens-glossary.md).

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
>Erfahren Sie mehr über [Token für interessante Momente](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/tabs-in-the-msi-panel/interesting-moments/trigger-tokens-for-interesting-moments.md) die auf den in einer Smart-Kampagne verwendeten Triggern basieren.

## Programm-Token {#program-tokens}

* `{{program.Name}}`
* `{{program.Description}}`
* `{{program.id}}`

## [!UICONTROL Meine Token] {#my-tokens}

[!UICONTROL Meine Token] werden in einem Programm definiert und beginnen mit `{{my.` gefolgt vom Namen, den Sie für das Token erstellt haben. Erfahren Sie mehr über [Meine Token in einem Programm](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/understanding-my-tokens-in-a-program.md).

## Mitglieds-Token {#member-token}

Mitglieder-Token werden verwendet, um eindeutige Werte von integrierten Service-Partnern einzufügen. Mitglieder-Token werden häufig für eindeutige URLs für Webinar-Teilnehmer verwendet. Jede Person verfügt über eine eindeutige URL für den Zugriff auf das Webinar, die mithilfe eines `{{member.webinar url}}`-Tokens eingefügt werden kann. Das `{{member.webinar url}}`-Token löst automatisch die eindeutige Bestätigungs-URL der Person auf, die vom Dienstleister generiert wurde.

* `{{member.webinar url}}`

>[!CAUTION]
>
>Das `{{member.webinar url}}`-Token wird nur aufgefüllt, wenn die Smart-Kampagne, die die E-Mail sendet, ein untergeordnetes Asset des Ereignisprogramms ist.
