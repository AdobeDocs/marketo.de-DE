---
description: Antwortprotokollierung - Marketo-Dokumente - Produktdokumentation
title: Antwortprotokollierung
hide: true
hidefromtoc: true
exl-id: a89e8212-83cb-4987-abc9-76c5fd74c152
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 2%

---

# Antwortprotokollierung {#reply-logging}

Mit Sales Insight Actions können Sie die Antworten Ihrer Interessenten automatisch [!DNL Salesforce] protokollieren. Die Struktur, die Ihnen dies ermöglicht, basiert auf unserem E-Mail-Antwort-Tracking. Wenn wir die Antwort eines Interessenten verfolgen können, können wir diese Antwort in [!DNL Salesforce] protokollieren.

## Anforderungen {#requirements}

* Muss E-Mails über API-Protokollierung protokollieren
* Muss in der Lage sein, [eine Antwort zu verfolgen](/help/marketo/product-docs/marketo-sales-insight/actions/send-a-sales-email/email-tracking-overview.md#how-reply-tracking-works)
* Muss mit [!DNL Salesforce] verbunden sein
* Muss [!DNL Salesforce] ([) ](https://developer.salesforce.com/docs/atlas.en-us.salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet/salesforce_app_limits_platform_api.htm) haben

## Antwortprotokollierung aktivieren {#enable-reply-logging}

1. Um die Antwortprotokollierung zu aktivieren, gehen Sie zu Ihrer Seite mit den [!DNL Salesforce]. Sobald die API-Protokollierung deaktiviert ist, sehen Sie die Option zum Überprüfen _Antworten protokollieren_.

   >[!NOTE]
   >
   >Für die Protokollierung von Antworten gelten dieselben Regeln wie für die Protokollierung gesendeter E-Mails. Dazu gehört, wie E-Mails protokolliert werden, an Leads und Kontakte, wenn ein doppelter Eintrag vorhanden ist und wenn keine übereinstimmenden Einträge gefunden werden.

## Festlegen des Typs für „Antwort in [!DNL Salesforce]&quot; {#setting-type-to-reply-in-salesforce}

Es ist wichtig, aussagekräftige Daten aus Ihren [!DNL Salesforce]-Berichten zu erhalten. Die Möglichkeit, das Feld Typ als „Antwort“ füllen zu lassen, ermöglicht es Ihnen, diese Daten durch Ihre Berichte zu erhalten. Arbeiten Sie mit Ihrem `[!DNL Salesforce] admin` zusammen, um dieses Setup zu erhalten.

1. Wechseln Sie **[!UICONTROL Setup]** > **[!UICONTROL Anpassen]** > **[!UICONTROL Aktivitäten]** > **[!UICONTROL Aufgabenfelder]**.
1. Klicken Sie auf **[!UICONTROL Typ]**.
1. Klicken [!UICONTROL  unter „Aufgabenart Auswahllistenwerte] auf **[!UICONTROL Neu]**.
1. Geben Sie „Antwort“ in das leere Feld ein. Achten Sie darauf, das „R“ großzuschreiben und auf &quot;**[!UICONTROL &quot;]**.

   >[!NOTE]
   >
   >Sie müssen keinen Standard unter der Auswahlliste Typ auswählen. [!DNL Sales Insight Actions] sehen, dass dieser Aktivitätstyp in Ihrer [!DNL Salesforce] verfügbar ist, und füllen das Aufgabenfeld bei Ihren eingehenden Aktivitäten entsprechend aus.
