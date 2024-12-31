---
description: Antwortprotokollierung - Marketo-Dokumente - Produktdokumentation
title: Antwortprotokollierung
hide: true
hidefromtoc: true
exl-id: a89e8212-83cb-4987-abc9-76c5fd74c152
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Antwortprotokollierung {#reply-logging}

Aktionen mit Sales Insight bieten Ihnen die Möglichkeit, die Antworten Ihrer Interessenten automatisch in Salesforce zu protokollieren. Die Struktur, die Ihnen dies ermöglicht, basiert auf unserem E-Mail-Antwort-Tracking. Wenn wir die Antwort eines Interessenten verfolgen können, können wir diese Antwort bei Salesforce protokollieren.

## Anforderungen {#requirements}

* Muss E-Mails über API-Protokollierung protokollieren
* Muss in der Lage sein, [eine Antwort zu verfolgen](/help/marketo/product-docs/marketo-sales-insight/actions/send-a-sales-email/email-tracking-overview.md#how-reply-tracking-works)
* Muss mit Salesforce verbunden sein
* Muss Salesforce [API-Aufrufe) ](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm) haben

## Antwortprotokollierung aktivieren {#enable-reply-logging}

1. Um die Antwortprotokollierung zu aktivieren, gehen Sie zu Ihrer Salesforce-Einstellungsseite. Sobald die API-Protokollierung deaktiviert ist, sehen Sie die Option zum Überprüfen _Antworten protokollieren_.

   >[!NOTE]
   >
   >Für die Protokollierung von Antworten gelten dieselben Regeln wie für die Protokollierung gesendeter E-Mails. Dazu gehört, wie E-Mails protokolliert werden, an Leads und Kontakte, wenn ein doppelter Eintrag vorhanden ist und wenn keine übereinstimmenden Einträge gefunden werden.

## Festlegen des Antworttyps in Salesforce {#setting-type-to-reply-in-salesforce}

Es ist wichtig, aussagekräftige Daten aus Ihren Salesforce-Berichten zu erhalten. Die Möglichkeit, das Feld Typ als „Antwort“ füllen zu lassen, ermöglicht es Ihnen, diese Daten durch Ihre Berichte zu erhalten. Arbeiten Sie mit Ihrem `Salesforce admin` zusammen, um dieses Setup zu erhalten.

1. Wechseln Sie **Setup** > **Anpassen** > **Aktivitäten** > **Aufgabenfelder**.
1. Klicken Sie auf **Typ**.
1. Klicken Sie unter „Aufgabentyp-Auswahllistenwerte“ auf **Neu**.
1. Geben Sie „Antwort“ in das leere Feld ein. Achten Sie darauf, das „R“ großzuschreiben und auf &quot;**&quot;**.

   >[!NOTE]
   >
   >Sie müssen keinen Standard unter der Auswahlliste Typ auswählen. Sales Insight-Aktionen stellen fest, dass dieser Aktivitätstyp in Ihrer Salesforce-Instanz verfügbar ist, und füllen das Aufgabenfeld bei Ihren eingehenden Aktivitäten entsprechend aus.
