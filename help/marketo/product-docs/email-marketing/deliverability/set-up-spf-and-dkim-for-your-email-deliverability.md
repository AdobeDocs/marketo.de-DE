---
unique-page-id: 4720710
description: Erfahren Sie, wie Sie SPF und DKIM in Ihrem DNS einrichten, um die E-Mail-Zustellbarkeit zu verbessern. Marketo autorisieren, in Ihrem Namen zu senden und Spam-Flags zu reduzieren.
title: Einrichten von SPF und DKIM für die Zustellbarkeit Ihrer E-Mails
exl-id: a0f88e94-3348-4f48-bbd2-963e2af93dc0
feature: Deliverability
source-git-commit: 7eb2f49718ea02be4a394a142c3a0ff05eeff796
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 94%

---

# Einrichten von SPF und DKIM für die Zustellbarkeit Ihrer E-Mails {#set-up-spf-and-dkim-for-your-email-deliverability}

Eine schnelle Methode zur Verbesserung der E-Mail-Zustellraten besteht darin, **SPF** (Sender Policy Framework) und **DKIM** (Domain Keys Identified Mail) in Ihre DNS-Einstellungen einzubinden. Mit dieser Ergänzung Ihrer DNS-Einträge teilen Sie den Empfangenden mit, dass Sie Marketo autorisiert haben, E-Mails in Ihrem Namen zu senden. Ohne diese Änderung ist die Wahrscheinlichkeit höher, dass Ihre E-Mail als Spam gekennzeichnet wird, da sie von Ihrer Domain adressiert, aber von einer IP-Adresse mit einer Marketo-Domain gesendet wurde.

>[!CAUTION]
>
>Ihre bzw. Ihr Netzwerkadmin muss diese Änderung an Ihrem DNS-Eintrag vornehmen.

## Einrichten von SPF {#set-up-spf}

**Wenn KEIN SPF-Eintrag in Ihrer Domain vorhanden ist**

Bitten Sie Ihre bzw. Ihren Netzwerkadmin, die folgende Zeile zu Ihren DNS-Einträgen hinzuzufügen. Ersetzen Sie [Domain] durch die Haupt-Domain Ihrer Website (z. B. „unternehmen.com“) und [corpIP] mit der IP-Adresse des E-Mail-Servers Ihres Unternehmens (z. B. „255.255.255.255“). Wenn Sie E-Mails von mehreren Domains über Marketo senden, sollten Sie dies zu jeder Domain hinzufügen (in einer Zeile).

`[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all`

**Wenn ein SPF-Eintrag in Ihrer Domain VORHANDEN ist**

Wenn bereits ein SPF-Eintrag in Ihrem DNS-Eintrag vorhanden ist, fügen Sie einfach Folgendes hinzu:

include:mktomail.com

## Einrichten von DKIM {#set-up-dkim}

**Was ist DKIM? Warum sollte ich DKIM einrichten?**

DKIM ist ein Authentifizierungsprotokoll, mit dem E-Mail-Empfangende bestimmen, ob eine E-Mail-Nachricht von der Entität gesendet wurde, die vorgegeben hat, sie zu senden. DKIM verbessert häufig die Zustellbarkeit von E-Mails an den Posteingang, da Empfangende sicher sein können, dass die Nachricht keine Fälschung ist.

**Wie funktioniert DKIM?**

Nachdem Sie den öffentlichen Schlüssel in Ihrem DNS-Eintrag eingerichtet und die Versand-Domain im Bereich „Administrator“ (A) aktiviert haben, wird die benutzerdefinierte DKIM-Signatur für Ihre ausgehenden Nachrichten aktiviert. Diese enthält eine verschlüsselte digitale Signatur mit jeder E-Mail, die für Sie versendet wird (B). Die Empfangenden können die digitale Signatur entschlüsseln, indem sie den „öffentlichen Schlüssel“ im DNS Ihrer Versand-Domain (C) nachschlagen. Wenn der Schlüssel in der E-Mail mit dem Schlüssel in Ihrem DNS-Eintrag übereinstimmt, akzeptiert der empfangende E-Mail-Server mit höherer Wahrscheinlichkeit die E-Mail, die Marketo in Ihrem Namen gesendet hat.

![](assets/image2015-1-12-13-3a56-3a55.png)

**Wie richte ich DKIM ein?**

Informationen dazu finden Sie unter [Einrichten einer benutzerdefinierten DKIM-Signatur](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* Weitere Informationen über SPF und wie es funktioniert`: http://www.open-spf.org/Introduction/`
>* Ist mein SPF korrekt eingerichtet?: `https://www.kitterman.com/spf/validate.html`
>* Habe ich die richtige Syntax verwendet?: `http://www.open-spf.org/SPF_Record_Syntax/`
