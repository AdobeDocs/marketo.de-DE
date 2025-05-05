---
description: Warum werden meine dynamischen Felder nicht ausgefüllt? - Marketo-Dokumente - Produktdokumentation
title: Warum werden meine dynamischen Felder nicht ausgefüllt?
exl-id: 4e1d133f-8314-4e64-b50b-f3e824c3bef4
feature: Sales Insight Actions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Warum werden meine dynamischen Felder nicht ausgefüllt? {#why-arent-my-dynamic-fields-filling-out}

Dynamische Felder funktionieren nur, wenn Sie eine Vorlage verwenden. Einzelne einmalige E-Mails, die Sie schreiben, füllen diese nicht aus.

## Was zu überprüfen ist {#what-to-check}

Es gibt drei Arten von dynamischen Feldern in Sales-Insight-Aktionen: „Standard“, „Benutzerdefiniert“ und &quot;Salesforce&quot;. Sowohl einfache als auch benutzerdefinierte Elemente sehen so aus, dass Informationen aus der [Web-Anwendung“ abgerufen ](https://toutapp.com/login){target="_blank"}. Wenn die Informationen nicht in der Web-Anwendung vorhanden sind, sind die Felder leer. Salesforce-Felder rufen Informationen von [Salesforce.com](https://salesforce.com){target="_blank"} ab.

**Fehlerbehebung bei Salesforce-Feldern**

Salesforce-Felder: z. B. `{{sfdc_account_name}}`

* Stellen Sie sicher, dass sie ordnungsgemäß mit Sales Insight-Aktionen verbunden ist. Navigieren Sie zur Seite [Einstellungen] (https://toutapp.com/login{target="_blank"} und klicken Sie auf **Verwalten** neben Ihrem CRM.

**Fehlerbehebung bei grundlegenden und benutzerdefinierten Feldern**

Grundlegende Felder für Marketo Sales Insight-Aktionen: z. B. `{{company}}`

Benutzerdefinierte Felder für Marketo Sales Insight-Aktionen: z. B. `{{custom_field_favorite_movie}}`

* Das entsprechende Feld muss für Ihren Kontakt auf der Seite „Personen[ gespeichert werden, ](https://toutapp.com/next#relationships){target="_blank"} unser dynamisches Feld referenzieren zu können. Wenn Sie beispielsweise eine E-Mail an Mary senden und das Feld `{{company}}` verwenden, in ihrem Kontaktdatensatz jedoch keine Firma aufgeführt ist, können wir dies nicht ausfüllen.

## Warum wurde meine E-Mail gesendet, ohne alle dynamischen Felder auszufüllen? {#why-did-my-email-send-without-populating-all-dynamic-fields}

Sales Insight-Aktionen verhindern den Versand Ihrer E-Mails, wenn nicht alle dynamischen Felder in der E-Mail ausgefüllt werden können. **Es** jedoch einige Ausnahmen von dieser Regel. Einige Felder werden leer gesendet oder automatisch einen Wert ausgefüllt, falls wir einen finden können. Diese Felder und wie sie reagieren, wenn sie das Feld nicht ausfüllen können, sind unten aufgeführt.

`{{first_name}}` = LEER

`{{last_name}}` = LEER

`{{title}}` = LEER

`{{company}}` = „Ihre Firma“

`{{friendly_company}}` = „Ihre Firma“

>[!NOTE]
>
>Das Feld `{{first_name}}` wird sowohl in Sales Insight-Aktionen als auch in Salesforce angezeigt, um zu versuchen, Informationen abzurufen. Alle anderen Felder in dieser Liste werden nur in Sales Insight-Aktionen untersucht, um das Feld auszufüllen.
