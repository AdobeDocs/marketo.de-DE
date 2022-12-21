---
description: Warum werden meine dynamischen Felder nicht ausgefüllt - Marketo Docs - Produktdokumentation
title: Warum werden meine dynamischen Felder nicht ausgefüllt?
hide: true
hidefromtoc: true
exl-id: 4e1d133f-8314-4e64-b50b-f3e824c3bef4
source-git-commit: f77a076c243c25f3bff98a82751f51c464712795
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 1%

---

# Warum werden meine dynamischen Felder nicht ausgefüllt? {#why-arent-my-dynamic-fields-filling-out}

Dynamische Felder funktionieren nur, wenn Sie eine Vorlage verwenden. Einzelne einmalige E-Mails, die Sie schreiben, werden diese nicht ausfüllen.

## Was zu überprüfen ist {#what-to-check}

Es gibt drei Arten dynamischer Felder in Sales Insight-Aktionen: Basic, Custom und Salesforce. Sowohl die grundlegende als auch die benutzerdefinierte Ansicht verwenden Informationen aus der [Webanwendung](https://toutapp.com/login). Wenn die Informationen nicht in der Webanwendung vorhanden sind, sind die Felder leer. Salesforce-Felder rufen Informationen ab von [Salesforce.com](https://salesforce.com).

**Fehlerbehebung bei Salesforce-Feldern**

Salesforce-Felder: z. B. `{{sfdc_account_name}}`

* Stellen Sie sicher, dass es ordnungsgemäß mit Sales Insight-Aktionen verbunden ist. Navigieren Sie zu [Einstellungen](https://toutapp.com/login) Seite und klicken Sie auf **Verwalten** neben Ihrem CRM.

**Fehlerbehebung für einfache und benutzerdefinierte Felder**

Tout Basic Fields: z. B. `{{company}}`

Festlegen benutzerdefinierter Felder: z. B. `{{custom_field_favorite_movie}}`

* Das entsprechende Feld muss für Ihren Kontakt im [Personenseite](https://toutapp.com/next#relationships) für unser dynamisches Feld zu referenzieren. Wenn Sie beispielsweise eine E-Mail an Maria senden und die Variable `{{company}}` -Feld, aber ihr Kontaktdatensatz listet kein Unternehmen auf, wir können das nicht ausfüllen.

## Warum hat meine E-Mail gesendet, ohne alle dynamischen Felder zu füllen? {#why-did-my-email-send-without-populating-all-dynamic-fields}

Sales Insight-Aktionen verhindern den Versand Ihrer E-Mails, wenn nicht alle dynamischen Felder in der E-Mail ausgefüllt werden können. **Jedoch** gibt es einige Ausnahmen von dieser Regel. Einige Felder werden leer gesendet oder automatisch ausgefüllt, wenn ein Wert gefunden werden kann. Diese Felder und wie sie reagieren, wenn sie das Feld nicht ausfüllen können, sind unten aufgeführt.

`{{first_name}}` = BLANK

`{{last_name}}` =BLANK

`{{title}}` = BLANK

`{{company}}` = &quot;Ihr Unternehmen&quot;

`{{friendly_company}}` = &quot;Ihr Unternehmen&quot;

>[!NOTE]
>
>Die `{{first_name}}` -Feld sucht sowohl in Sales Insight-Aktionen als auch in Salesforce nach dem Versuch, Informationen abzurufen. Alle anderen Felder in dieser Liste suchen nur nach Sales Insight-Aktionen , um das Feld zu füllen.
