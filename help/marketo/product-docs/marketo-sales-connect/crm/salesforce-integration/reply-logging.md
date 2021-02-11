---
unique-page-id: 14352480
description: Logging (SFDC) - Marketing Docs - Produktdokumentation
title: Antwortprotokollierung (SFDC)
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# Antwortprotokollierung (SFDC) {#reply-logging-sfdc}

Sales Connect bietet Ihnen die Möglichkeit, die Antworten Ihrer Potenzieller Kunde automatisch bei Salesforce zu protokollieren. Die Struktur, die Ihnen dies ermöglicht, basiert auf unserer E-Mail-Antwort-Verfolgung. Wenn wir die Antwort eines Potenzieller Kunden nachverfolgen können, können wir diese Antwort bei Salesforce protokollieren.

## Voraussetzungen {#requirements}

* Muss E-Mails über API-Protokollierung protokollieren
* Muss in der Lage sein, eine Antwort &lt; a1/> zu verfolgen[](/help/marketo/product-docs/marketo-sales-connect/email/common-tracking-questions/how-reply-tracking-works.md)
* Muss mit Salesforce verbunden sein
* muss Salesforce [API-Aufrufe](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm) verfügbar haben

## Antwortprotokollierung aktivieren {#enable-reply-logging}

1. Zur Aktivierung der Antwortprotokollierung gelangen Sie zu Ihrer Salesforce-Einstellungsseite. Wenn die API-Protokollierung deaktiviert ist, wird die Option zum Aktivieren von _Protokollantworten_ angezeigt.

   >[!NOTE]
   >
   >Bei der Antwortenprotokollierung gelten dieselben Regeln wie bei der Protokollierung von gesendeten E-Mails. Dazu gehört auch, wie E-Mails protokolliert werden. Interessenten und Kontakte; wenn ein Duplikat vorliegt; wenn keine übereinstimmenden Datensätze gefunden wurden.

## Einstellen des Typs für Antwort in Salesforce {#setting-type-to-reply-in-salesforce}

Es ist wichtig, aussagekräftige Daten aus Ihren Salesforce-Berichten zu erhalten. Wenn das Feld &quot;Typ&quot;als &quot;Antwort&quot;ausgefüllt werden kann, können Sie diese Daten durch Ihre Berichte abrufen. Setzen Sie `Salesforce admin` ein, um dieses Setup zu erhalten.

1. Gehen Sie zu **Setup** > **Anpassen** > **Aktivitäten** > **Aufgaben-Felder**.
1. Klicken Sie auf **Typ**.
1. Klicken Sie unter &quot;Aufgabe Type Picklist Values&quot;auf **New**.
1. Geben Sie &quot;Antworten&quot;in das leere Feld ein. Vergewissern Sie sich, dass Sie das R großschreiben und klicken Sie auf **Speichern**.

   >[!NOTE]
   >
   >Es ist nicht erforderlich, einen Standard in der Liste Typ auszuwählen. Sales Connect wird sehen, dass dieser Aktivität-Typ in Ihrer Salesforce-Instanz verfügbar ist, und das Feld Aufgabe entsprechend auf Ihren eingehenden Aktivitäten ausfüllen.
