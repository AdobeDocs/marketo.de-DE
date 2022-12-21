---
unique-page-id: 2953243
description: Benachrichtigungstypen - Marketo-Dokumente - Produktdokumentation
title: Benachrichtigungstypen
exl-id: 384cea0a-6252-4600-9211-aa5d6a7e875c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 5%

---

# Benachrichtigungstypen {#notification-types}

Es gibt mehrere Benachrichtigungstypen.

## Kampagnenfehler  {#campaign-failure}

Kampagnenfehler melden Fehler in Ihren Smart-Kampagnen.

## CRM-Synch. {#crm-sync}

Benachrichtigungen zur CRM-Synchronisierung informieren Sie über kritische Probleme bei der CRM-Synchronisierung, z. B. falsche Berechtigungen oder die Synchronisierung.

**Microsoft Dynamics**

Dynamics-Benachrichtigungen werden alle 24 Stunden einmal gesendet und enthalten Leads, die in diesem Zeitraum nicht synchronisiert werden konnten. Typische Gründe für einen Fehler sind doppelte Leads (wie oben) oder Fehler bei der Feldlänge.

![](assets/image2016-1-20-11-3a19-3a58.png)

**Salesforce**

Wenn Sie Salesforce verwenden, sehen Synchronisierungsfehlerbenachrichtigungen etwa wie folgt aus: Typische Fehler umfassen abgelaufene Anmeldeinformationen und überschrittene API-Beschränkungen.

![](assets/salesforcesyncerror.png)

Engagement

Wenn Leads in einem Stream erschöpft sind, senden wir eine Benachrichtigung.  Die Benachrichtigung enthält die Anzahl der ausgelösten Leads und weitere Informationen.

![](assets/image2014-10-14-10-3a57-3a9.png)

Facebook

Wenn Sie versuchen, Leads an Facebook zu senden, ohne die Nutzungsbedingungen zu akzeptieren, oder wenn Sie versuchen, Leads nach dem Entfernen der Marketo-App an Facebook zu senden.

Leerlauf-Auslöser-Kampagnenbereinigung

Deaktivieren Sie ausgelöste Smart-Kampagnen, die keine Aktivität mehr erhalten. Weitere Informationen  [automatische Trigger-Kampagnenbereinigung](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/automatic-trigger-campaign-cleanup.md).

LinkedIn

Wenn Marketo nach drei Versuchen nicht in der Lage ist, eine neue Zielgruppe zu erstellen, sich anzumelden oder E-Mails an LinkedIn zu senden.

![](assets/linkedin.png)

Web-Services

Sie werden benachrichtigt, wenn Sie Ihr tägliches Kontingent erreichen. Die Quote wird jede Nacht um Mitternacht, Central Time, zurückgesetzt.

>[!NOTE]
>
>Einige der Fehlercodes, die Sie möglicherweise erhalten, sind in unserer [Entwicklerdokumentation](https://developers.marketo.com/rest-api/error-codes/#response_level_error_codes).
