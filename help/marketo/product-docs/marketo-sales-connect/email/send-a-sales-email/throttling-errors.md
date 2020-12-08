---
unique-page-id: 14352581
description: Einschränken von Fehlern - MarketingToDocs - Produktdokumentation
title: Einschränken von Fehlern
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 0%

---


# Einschränken von Fehlern {#throttling-errors}

## Dateibeschränkung erreicht {#file-limit-reached}

Wenn Sie über Ihren eigenen Server senden, wird es Beschränkungen für die Anzahl der E-Mails geben, die Sie gleichzeitig senden können. Wenn Sie über Sales Connect senden, haben Sie die Möglichkeit, viele E-Mails zu senden, aber wir versuchen, sie alle gleichzeitig zu senden. Wenn Sie also wissen, dass Ihr Server Sie bei 100 E-Mails pro Minute ausschaltet, müssen Sie nur bis zu 100 E-Mails über die [Webanwendung](http://toutapp.com/login)senden. Andernfalls können die E-Mails hier landen, da die E-Mails auf Ihrem Server gedrosselt werden.

## Authentifizierungsfehler {#authentication-error}

Das bedeutet, dass wir die Verbindung zu Ihrem SMTP-Server nicht authentifizieren konnten. Wahrscheinlich hat sich Ihr Passwort kürzlich geändert und Sie müssen lediglich Ihre neuen Anmeldedaten authentifizieren.

Gehen Sie dazu zu Ihren [SMTP-Einstellungen](http://docs.marketo.com/display/docs/assets/external-link-1.jspa) `where you should see the same error message. Update your credentials and hit **Authenticate and Save** to see a confirmation message.`

Gehen Sie zu Ihren fehlgeschlagenen Versänden, um zu versuchen, diese E-Mails erneut zu senden.
