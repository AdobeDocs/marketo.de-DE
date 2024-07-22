---
unique-page-id: 14352602
description: Meine dynamischen Felder werden nicht ausgefüllt - Marketo Docs - Produktdokumentation
title: Meine dynamischen Felder werden nicht ausgefüllt
exl-id: fb3e8b56-506a-41f8-a84f-41370381c058
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Meine dynamischen Felder werden nicht ausgefüllt {#my-dynamic-fields-arent-filling-out}

Dynamische Felder funktionieren nur, wenn Sie eine Vorlage verwenden. Einzelne einmalige E-Mails, die Sie schreiben, werden diese nicht ausfüllen.

## Was zu überprüfen ist {#what-to-check}

In Sales Connect gibt es drei Arten dynamischer Felder: Einfach, Benutzerdefiniert und Salesforce. Sowohl die einfache als auch die benutzerdefinierte Ansicht sehen so aus, dass Informationen aus der [Webanwendung](https://toutapp.com/login) abgerufen werden. Wenn die Informationen nicht in der Webanwendung vorhanden sind, sind die Felder leer. Salesforce-Felder rufen Informationen von [Salesforce.com](https://salesforce.com) ab.

**Fehlerbehebung bei Salesforce-Feldern**

Salesforce-Felder: z. B. `{{sfdc_account_name}}`

* Stellen Sie sicher, dass es ordnungsgemäß mit Sales Connect verbunden ist. Gehen Sie zur Seite [Einstellungen](https://toutapp.com/login) und klicken Sie neben Ihrem CRM-System auf **Verwalten** .

**Fehlerbehebung bei einfachen und benutzerdefinierten Feldern**

Tout Basic Fields: z. B. `{{company}}`

Festlegen benutzerdefinierter Felder: z. B. `{{custom_field_favorite_movie}}`

* Das entsprechende Feld muss für Ihren Kontakt auf der Seite [Personen](https://toutapp.com/next#relationships) gespeichert werden, damit unser dynamisches Feld darauf verweist. Wenn Sie beispielsweise eine E-Mail an Maria senden und das Feld `{{company}}` verwenden, ihr Kontaktdatensatz jedoch keine Firma auflistet, können wir dies nicht ausfüllen.

## Warum hat meine E-Mail gesendet, ohne alle dynamischen Felder zu füllen? {#why-did-my-email-send-without-populating-all-dynamic-fields}

Sales Connect stoppt den Versand Ihrer E-Mails, wenn nicht alle dynamischen Felder in der E-Mail ausgefüllt werden können. **Allerdings** gibt es einige Ausnahmen von dieser Regel. Einige Felder werden leer gesendet oder automatisch ausgefüllt, wenn ein Wert gefunden werden kann. Diese Felder und wie sie reagieren, wenn sie das Feld nicht ausfüllen können, sind unten aufgeführt.

`{{first_name}}` = BLANK

`{{last_name}}` =BLANK

`{{title}}` = BLANK

`{{company}}` = &quot;Ihr Unternehmen&quot;

`{{friendly_company}}` = &quot;Ihr Unternehmen&quot;

>[!NOTE]
>
>Das Feld `{{first_name}}` sucht sowohl in Sales Connect als auch in Salesforce nach dem Versuch, Informationen abzurufen. Alle anderen Felder in dieser Liste suchen nur in Sales Connect, um das Feld auszufüllen.
