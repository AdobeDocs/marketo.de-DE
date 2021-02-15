---
unique-page-id: 14352602
description: Meine dynamischen Felder füllen nicht aus - Marketing Docs - Produktdokumentation
title: Meine dynamischen Felder sind nicht ausgefüllt
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 0%

---


# Meine dynamischen Felder füllen nicht aus {#my-dynamic-fields-arent-filling-out}

Dynamische Felder funktionieren nur, wenn Sie eine Vorlage verwenden. Einzelne einmalige E-Mails, die Sie schreiben, werden diese nicht ausfüllen.

## Was zu überprüfen ist {#what-to-check}

Es gibt drei Arten dynamischer Felder in Sales Connect: Basic, Custom und Salesforce. Sowohl Standard als auch Benutzerdefiniert suchen, um Informationen aus der [Webanwendung](https://toutapp.com/login) abzurufen. Wenn die Informationen in der Webanwendung nicht vorhanden sind, sind die Felder leer. Salesforce-Felder rufen Informationen von [Salesforce.com](https://salesforce.com) ab.

**Fehlerbehebung bei Salesforce-Feldern**

Salesforce-Felder: z. B. `{{sfdc_account_name}}`

* Vergewissern Sie sich, dass es ordnungsgemäß mit Sales Connect verbunden ist. Gehen Sie zur Seite [Einstellungen](https://toutapp.com/login) und klicken Sie auf **Verwalten** neben Ihrem CRM.

**Fehlerbehebung bei einfachen und benutzerdefinierten Feldern**

Tout-Grundfelder: z. B. `{{company}}`

Tout Custom Fields: z. B. `{{custom_field_favorite_movie}}`

* Das entsprechende Feld muss für Ihren Kontakt auf der Seite [Personen](https://toutapp.com/next#relationships) gespeichert werden, damit unser dynamisches Feld referenziert werden kann. Wenn Sie beispielsweise eine E-Mail an Maria senden und das Feld `{{company}}` verwenden, ihr Kontaktdatensatz jedoch keine Firma Liste, können wir das nicht ausfüllen.

## Warum hat meine E-Mail gesendet, ohne alle dynamischen Felder auszufüllen? {#why-did-my-email-send-without-populating-all-dynamic-fields}

Sales Connect verhindert, dass Ihre E-Mails gesendet werden, wenn nicht alle dynamischen Felder in der E-Mail ausgefüllt werden können. **Es gibt jedoch** einige Ausnahmen von dieser Regel. Einige Felder werden leer gesendet oder automatisch mit einem Wert gefüllt, wenn einer gefunden wird. Diese Felder und wie sie reagieren, wenn sie das Feld nicht füllen können, sind unten aufgeführt.

`{{first_name}}` = BLANK

`{{last_name}}` =BLANK

`{{title}}` = BLANK

`{{company}}` = &quot;Ihre Firma&quot;

`{{friendly_company}}` = &quot;Ihre Firma&quot;

>[!NOTE]
>
>Das Feld `{{first_name}}` sucht sowohl in Sales Connect als auch in Salesforce nach Informationen. Alle anderen Felder in dieser Liste suchen nur in Sales Connect, um das Feld auszufüllen.
