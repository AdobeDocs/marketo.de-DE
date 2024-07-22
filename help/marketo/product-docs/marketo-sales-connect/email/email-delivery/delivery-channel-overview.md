---
unique-page-id: 14352407
description: Versandkanal-Übersicht - Marketo-Dokumente - Produktdokumentation
title: Versandkanal-Übersicht
exl-id: 432bad1e-4eaf-4be8-b856-be364c44816e
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 0%

---

# Versandkanal-Übersicht {#delivery-channel-overview}

Marketo Sales Connect bietet Ihnen mehrere Optionen zum Versand von E-Mails. In diesem Artikel wird beschrieben, welche Versandkanäle Sie nutzen können, wie Sie sie auswählen und wann Sie einen anderen wählen können.

## Empfohlen: Gmail oder Exchange über E-Mail-Verbindung {#recommended-gmail-or-exchange-via-email-connection}

Sales Connect ermöglicht eine optimierte Einrichtung und die verbesserte Zustellbarkeit über unseren E-Mail-Verbindungsdienst. Die E-Mail-Verbindung ermöglicht es jedem Benutzer, eine Verbindung zu seinem [Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md) - oder [Exchange](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md) -Konto zu Sales Connect herzustellen, damit er als bevorzugter Versandkanal für alle Sales Connect-E-Mails verwendet werden kann.

Die Verwendung von Gmail oder Exchange bietet einige deutliche Vorteile gegenüber anderen Optionen für Versandkanäle:

* Dies ist ein bewährter Versandkanal mit bewährter Reputation, der dazu beiträgt, die Zustellbarkeit hoch zu halten.
* Authentifizierungsmethoden wie SPF und DKIM werden bereits von Ihrem IT-Team konfiguriert und verwaltet, sodass es keine zusätzliche Einrichtung gibt.
* Der Versand von E-Mails innerhalb eines bestimmten E-Mail-Netzwerks (d. h. das Senden einer E-Mail als Exchange-Benutzer an ein Unternehmen, das E-Mails über Exchange erhält) kann die Zustellbarkeit weiter verbessern.

Beachten Sie, dass diese Versandkanäle über eigene Versandbeschränkungen verfügen, die von Microsoft und Google erzwungen werden. Um dies zu bekämpfen, verwenden wir einen Drosselungsmechanismus, der Benutzern dabei hilft, diese Beschränkungen einzuhalten. Weitere Informationen zu [E-Mail-Einschränkungen finden Sie hier](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

>[!NOTE]
>
>Standardmäßig verwendet das O365-Plug-in immer Ihren Exchange-Versandkanal und das Gmail-Plug-in nutzt immer Ihren Gmail-Versandkanal, um E-Mails von den Plug-ins zu versenden.

**Bounce Tracking**: MSC kann Bounces für Exchange Online- oder Gmail-Benutzer erkennen, indem er die Bounce-Nachricht erkennt, die an den Posteingang des Absenders gesendet wird. Diese Bounce-Benachrichtigungen werden für Benutzer in Vorlagenanalysen, Campaign-Analysen und Live-Feed-Benachrichtigungen zusammengefasst. Das Bounce-Tracking wird für Exchange On-Prem-Kunden nicht unterstützt.

## Benutzerspezifischer Bereitstellungskanal über SMTP {#custom-delivery-channel-via-smtp}

Sales Connect bietet die zusätzliche Option, einen Drittanbieter-SMTP-Server anzuschließen, der als bevorzugter Versandkanal Ihres Verkaufsteams verwendet werden kann.

Die Verwendung eines SMTP-Anbieters eines Drittanbieters ist eine hervorragende Option für Vertriebsteams, in denen das E-Mail-Volumen die höchste Priorität hat. SMTP-Anbieter wie Sendgrid und Sparkpost sind optimiert, um die Anforderungen des Massen-E-Mail-Versands zu erfüllen und können skaliert werden, um die Anforderungen von Personen zu erfüllen, die große E-Mail-Volumen bereitstellen möchten.

Darüber hinaus bieten SMTP-Drittanbieter eine Vielzahl von Funktionen, mit denen Sie die Zustellbarkeitsanforderungen Ihres Teams unterstützen können (z. B. E-Mail-Versandberichte und dedizierte IP-Adressen). Dies ist eine hervorragende Option für diejenigen, die nach detaillierteren Kontrollen und einer besseren Sichtbarkeit ihres E-Mail-Versandkanals suchen.

## MSC-Server (alt) {#msc-servers-legacy}

MSC-Server sind nur für einige ältere ToutApp-Kunden verfügbar. Diese Kunden sehen MSC-Server, die in ihren E-Mail-Einstellungen verfügbar sind. Nicht-ältere Kunden sehen MSC nicht als Option und sollten ihr Gmail- oder Outlook-Konto mit Sales Connect verbinden, um einen Versandkanal zu entsperren.

MSC-Server unterstützen keine DKIM- und SPF-Authentifizierungsmethoden, die die Zustellrate senken können. Aus diesem Grund empfehlen wir allen Kunden, eine Verbindung zu Gmail oder Outlook herzustellen, um eine optimale Zustellbarkeit zu erreichen.

## Marketo-Server {#marketo-servers}

Marketo-E-Mail-Server werden nicht in Sales Connect integriert. Marketo-Server sind für die Massenbereitstellung optimiert, damit sie entsprechend den Anforderungen von Marketing-Experten skaliert werden können. Gmail und Exchange weisen jedoch eine höhere Erfolgsrate bei der 1:1-Verkaufskommunikation auf. Deshalb empfehlen wir die Verwendung dieser Server für Ihre Verkaufskommunikation.

>[!MORELIKETHIS]
>
>* [E-Mail-Verbindung für Gmail-Benutzer](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [E-Mail-Verbindung für Outlook-Benutzer](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [Einrichten eines benutzerdefinierten Bereitstellungskanals](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [Einschränken der E-Mail-Verbindung](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)
