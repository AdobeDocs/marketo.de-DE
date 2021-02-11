---
unique-page-id: 14352482
description: Funktionsweise der Rückverfolgung von Antworten - Marketing Docs - Produktdokumentation
title: Funktionsweise der Nachverfolgung von Antworten
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# Funktionsweise der Nachverfolgung von Antworten {#how-reply-tracking-works}

Die Rückverfolgung der Antworten erfolgt durch Prüfen einer Nachrichten-ID, die in jeder E-Mail enthalten ist, die Sie senden. Jede E-Mail enthält eine eindeutige Nachrichten-ID, mit der wir einige der besten Antworten verfolgen können.

>[!PREREQUISITES]
>
>**Verbindung mit E-Mail-Server:** Sales Connect muss mit Ihrem Posteingang verbunden sein, damit wir wissen, wann eine neue Antwort eingetroffen ist. Sie benötigen Ihr Sales Connect-Konto [mit Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-tab-for-gmail-users.md) verbunden. Wenn Sie Outlook verwenden, müssen wir mit Ihrem [Exchange-Server](https://toutapp.com/next#settings/exchange_settings) integrieren.

Wenn Sales Connect die Antwort Ihres Potenzieller Kunden auf Ihre E-Mail nicht verfolgen kann, kann eine Kampagne nicht aufgrund der Antworterkennung oder der Anmeldung bei Salesforce beendet werden.  Was bedeuten wir, dass jede E-Mail-Adresse antworten kann?

Das bedeutet, dass wir die Antwort verfolgen können, wenn Sie flynn@flynnsarcade.com per E-Mail senden und er mit kevinf@flynnsarcade.com antwortet. Wenn Sie außerdem flynn@flynnsarcade.com und CC alan@encom.com per E-Mail senden und Alan Sie zurückschreibt, wird die Antwort auch erkannt und die Kampagne beendet.
