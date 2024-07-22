---
unique-page-id: 14352482
description: Funktionsweise der Antwortverfolgung - Marketo-Dokumente - Produktdokumentation
title: Funktionsweise der Antwortverfolgung
exl-id: 8d087014-99b7-47ba-9f08-95b13bc16438
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---

# Funktionsweise der Antwortverfolgung {#how-reply-tracking-works}

Das Tracking der Antworten erfolgt durch Überprüfen einer Nachrichten-ID, die in jeder gesendeten E-Mail enthalten ist. Jede E-Mail enthält eine eindeutige Nachrichten-ID, mit der wir die beste Antwort-Tracking-Funktion nutzen können.

>[!PREREQUISITES]
>
>**Verbindung mit E-Mail-Server:** Sales Connect muss mit Ihrem Posteingang verbunden sein, damit wir wissen, wann eine neue Antwort eintrifft. Sie müssen Ihr Sales Connect-Konto [mit Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md) verbinden. Wenn Sie Outlook verwenden, müssen wir in Ihren [Exchange-Server](https://toutapp.com/next#settings/exchange_settings) integrieren.

Wenn Sales Connect die Antwort Ihres Interessenten auf Ihre E-Mail nicht verfolgen kann, kann eine Kampagne nicht aufgrund der Antworterkennung angehalten oder die Antwort an Salesforce protokolliert werden.  Was bedeutet, dass jede E-Mail-Adresse antworten kann?

Wenn Sie also flynn@flynnsarcade.com per E-Mail senden und er mit kevinf@flynnsarcade.com antwortet, können wir die Antwort verfolgen. Wenn Sie außerdem eine E-Mail an flynn@flynnsarcade.com und CC alan@encom.com senden und Alan Sie zurückschreibt, wird auch die Antwort erkannt und die Kampagne beendet.
