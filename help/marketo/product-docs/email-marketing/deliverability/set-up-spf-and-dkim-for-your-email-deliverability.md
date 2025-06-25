---
unique-page-id: 4720710
description: Einrichten von SPF und DKIM für die Zustellbarkeit Ihrer E-Mails - Marketo-Dokumente - Produktdokumentation
title: Einrichten von SPF und DKIM für die Zustellbarkeit Ihrer E-Mails
exl-id: a0f88e94-3348-4f48-bbd2-963e2af93dc0
feature: Deliverability
source-git-commit: b95458ffab422901ef5e674756ae5e413ec542fd
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---

# Einrichten von SPF und DKIM für die Zustellbarkeit Ihrer E-Mails {#set-up-spf-and-dkim-for-your-email-deliverability}

Eine schnelle Methode zur Verbesserung der E-Mail-Versandraten besteht darin, **SPF** (Sender Policy Framework) und **DKIM** (Domain Keys Identified Mail) in Ihre DNS-Einstellungen einzubinden. Mit dieser Ergänzung Ihrer DNS-Einträge teilen Sie den Empfängern mit, dass Sie Marketo autorisiert haben, E-Mails in Ihrem Namen zu senden. Ohne diese Änderung ist die Wahrscheinlichkeit höher, dass Ihre E-Mail als Spam gekennzeichnet wird, da die E-Mail von Ihrer Domain adressiert, aber von einer IP-Adresse mit einer Marketo-Domain gesendet wurde.

>[!CAUTION]
>
>Sie benötigen Ihren Netzwerkadministrator, um diese Änderung in Ihrem DNS-Eintrag vorzunehmen.

## Einrichten von SPF {#set-up-spf}

**Wenn Sie keinen SPF-Eintrag in Ihrer Domain haben**

Bitten Sie Ihren Netzwerkadministrator, die folgende Zeile zu Ihren DNS-Einträgen hinzuzufügen. Ersetzen [Domain] durch die Haupt-Domain Ihrer Website (z. B. „company.com„) und [corpIP] mit der IP-Adresse Ihres E-Mail-Servers (z.B. &quot;255.255.255.255„) Wenn Sie E-Mails von mehreren Domains über Marketo senden, sollten Sie diese zu jeder Domain hinzufügen (in einer Zeile).

`[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all`

**Wenn Sie in Ihrer Domain über einen SPF-Eintrag verfügen**

Wenn Sie bereits über einen SPF-Eintrag in Ihrem DNS-Eintrag verfügen, fügen Sie Folgendes hinzu:

include:mktomail.com

## Einrichten von DKIM {#set-up-dkim}

**Was ist DKIM? Warum möchte ich DKIM einrichten?**

DKIM ist ein Authentifizierungsprotokoll, mit dem E-Mail-Empfänger bestimmen, ob eine E-Mail-Nachricht von jemandem gesendet wurde, von dem sie gesendet wurde. DKIM verbessert häufig die Zustellbarkeit von E-Mails an den Posteingang, da ein Empfänger sicher sein kann, dass die Nachricht keine Fälschung ist.

**Wie funktioniert DKIM?**

Nachdem Sie den öffentlichen Schlüssel in Ihrem DNS-Eintrag eingerichtet und die Versand-Domain im Admin-Bereich (A) aktiviert haben, aktivieren wir die benutzerdefinierte DKIM-Signatur für Ihre ausgehenden Nachrichten, die eine verschlüsselte digitale Signatur mit jeder E-Mail enthält, die wir für Sie versenden (B). Die Empfänger können die digitale Signatur entschlüsseln, indem sie den „öffentlichen Schlüssel“ im DNS (C) Ihrer Versand-Domain nachschlagen. Wenn der Schlüssel in der E-Mail mit dem Schlüssel in Ihrem DNS-Eintrag übereinstimmt, akzeptiert der empfangende E-Mail-Server mit höherer Wahrscheinlichkeit die E-Mail, die Marketo in Ihrem Namen gesendet hat.

![](assets/image2015-1-12-13-3a56-3a55.png)

**Wie richte ich DKIM ein?**

Siehe [Einrichten einer benutzerdefinierten DKIM-Signatur](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* Erfahren Sie mehr über SPF und wie es funktioniert`: http://www.open-spf.org/Introduction/`
>* Ist mein SPF korrekt eingerichtet?: `https://www.kitterman.com/spf/validate.html`
>* Habe ich die richtige Syntax verwendet?: `http://www.open-spf.org/SPF_Record_Syntax/`
