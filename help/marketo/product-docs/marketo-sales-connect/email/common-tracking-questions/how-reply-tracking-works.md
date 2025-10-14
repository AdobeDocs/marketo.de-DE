---
unique-page-id: 14352482
description: Funktionsweise des Antwort-Trackings - Marketo-Dokumente - Produktdokumentation
title: Funktionsweise der Antwortverfolgung
exl-id: 8d087014-99b7-47ba-9f08-95b13bc16438
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 4%

---

# Funktionsweise der Antwortverfolgung {#how-reply-tracking-works}

Das Antwort-Tracking erfolgt anhand einer Nachrichten-ID in jeder gesendeten E-Mail. Jede E-Mail enthält eine eindeutige Nachrichten-ID, mit der wir einige der besten Antworten verfolgen können.

>[!PREREQUISITES]
>
>**Verbindung zum E-Mail-Server:** [!DNL Sales Connect] muss mit Ihrem Posteingang verbunden sein, damit wir wissen, wann eine neue Antwort eingegangen ist. Sie müssen Ihr [!DNL Sales Connect]-Konto mit [Gmail“ &#x200B;](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md). Wenn Sie [!DNL Outlook] verwenden, müssen wir eine Integration mit Ihrem [Exchange-Server](https://toutapp.com/next#settings/exchange_settings) vornehmen.

Wenn [!DNL Sales Connect] die Antwort Ihres Interessenten auf Ihre E-Mail nicht verfolgen können, kann er eine Kampagne nicht auf der Grundlage der Antworterkennung stoppen oder diese Antwort [!DNL Salesforce] protokollieren.  Was meinen wir damit, dass jede E-Mail-Adresse antworten kann?

Wenn Sie also eine E-Mail an <flynn@flynnsarcade.com> senden und er mit <kevinf@flynnsarcade.com> antwortet, können wir die Antwort verfolgen. Wenn Sie <flynn@flynnsarcade.com> und CC <alan@encom.com> per E-Mail senden und Alan Sie zurückschreibt, wird die Antwort ebenfalls erkannt und die Kampagne wird beendet.
