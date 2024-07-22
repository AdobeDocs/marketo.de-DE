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

Dynamische Felder funktionieren nur, wenn Sie eine Vorlage verwenden. Einzelne einmalige E-Mails, die Sie schreiben, werden diese nicht ausfüllen.

## Was zu überprüfen ist {#what-to-check}

Es gibt drei Arten dynamischer Felder in Sales Insight-Aktionen: Einfach, Benutzerdefiniert und Salesforce. Sowohl die einfache als auch die benutzerdefinierte Ansicht sehen so aus, dass Informationen aus der [Webanwendung](https://toutapp.com/login){target="_blank"} abgerufen werden. Wenn die Informationen nicht in der Webanwendung vorhanden sind, sind die Felder leer. Salesforce-Felder rufen Informationen von [Salesforce.com](https://salesforce.com){target="_blank"} ab.

**Fehlerbehebung bei Salesforce-Feldern**

Salesforce-Felder: z. B. `{{sfdc_account_name}}`

* Stellen Sie sicher, dass es ordnungsgemäß mit Sales Insight-Aktionen verbunden ist. Rufen Sie die Seite [Einstellungen](https://toutapp.com/login{target="_blank"} auf und klicken Sie neben Ihrem CRM-System auf **Verwalten** .

**Fehlerbehebung bei einfachen und benutzerdefinierten Feldern**

Marketo Sales Insight-Aktionen - Grundlegende Felder, z. B. `{{company}}`

Benutzerdefinierte Felder für Marketo Sales Insight-Aktionen, z. B. `{{custom_field_favorite_movie}}`

* Das entsprechende Feld muss für Ihren Kontakt auf der Seite [Personen](https://toutapp.com/next#relationships){target="_blank"} gespeichert werden, damit unser dynamisches Feld darauf verweist. Wenn Sie beispielsweise eine E-Mail an Maria senden und das Feld `{{company}}` verwenden, ihr Kontaktdatensatz jedoch keine Firma auflistet, können wir dies nicht ausfüllen.

## Warum hat meine E-Mail gesendet, ohne alle dynamischen Felder zu füllen? {#why-did-my-email-send-without-populating-all-dynamic-fields}

Sales Insight-Aktionen verhindern den Versand Ihrer E-Mails, wenn nicht alle dynamischen Felder in der E-Mail ausgefüllt werden können. **Allerdings** gibt es einige Ausnahmen von dieser Regel. Einige Felder werden leer gesendet oder automatisch ausgefüllt, wenn ein Wert gefunden werden kann. Diese Felder und wie sie reagieren, wenn sie das Feld nicht ausfüllen können, sind unten aufgeführt.

`{{first_name}}` = BLANK

`{{last_name}}` =BLANK

`{{title}}` = BLANK

`{{company}}` = &quot;Ihr Unternehmen&quot;

`{{friendly_company}}` = &quot;Ihr Unternehmen&quot;

>[!NOTE]
>
>Das Feld `{{first_name}}` sucht sowohl in Sales Insight-Aktionen als auch in Salesforce nach dem Versuch, Informationen abzurufen. Alle anderen Felder in dieser Liste suchen nur nach Sales Insight-Aktionen , um das Feld zu füllen.
