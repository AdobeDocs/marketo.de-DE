---
description: Reply Logging - Marketo Docs - Produktdokumentation
title: Reply Logging
hide: true
hidefromtoc: true
source-git-commit: c398aff77e09f4a63db5d51af55178aa663ec98e
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 0%

---

# Reply Logging {#reply-logging}

Sales Insight Actions bietet Ihnen die Möglichkeit, die Antworten Ihrer Interessenten automatisch in Salesforce zu protokollieren. Die Struktur, die dies ermöglicht, basiert auf unserem E-Mail-Antworten-Tracking. Wenn wir die Antwort eines Interessenten nachverfolgen können, können wir diese Antwort an Salesforce protokollieren.

## Anforderungen {#requirements}

* Muss E-Mails über die API-Protokollierung protokollieren
* Muss [Antworten tracken](/help/marketo/product-docs/marketo-sales-insight/actions/send-a-sales-email/email-tracking-overview.md#how-reply-tracking-works)
* Muss mit Salesforce verbunden sein
* Muss Salesforce enthalten [API-Aufrufe](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm) available

## Aktivieren der Antwortprotokollierung {#enable-reply-logging}

1. Um die Antwortenprotokollierung zu aktivieren, gehen Sie zu Ihrer Salesforce-Einstellungsseite. Sobald die API-Protokollierung deaktiviert ist, wird die Option zum Aktivieren von _Protokollantworten_.

   >[!NOTE]
   >
   >Die Reaktionsprotokollierung folgt denselben Regeln wie die Protokollierung von gesendeten E-Mails. Dazu gehört auch die Protokollierung von E-Mails. Leads und Kontakte; wenn ein Datensatz doppelt vorhanden ist; wenn keine übereinstimmenden Datensätze gefunden wurden.

## Einstellen des Typs auf Antwort in Salesforce {#setting-type-to-reply-in-salesforce}

Es ist wichtig, aussagekräftige Daten aus Ihren Salesforce-Berichten zu erhalten. Wenn das Feld Typ als &quot;Antwort&quot;ausgefüllt werden kann, können Sie diese Daten durch Ihre Berichte abrufen. Partner sich mit Ihrem `Salesforce admin` um diese Einrichtung zu erhalten.

1. Navigieren Sie zu **Einrichtung** > **Anpassen** > **Tätigkeiten** > **Aufgabenfelder**.
1. Klicken **Typ**.
1. Klicken Sie unter &quot;Task Type Picklist Values&quot; **Neu**.
1. Geben Sie &quot;Antwort&quot;in das leere Feld ein. Vergewissern Sie sich, dass Sie das R großschreiben, und klicken Sie auf **Speichern**.

   >[!NOTE]
   >
   >Sie müssen unter der Auswahlliste Typ keinen Standardwert auswählen. Sales Insight-Aktionen sehen, dass dieser Aktivitätstyp in Ihrer Salesforce-Instanz verfügbar ist, und füllen das Aufgabenfeld entsprechend für Ihre eingehenden Aktivitäten aus.
