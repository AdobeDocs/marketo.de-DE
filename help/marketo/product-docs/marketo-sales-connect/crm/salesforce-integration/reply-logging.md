---
unique-page-id: 14352480
description: Logging (SFDC) - Marketing Docs - Produktdokumentation
title: Antwortprotokollierung (SFDC)
translation-type: tm+mt
source-git-commit: f28ff1acb0090892bdb92b75ef90d489db7abf20
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---


# Antwortprotokollierung (SFDC) {#reply-logging-sfdc}

Sales Connect bietet Ihnen die Möglichkeit, die Antworten Ihrer Potenzieller Kunde automatisch bei Salesforce zu protokollieren. Die Struktur, die Ihnen dies ermöglicht, basiert auf unserer E-Mail-Antwort-Verfolgung. Wenn wir die Antwort eines Potenzieller Kunden nachverfolgen können, können wir diese Antwort bei Salesforce protokollieren.

## Anforderungen {#requirements}

* Muss E-Mails über API-Protokollierung protokollieren
* Muss eine Antwort [verfolgen können](http://docs.marketo.com/x/BYPS)
* Muss mit Salesforce verbunden sein
* Salesforce- [API-Aufrufe](http://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm) müssen verfügbar sein

## Antwortprotokollierung aktivieren {#enable-reply-logging}

1. Zur Aktivierung der Antwortprotokollierung gelangen Sie auf Ihre Seite [Salesforce-Einstellungen](http://docs.marketo.com/pages/assets/external-link.jspa) . Wenn die API-Protokollierung deaktiviert ist, sehen Sie die Option *Logantworten.\
   *

   >[!NOTE]
   >
   >Bei der Antwortenprotokollierung gelten dieselben Regeln wie bei der Protokollierung von gesendeten E-Mails. Dazu gehört auch, wie E-Mails protokolliert werden. Interessenten und Kontakte; wenn ein Duplikat vorliegt; wenn keine übereinstimmenden Datensätze gefunden wurden.

## Einstellen des Typs für die Antwort in Salesforce {#setting-type-to-reply-in-salesforce}

Es ist wichtig, aussagekräftige Daten aus Ihren Salesforce-Berichten zu erhalten. Wenn das Feld &quot;Typ&quot;als &quot;Antwort&quot;ausgefüllt werden kann, können Sie diese Daten durch Ihre Berichte abrufen. Setzen Sie sich mit Ihrem Partner `Salesforce admin` zusammen, um dieses Setup zu erhalten.

1. Gehen Sie zu **Setup **> **Anpassen **> **Aktivitäten **> **Aufgaben-Felder**.
1. Klicken Sie auf **Typ**.
1. Klicken Sie unter &quot;Aufgabe Type Picklist Values&quot;auf **New**.
1. Geben Sie &quot;Antworten&quot;in das leere Feld ein. Vergewissern Sie sich, dass Sie das R großgeschrieben haben, und klicken Sie auf **Speichern**.

   >[!NOTE]
   >
   >Es ist nicht erforderlich, einen Standard in der Liste Typ auszuwählen. Sales Connect wird sehen, dass dieser Aktivität-Typ in Ihrer Salesforce-Instanz verfügbar ist, und das Feld Aufgabe entsprechend auf Ihren eingehenden Aktivitäten ausfüllen.

