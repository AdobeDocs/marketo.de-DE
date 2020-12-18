---
unique-page-id: 14352600
description: Einrichten Ihres Outlook365 SMTP-Servers mit Sales Connect - Marketing Docs - Produktdokumentation
title: Einrichten des Outlook365 SMTP-Servers mit Vertriebsverbindung
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---


# Einrichten des Outlook365 SMTP-Servers mit Vertriebsverbindung {#how-to-set-up-your-outlook-smtp-server-with-sales-connect}

>[!NOTE]
>
>Wenn Ihr Unternehmen Outlook verwendet und Sie versuchen, einen E-Mail-Versand-Kanal mit Marketo Sales Connect einzurichten, empfehlen wir, eine Verbindung mit Ihrem Exchange-Server [über unsere E-Mail-Verbindungsfunktion ](http://docs.marketo.com/x/Z4AOAQ) herzustellen.

Um einen benutzerdefinierten Server [SMTP](http://docs.marketo.com/x/zYTS) als alternativen Versand-Kanal einzurichten, erfordert ToutApp, dass Sie aus Sicherheitsgründen eine bestimmte Form der Authentifizierung verwenden. Sie können einen beliebigen SMTP-Server auf Ihrer [SMTP-Konfigurationsseite](http://toutapp.com/next#settings/email-servers/smtp/configure) einrichten. Zum Einrichten eines Office365 SMTP-Servers empfiehlt Microsoft die folgende Konfiguration:\
**SMTP-Server**: smtp.office365.com\
**Serveranschluss**: Port 587 - gesichert\
**Authentifizierungsmethode**: Anmeldung (SSL/TLS)\
**Benutzername oder Anmeldung**: Ihre Office365-E-Mail-Adresse\
**Kennwort**: Ihr Office365-E-Mail-Kennwort\
**Ihre Domäne**: Ihre Firma

Wenn beim Einrichten des SMTP-Servers noch Probleme auftreten, stellen Sie sicher, dass die richtigen Anmeldeinformationen verwendet werden.

>[!NOTE]
>
>Beim Senden über Ihr Office365 SMTP setzt Microsoft ein `limit of 30 messages sent per minute` und eine Beschränkung von 10.000 Empfänger pro Tag ein. Außerdem müssen `each member` Ihres Teams, das E-Mails über den Office365 SMTP-Server senden möchte, diese mit ihrer eigenen E-Mail-Adresse und ihrem Passwort in ihren Sales Connect-Einstellungen einrichten. Aktivieren Sie das Kontrollkästchen für die Einstellung &quot; `Make this deliverability channel to all my team members` `" will not work` für diese Konfiguration gemäß den Microsoft Office365-Kontorichtlinien.

