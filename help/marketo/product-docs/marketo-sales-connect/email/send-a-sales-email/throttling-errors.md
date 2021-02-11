---
unique-page-id: 14352581
description: Einschränken von Fehlern - MarketingToDocs - Produktdokumentation
title: Einschränken von Fehlern
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---


# Einschränken von Fehlern {#throttling-errors}

## Dateibeschränkung erreicht {#file-limit-reached}

Wenn Sie über Ihren eigenen Server senden, wird es Beschränkungen für die Anzahl der E-Mails geben, die Sie gleichzeitig senden können. Wenn Sie über Sales Connect senden, haben Sie die Möglichkeit, viele E-Mails zu senden, aber wir versuchen, sie alle gleichzeitig zu senden. Wenn Sie also wissen, dass Ihr Server Sie bei 100 E-Mails pro Minute ausschaltet, müssen Sie über die [Webanwendung](https://toutapp.com/login) nur bis zu 100 E-Mails senden. Andernfalls können die E-Mails hier landen, da die E-Mails auf Ihrem Server gedrosselt werden.

## Authentifizierungsfehler {#authentication-error}

Das bedeutet, dass wir die Verbindung zu Ihrem SMTP-Server nicht authentifizieren konnten. Wahrscheinlich hat sich Ihr Passwort kürzlich geändert und Sie müssen lediglich Ihre neuen Anmeldedaten authentifizieren.

Gehen Sie dazu zu Ihren SMTP-Einstellungen, wo Sie die gleiche Fehlermeldung sehen sollten. Aktualisieren Sie Ihre Anmeldeinformationen und klicken Sie auf **Authentifizierung und Speichern**, um eine Bestätigungsmeldung anzuzeigen.

Gehen Sie zu Ihren fehlgeschlagenen Versänden, um zu versuchen, diese E-Mails erneut zu senden.
