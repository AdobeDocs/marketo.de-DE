---
unique-page-id: 14352482
description: Funktionsweise der Rückverfolgung von Antworten - Marketing Docs - Produktdokumentation
title: Funktionsweise der Nachverfolgung von Antworten
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---


# Funktionsweise der Nachverfolgung von Antworten {#how-reply-tracking-works}

Die Rückverfolgung der Antworten erfolgt durch Prüfen einer Nachrichten-ID, die in jeder E-Mail enthalten ist, die Sie senden. Jede E-Mail enthält eine eindeutige Nachrichten-ID, mit der wir einige der besten Antworten verfolgen können.

>[!PREREQUISITES]
>
>**Verbindung mit E-Mail-Server:** Sales Connect muss mit Ihrem Posteingang verbunden sein, damit wir wissen, wann eine neue Antwort eingetroffen ist. Sie benötigen Ihr Sales Connect-Konto [mit Gmail](http://docs.marketo.com/x/kYMOAQ) verbunden. Wenn Sie Outlook verwenden, müssen wir mit Ihrem [Exchange-Server](http://toutapp.com/next#settings/exchange_settings) integrieren.

Wenn Sales Connect die Antwort Ihres Potenzieller Kunden auf Ihre E-Mail nicht verfolgen kann, kann eine Kampagne nicht aufgrund der Antworterkennung oder der Anmeldung bei Salesforce beendet werden.  Was bedeuten wir, dass jede E-Mail-Adresse antworten kann?

Das bedeutet, wenn Sie [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#783217162b16170f3830170d0b1d2b0c190a13561b1715) per E-Mail senden und er mit [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#c08aafae93aeafb78094a8a58ea9a7a8b4b397a1b4a3a8eea3afad) antwortet, können wir die Antwort verfolgen. Wenn Sie [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#450f2a2b162b2a32050d2a303620163124372e6b262a28) und CC [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#3e5f525f507e5b505d5153105d5153) per E-Mail versenden und Alan Sie zurückschreibt, wird auch die Antwort erkannt und die Kampagne beendet.
