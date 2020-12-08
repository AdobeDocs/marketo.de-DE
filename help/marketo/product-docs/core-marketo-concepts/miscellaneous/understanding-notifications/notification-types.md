---
unique-page-id: 2953243
description: Benachrichtigungstypen - Marketing-Dokumente - Produktdokumentation
title: Benachrichtigungstypen
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---


# Benachrichtigungstypen {#notification-types}

Es gibt mehrere Benachrichtigungstypen.

## Kampagne fehlgeschlagen  {#campaign-failure}

Fehler bei der Kampagne benachrichtigen Sie über Fehler in Ihren intelligenten Kampagnen.

## CRM-Synchronisierung {#crm-sync}

CRM-Synchronisierungsbenachrichtigungen warnen Sie vor kritischen Problemen, die bei der CRM-Synchronisierung aufgetreten sind, wie z. B. fehlerhaften Berechtigungen oder ausbleibender Synchronisierung.

**Microsoft Dynamics**

Dynamics-Benachrichtigungen werden einmal alle 24 Stunden gesendet und enthalten Interessenten, die in diesem Zeitraum nicht synchronisiert wurden. Typische Gründe für einen Fehler sind Duplikat-Interessenten (wie oben) oder Fehler bei der Feldlänge.

![](assets/image2016-1-20-11-3a19-3a58.png)

**Salesforce**

Wenn Sie Salesforce verwenden, sehen die Synchronisierungsfehlerbenachrichtigungen wie folgt aus. Zu den typischen Fehlern zählen abgelaufene Anmeldeinformationen und Überschreitungen der API-Beschränkungen.

![](assets/salesforcesyncerror.png)

Interaktion

Wenn Interessenten in einem Stream erschöpft sind, senden wir eine Benachrichtigung.  Die Meldung enthält die Anzahl der ausgenutzten Interessenten und weitere Informationen.

![](assets/image2014-10-14-10-3a57-3a9.png)

Facebook

Wenn Sie versuchen, Leads zu Facebook zu senden, ohne die Nutzungsbedingungen zu akzeptieren, oder wenn Sie versuchen, Leads zu Facebook zu senden, nachdem Sie die Marketing-App entfernt haben.

Säuberung der Idle Trigger-Kampagne

Deaktivieren Sie ausgelöste Smart-Kampagnen, die keine Aktivität mehr erhalten. Erfahren Sie mehr über die [automatische Kampagne](../../../../product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/automatic-trigger-campaign-cleanup.md)der Auslöser.

LinkedIn

Wenn Marketo nach drei Versuchen keine neue Audience, Anmeldung oder Push-E-Mails zu LinkedIn erstellen kann.

![](assets/linkedin.png)

Web-Services

Sie werden benachrichtigt, wenn Sie Ihr tägliches Kontingent erreichen. Die Quote wird jede Nacht um Mitternacht, Central Time, zurückgesetzt.

>[!NOTE]
>
>Einige der Fehlercodes, die Sie möglicherweise erhalten, sind in unserer [Entwicklerdokumentation](http://developers.marketo.com/rest-api/error-codes/#response_level_error_codes)aufgeführt.

