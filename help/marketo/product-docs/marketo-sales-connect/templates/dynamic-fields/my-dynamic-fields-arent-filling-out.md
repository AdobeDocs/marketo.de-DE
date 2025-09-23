---
unique-page-id: 14352602
description: Meine dynamischen Felder werden nicht ausgefüllt - Marketo-Dokumente - Produktdokumentation
title: Meine dynamischen Felder werden nicht ausgefüllt
exl-id: fb3e8b56-506a-41f8-a84f-41370381c058
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 4%

---

# Meine dynamischen Felder werden nicht ausgefüllt {#my-dynamic-fields-arent-filling-out}

Dynamische Felder funktionieren nur, wenn Sie eine Vorlage verwenden. Einzelne einmalige E-Mails, die Sie schreiben, füllen diese nicht aus.

## Was zu überprüfen ist {#what-to-check}

In [!DNL Sales Connect] gibt es drei Arten von dynamischen Feldern: „Standard“, „Benutzerdefiniert“ und &quot;[!DNL Salesforce]&quot;. Sowohl einfache als auch benutzerdefinierte Elemente sehen so aus, dass Informationen aus der [Web-Anwendung“ abgerufen ](https://toutapp.com/login). Wenn die Informationen nicht in der Web-Anwendung vorhanden sind, sind die Felder leer. [!DNL Salesforce] Felder rufen Informationen von [Salesforce.com](https://salesforce.com) ab.

**Fehlerbehebung bei [!DNL Salesforce] Feldern**

[!DNL Salesforce] Felder: z. B. `{{sfdc_account_name}}`

* Vergewissern Sie sich, dass es richtig mit [!DNL Sales Connect] verbunden ist. Navigieren Sie zur Seite [Einstellungen](https://toutapp.com/login) und klicken Sie **[!UICONTROL Verwalten]** neben Ihrem CRM.

**Fehlerbehebung bei grundlegenden und benutzerdefinierten Feldern**

Tout Basic Fields: z.B. `{{company}}`

Tout Benutzerdefinierte Felder: z. B. `{{custom_field_favorite_movie}}`

* Das entsprechende Feld muss für Ihren Kontakt auf der Seite „Personen[ gespeichert werden, ](https://toutapp.com/next#relationships) unser dynamisches Feld referenzieren zu können. Wenn Sie beispielsweise eine E-Mail an Mary senden und das Feld `{{company}}` verwenden, in ihrem Kontaktdatensatz jedoch keine Firma aufgeführt ist, können wir dies nicht ausfüllen.

## Warum wurde meine E-Mail gesendet, ohne alle dynamischen Felder auszufüllen? {#why-did-my-email-send-without-populating-all-dynamic-fields}

[!DNL Sales Connect] wird der Versand Ihrer E-Mails verhindert, wenn wir nicht alle Ihre dynamischen Felder in der E-Mail ausfüllen können. **Es** jedoch einige Ausnahmen von dieser Regel. Einige Felder werden leer gesendet oder automatisch einen Wert ausgefüllt, falls wir einen finden können. Diese Felder und wie sie reagieren, wenn sie das Feld nicht ausfüllen können, sind unten aufgeführt.

`{{first_name}}` = LEER

`{{last_name}}` = LEER

`{{title}}` = LEER

`{{company}}` = „Ihre Firma“

`{{friendly_company}}` = „Ihre Firma“

>[!NOTE]
>
>Das `{{first_name}}` Feld wird sowohl in [!DNL Sales Connect] als auch [!DNL Salesforce] angezeigt, um zu versuchen, Informationen abzurufen. Alle anderen Felder in dieser Liste [!DNL Sales Connect] nur das Ausfüllen des Felds.
