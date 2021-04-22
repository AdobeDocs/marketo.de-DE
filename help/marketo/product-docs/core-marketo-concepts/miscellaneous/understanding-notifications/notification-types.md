---
unique-page-id: 2953243
description: Benachrichtigungstypen - Marketo Docs - Produktdokumentation
title: Benachrichtigungstypen
exl-id: 384cea0a-6252-4600-9211-aa5d6a7e875c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 5%

---

# Benachrichtigungstypen {#notification-types}

Es gibt mehrere Benachrichtigungstypen.

## Kampagnenfehler  {#campaign-failure}

Fehler bei der Kampagne benachrichtigen Sie über Fehler in Ihren intelligenten Kampagnen.

## CRM-Synch.{#crm-sync}

CRM-Synchronisierungsbenachrichtigungen warnen Sie vor kritischen Problemen, die bei der CRM-Synchronisierung aufgetreten sind, wie z. B. fehlerhaften Berechtigungen oder ausbleibender Synchronisierung.

**Microsoft Dynamics**

Dynamics-Benachrichtigungen werden einmal alle 24 Stunden gesendet und enthalten Interessenten, die in diesem Zeitraum nicht synchronisiert wurden. Typische Gründe für einen Fehler sind Duplikat-Interessenten (wie oben) oder Fehler bei der Feldlänge.

![](assets/image2016-1-20-11-3a19-3a58.png)

**Salesforce**

Wenn Sie Salesforce verwenden, sehen die Synchronisierungsfehlerbenachrichtigungen wie folgt aus. Zu den typischen Fehlern zählen abgelaufene Anmeldeinformationen und Überschreitungen der API-Beschränkungen.

![](assets/salesforcesyncerror.png)

Engagement

Wenn Interessenten in einem Stream erschöpft sind, senden wir eine Benachrichtigung.  Die Meldung enthält die Anzahl der ausgenutzten Interessenten und weitere Informationen.

![](assets/image2014-10-14-10-3a57-3a9.png)

Facebook

Wenn Sie versuchen, Leads nach Facebook zu senden, ohne die Nutzungsbedingungen zu akzeptieren, oder wenn Sie versuchen, Leads nach dem Entfernen der Marketo-App nach Facebook zu senden.

Leerlauf-Auslöser-Kampagnenbereinigung

Deaktivieren Sie ausgelöste Smart-Kampagnen, die keine Aktivität mehr erhalten. Erfahren Sie mehr über [automatische Bereinigung der Trigger-Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/automatic-trigger-campaign-cleanup.md).

LinkedIn

Wenn Marketo nach drei Versuchen nicht in der Lage ist, eine neue Audience zu erstellen, sich anzumelden oder Push-E-Mails an LinkedIn zu senden.

![](assets/linkedin.png)

Web-Services

Sie werden benachrichtigt, wenn Sie Ihr tägliches Kontingent erreichen. Die Quote wird jede Nacht um Mitternacht, Central Time, zurückgesetzt.

>[!NOTE]
>
>Einige der Fehlercodes, die Sie möglicherweise erhalten, sind in unserer [Entwicklerdokumentation](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes) aufgeführt.
