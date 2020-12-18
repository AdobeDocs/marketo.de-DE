---
unique-page-id: 14746594
description: Einrichten eines SMTP-Servers - Marketing Docs - Produktdokumentation
title: Einrichten eines SMTP-Servers
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 0%

---


# Einrichten eines SMTP-Servers {#setting-up-an-smtp-server}

## Übersicht {#overview}

**Was ist ein SMTP-Server?**

**Das** Simple  **** Mail  **** Transfer  **** Protocol ist der Server, der für den Versand Ihrer ausgehenden E-Mail verantwortlich ist. Wenn Sie eine E-Mail von Ihrem E-Mail-Client senden, verwenden Sie denselben Dienst, um Ihre E-Mail zu senden.

**Warum möchte ich meinen SMTP-Server mit Sales Connect einrichten?**

Sie ermöglicht es Ihnen, den Ruf Ihrer Firma zu nutzen und sich nicht auf andere zu verlassen. Unsere Standard-MSC-Server sind Teil eines gemeinsamen IP-Pools, was bedeutet, dass sie von einem gemeinsamen Ruf gesendet werden. Wir empfehlen Ihnen, dass Ihr Team einen eigenen Versand-Kanal mit Sales Connect einrichtet.

**Wie sendet Sales Connect mit meinem SMTP-Server?**

Indem Sie [diese Schritte](http://docs.marketo.com/x/ZgPh) befolgen.

![](assets/1.png)

`<pre><em>SMTP Server Setup Page in Sales Connect</em><br> </pre>` **Muss ich etwas in meinem E-Mail-Client einrichten?**

Was den Kanal eines Versands betrifft, nein. Sobald Sie unser Add-In installiert haben, nutzt Sales Connect denselben Versand-Kanal, den Sie für das Senden von E-Mails eingerichtet haben.

## SMTP-Berechtigungen abrufen {#getting-the-smtp-credentials}

**Wie erhalte ich meine SMTP-Anmeldeinformationen?**

Wenden Sie sich an Ihr IT-Team, um herauszufinden, welchen Versand-Kanal Ihre Firma zum Senden von E-Mails verwendet und wie Sie Zugriff auf Ihre SMTP-Anmeldeinformationen erhalten. Je nachdem, wie Ihr Server konfiguriert ist, verfügen Sie möglicherweise über einige benutzerdefinierte Werte für den SMTP-Servernamen oder den Serveranschluss. Wenn Sie über kein eigenes IT-Team verfügen, wenden Sie sich an Ihren E-Mail-Anbieter.

**Welche Optionen stehen zur Verfügung, wenn meine Firma Office365 verwendet?**

Vorteile

* Einfache Einrichtung
* Jeder Benutzer mit einem Office365-Konto hat Zugriff auf diesen SMTP-Server

Nachteile

* Einschränkungen können auftreten
* Jeder Benutzer muss dies selbst einrichten
* Das Ändern des O365-Kennworts eines Benutzers führt zu einer fehlerhaften Verbindung.

Wenn Sie Office365 oder Exchange Online verwenden, können Sie eine Verbindung zu Ihrem SMTP-Server herstellen, indem Sie einen Standardberechtigungssatz verwenden. Denken Sie daran, dass Office365 kein Massen-E-Mail-Versand-Service ist, auch wenn dies für das Senden von einmaligen E-Mails gut funktioniert. Beim Senden von Massen-E-Mails kann Office365 Ihre E-Mails drosseln, was zu einem fehlgeschlagenen Versand führen kann. Weitere Informationen zu diesem Thema finden Sie im Microsoft-Artikel [wie Sie die SMTP-Clientübermittlung einrichten](http://support.office.com/en-us/article/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-365-69f58e99-c550-4274-ad18-c805d654b4c4).
`<blockquote>  <p>“You can only send from one email address unless your device can store login credentials for multiple Office 365 mailboxes. Office 365 imposes a limit of 30 messages sent per minute, and a limit of 10,000 recipients per day.”</p> </blockquote>`\
Wenn Sie sich entscheiden, Office365 als Versand-Kanal zu verwenden, müssen Sie diese Anmeldeinformationen eingeben. Die gleichen Anmeldeinformationen können nicht für das gesamte Team verwendet werden, da Office365 die E-Mail-Adresse und das Kennwort des Benutzers verwendet, um eine Verbindung herzustellen.

Microsoft- und Bulk-Senden

[Klicken Sie ](http://technet.microsoft.com/en-us/library/exchange-online-limits.aspx#RecipientLimits) hier, um mehr über die Massenversand in Office365 zu erfahren. 
`<blockquote>  <p>“Exchange Online customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.”</p> </blockquote>`\
**Was ist, wenn meine Firma Gmail benutzt?**

Sie benötigen keine SMTP-Anmeldeinformationen, wenn Ihr Team Gmail als Versand-Kanal mit Sales Connect verwenden möchte. Mit Sales Connect können Benutzer über unsere OAuth-Integration auf ihren Gmail Versand Kanal zugreifen. Benutzer können dies aktivieren, indem sie ihr Sales Connect-Konto mit Gmail integrieren.

![](assets/2.png)

**Kann ich die gleichen SMTP-Anmeldeinformationen für mein gesamtes Team freigeben?**

Das hängt vom verwendeten Versand-Kanal ab. Dienste wie Sparkpost erlauben beispielsweise, dass die Anmeldeinformationen domänenbasiert sind, sodass jeder, der mit einer bestimmten Domäne sendet, authentifiziert ist, über diesen Server zu senden. In diesem Fall können Sie die Anmeldeinformationen für das Team freigeben.

Wenn Sie eine Verbindung zu Office365 herstellen, basieren die Anmeldeinformationen auf E-Mail-Adressen. Das bedeutet, dass nur die E-Mail-Adresse, die die Verbindung hergestellt hat, authentifiziert wird, um E-Mails über diesen Versand-Kanal zu senden. Daher sollten die Anmeldeinformationen **nicht** freigegeben werden.

![](assets/3.png)

