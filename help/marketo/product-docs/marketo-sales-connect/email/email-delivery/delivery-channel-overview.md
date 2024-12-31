---
unique-page-id: 14352407
description: Übersicht über den Versandkanal - Marketo-Dokumente - Produktdokumentation
title: Versandkanal - Übersicht
exl-id: 432bad1e-4eaf-4be8-b856-be364c44816e
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 0%

---

# Versandkanal - Übersicht {#delivery-channel-overview}

Marketo Sales Connect bietet Ihnen mehrere Optionen zum Versand von E-Mails. In diesem Artikel werden die verfügbaren Versandkanäle sowie deren Auswahl und der Zeitpunkt der Auswahl erläutert.

## Empfohlen: Gmail oder Exchange via E-Mail-Verbindung {#recommended-gmail-or-exchange-via-email-connection}

Sales Connect ermöglicht eine optimierte Einrichtung und verbesserte Zustellbarkeit über unseren E-Mail-Verbindungsservice. Mit der E-Mail-Verbindung kann jeder Benutzer eine Verbindung zu seinem [Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)- oder [Exchange](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)-Konto mit Sales Connect herstellen, um als Versandkanal der Wahl für alle Sales Connect-E-Mails verwendet zu werden.

Die Verwendung von Gmail oder Exchange bietet einige deutliche Vorteile gegenüber anderen Versandkanaloptionen:

* Dies ist ein bewährter Versandkanal mit einer bewährten Reputation, die dazu beiträgt, die Zustellbarkeit hoch zu halten.
* Authentifizierungsmethoden wie SPF und DKIM werden bereits von Ihrem IT-Team konfiguriert und verwaltet, sodass es keine zusätzliche Einrichtung gibt.
* Das Senden von E-Mails innerhalb eines bestimmten E-Mail-Netzwerks (d. h. das Senden einer E-Mail als Exchange-Benutzer an ein Unternehmen, das E-Mails über Exchange erhält) kann die Zustellbarkeit weiter erhöhen.

Beachten Sie, dass diese Versandkanäle über eigene Versandbeschränkungen verfügen, die von Microsoft und Google durchgesetzt werden. Um dies zu bekämpfen, verwenden wir einen Drosselungsmechanismus, um Benutzern zu helfen, innerhalb dieser Grenzen zu bleiben. Weitere Informationen zu [E-Mail-Drosselung hier](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

>[!NOTE]
>
>Standardmäßig verwendet das O365-Plug-in immer Ihren Exchange-Versandkanal und das Gmail-Plug-in verwendet immer Ihren Gmail-Versandkanal, um E-Mails von den Plug-ins zu versenden.

**Bounce-Tracking**: MSC kann Bounces für Exchange Online- oder Gmail-Benutzer erkennen, indem die Bounce-Nachricht erkannt wird, die an den Posteingang des Absenders gesendet wird. Diese Bounce-Benachrichtigungen werden für Benutzer in den Bereichen Vorlagenanalyse, Campaign-Analyse und Live-Feed zusammengefasst. Das Bounce-Tracking wird für Exchange On-Premise-Kunden nicht unterstützt.

## Benutzerdefinierter Versandkanal über SMTP {#custom-delivery-channel-via-smtp}

Sales Connect bietet die zusätzliche Option, einen SMTP-Server eines Drittanbieters zu verbinden, der als bevorzugter Versandkanal Ihres Verkaufsteams verwendet werden kann.

Die Verwendung eines SMTP-Drittanbieters ist eine hervorragende Option für Vertriebsteams, in denen das E-Mail-Volumen die höchste Priorität hat. SMTP-Anbieter wie Sendgrid und SparkPost sind optimiert, um die Bedürfnisse des Massen-E-Mail-Versands zu bedienen, und können skaliert werden, um die Bedürfnisse derjenigen zu erfüllen, die große E-Mail-Mengen bereitstellen möchten.

Darüber hinaus bieten SMTP-Drittanbieter eine Fülle von Funktionen, um die Zustellbarkeitserfordernisse Ihres Teams zu unterstützen (z. B. E-Mail-Versandberichte und dedizierte IP-Adressen). Dies ist eine großartige Option für diejenigen, die nach einer detaillierteren Kontrolle und Sichtbarkeit rund um ihren E-Mail-Versandkanal für den Verkauf suchen.

## MSC-Server (veraltet) {#msc-servers-legacy}

MSC-Server sind nur für einige ältere ToutApp-Kunden verfügbar. Diese Kunden sehen MSC-Server in ihren E-Mail-Einstellungen. Nicht-Legacy-Kunden sehen MSC nicht als Option und sollten ihr Gmail- oder Outlook-Konto mit Sales Connect verbinden, um einen Versandkanal zu entsperren.

MSC-Server unterstützen keine DKIM- und SPF-Authentifizierungsmethoden, was die Zustellbarkeitsrate senken kann. Aus diesem Grund empfehlen wir allen Kunden, eine Verbindung zu Gmail oder Outlook herzustellen, um eine optimale Zustellbarkeit zu erzielen.

## Marketo-Server {#marketo-servers}

E-Mail-Server von Marketo sind nicht mit Sales Connect integriert. Marketo-Server sind für die Massenbereitstellung optimiert, damit sie an die Anforderungen von Marketing-Experten angepasst werden können. Gmail und Exchange haben jedoch eine höhere Erfolgsrate für die 1:1-Verkaufskommunikation, weshalb wir empfehlen, diese Server für Ihre Verkaufskommunikation zu verwenden.

>[!MORELIKETHIS]
>
>* [E-Mail-Verbindung für Gmail-Benutzer](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [E-Mail-Verbindung für Outlook-Benutzer](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [Einrichten eines benutzerdefinierten Versandkanals](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [Drosselung der E-Mail-Verbindung](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)
