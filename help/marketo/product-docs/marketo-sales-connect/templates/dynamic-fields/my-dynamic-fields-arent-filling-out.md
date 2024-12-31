---
unique-page-id: 14352602
description: Meine dynamischen Felder werden nicht ausgefüllt - Marketo-Dokumente - Produktdokumentation
title: Meine dynamischen Felder werden nicht ausgefüllt
exl-id: fb3e8b56-506a-41f8-a84f-41370381c058
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Meine dynamischen Felder werden nicht ausgefüllt {#my-dynamic-fields-arent-filling-out}

Dynamische Felder funktionieren nur, wenn Sie eine Vorlage verwenden. Einzelne einmalige E-Mails, die Sie schreiben, füllen diese nicht aus.

## Was zu überprüfen ist {#what-to-check}

Es gibt drei Arten von dynamischen Feldern in Sales Connect: „Basic“, „Custom“ und &quot;Salesforce&quot;. Sowohl einfache als auch benutzerdefinierte Elemente sehen so aus, dass Informationen aus der [Web-Anwendung“ abgerufen ](https://toutapp.com/login). Wenn die Informationen nicht in der Web-Anwendung vorhanden sind, sind die Felder leer. Salesforce-Felder rufen Informationen von [Salesforce.com](https://salesforce.com) ab.

**Fehlerbehebung bei Salesforce-Feldern**

Salesforce-Felder: z. B. `{{sfdc_account_name}}`

* Stellen Sie sicher, dass die Verbindung ordnungsgemäß mit Sales Connect hergestellt wird. Navigieren Sie zur Seite [Einstellungen](https://toutapp.com/login) und klicken Sie **Verwalten** neben Ihrem CRM.

**Fehlerbehebung bei grundlegenden und benutzerdefinierten Feldern**

Tout Basic Fields: z.B. `{{company}}`

Tout Benutzerdefinierte Felder: z. B. `{{custom_field_favorite_movie}}`

* Das entsprechende Feld muss für Ihren Kontakt auf der Seite „Personen[ gespeichert werden, ](https://toutapp.com/next#relationships) unser dynamisches Feld referenzieren zu können. Wenn Sie beispielsweise eine E-Mail an Mary senden und das Feld `{{company}}` verwenden, in ihrem Kontaktdatensatz jedoch keine Firma aufgeführt ist, können wir dies nicht ausfüllen.

## Warum wurde meine E-Mail gesendet, ohne alle dynamischen Felder auszufüllen? {#why-did-my-email-send-without-populating-all-dynamic-fields}

Sales Connect verhindert den Versand Ihrer E-Mails, wenn wir nicht alle Ihre dynamischen Felder in der E-Mail ausfüllen können. **Es** jedoch einige Ausnahmen von dieser Regel. Einige Felder werden leer gesendet oder automatisch einen Wert ausgefüllt, falls wir einen finden können. Diese Felder und wie sie reagieren, wenn sie das Feld nicht ausfüllen können, sind unten aufgeführt.

`{{first_name}}` = LEER

`{{last_name}}` = LEER

`{{title}}` = LEER

`{{company}}` = „Ihre Firma“

`{{friendly_company}}` = „Ihre Firma“

>[!NOTE]
>
>Das Feld `{{first_name}}` wird sowohl in Sales Connect als auch in Salesforce angezeigt, um zu versuchen, Informationen abzurufen. Alle anderen Felder in dieser Liste werden nur in Sales Connect berücksichtigt, um das Feld auszufüllen.
