---
unique-page-id: 4720710
description: Richten Sie SPF und DKIM für Ihre E-Mail-Zustellbarkeit ein - Marketing-Dokumente - Produktdokumentation
title: Richten Sie SPF und DKIM für Ihre E-Mail-Zustellbarkeit ein
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---


# Richten Sie SPF und DKIM für Ihre E-Mail-Zustellbarkeit {#set-up-spf-and-dkim-for-your-email-deliverability} ein.

Eine schnelle Methode zur Verbesserung der E-Mail-Versand besteht darin, **SPF** (Sender Policy Framework) und **DKIM** (Domain Keys Identified Mail) in Ihre DNS-Einstellungen zu integrieren. Mit dieser Ergänzung zu Ihren DNS-Einträgen teilen Sie Empfängern mit, dass Sie Marketo autorisiert haben, E-Mails in Ihrem Namen zu senden. Ohne diese Änderung hat Ihre E-Mail eine höhere Wahrscheinlichkeit, als Spam markiert zu werden, da die E-Mail von Ihrer Domäne adressiert, aber von einer IP-Adresse mit einer Marketing-Domäne gesendet wurde.

>[!CAUTION]
>
>Sie benötigen Ihren Netzwerkadministrator, um diese Änderung in Ihrem DNS-Datensatz vorzunehmen.

## Einrichten von SPF {#set-up-spf}

**Wenn Sie keinen SPF-Datensatz in Ihrer Domäne haben**

Bitten Sie Ihren Netzwerkadministrator, die folgende Zeile zu Ihren DNS-Einträgen hinzuzufügen. Ersetzen Sie [domain] durch die Hauptdomäne Ihrer Website (z. B. &quot;Firma.com&quot;) und [corpIP] mit der IP-Adresse Ihres Unternehmens-E-Mail-Servers (z. B. ‚255.255.255.255‘). Wenn Sie E-Mails von mehreren Domänen über Marketo senden, sollten Sie diese zu jeder Domäne hinzufügen (in einer Zeile).

`[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all`

**Wenn Sie einen SPF-Datensatz in Ihrer Domäne haben**

Wenn Ihr DNS-Eintrag bereits einen SPF-Datensatz enthält, fügen Sie Folgendes hinzu:

include:mktomail.com

## Einrichten von DKIM {#set-up-dkim}

**Was ist DKIM? Warum möchte ich DKIM einrichten?**

DKIM ist ein Authentifizierungsprotokoll, das von E-Mail-Empfängern verwendet wird, um festzustellen, ob eine E-Mail-Nachricht von dem Empfänger gesendet wurde, von dem die Nachricht stammt. DKIM verbessert oft die Zustellbarkeit von E-Mails an den Posteingang, da ein Empfänger sicher sein kann, dass die Nachricht keine Fälschung ist.

**Wie wirkt DKIM?**

Nachdem Sie den öffentlichen Schlüssel in Ihrem DNS-Datensatz eingerichtet und die sendende Domäne im Abschnitt &quot;Admin&quot;(A) aktiviert haben, werden wir die benutzerdefinierte DKIM-Signatur für Ihre ausgehenden Nachrichten aktivieren, die eine verschlüsselte digitale Signatur mit jeder E-Mail, die wir für Sie senden, enthält (B). Die Empfänger können die digitale Signatur entschlüsseln, indem sie den &quot;öffentlichen Schlüssel&quot; im DNS (C) Ihrer sendenden Domäne suchen. Wenn der Schlüssel in der E-Mail mit dem Schlüssel in Ihrem DNS-Datensatz übereinstimmt, wird der Empfänger-E-Mail-Server eher die E-Mail-Adresse akzeptieren, die in Ihrem Namen gesendet wird.

![](assets/image2015-1-12-13-3a56-3a55.png)

**Wie richte ich DKIM ein?**

Weitere Informationen finden Sie unter [Einrichten einer benutzerdefinierten DKIM-Signatur](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md).

>[!MORELIKETHIS]
>
>* [Weitere Informationen zu SPF und Funktionsweise](https://www.open-spf.org/Introduction/)
>* [Marketing-Tools für die E-Mail-Zustellung](https://www.marketo.com/software/email-marketing/email-deliverability/)
>* [Ist mein SPF korrekt eingerichtet?](https://www.kitterman.com/spf/validate.html)
>* [Habe ich die richtige Syntax verwendet?](https://www.open-spf.org/SPF_Record_Syntax/)

