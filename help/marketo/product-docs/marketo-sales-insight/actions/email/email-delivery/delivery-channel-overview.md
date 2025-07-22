---
description: Übersicht über den Versandkanal - Marketo-Dokumente - Produktdokumentation
title: Versandkanal - Übersicht
exl-id: 8dd6fe3e-86ae-4361-bc0a-6488dc1df9fa
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# Versandkanal - Übersicht {#delivery-channel-overview}

Marketo Sales bietet mehrere Optionen zum Versand von E-Mails. In diesem Artikel werden die verfügbaren Versandkanäle sowie deren Auswahl und der Zeitpunkt der Auswahl erläutert.

## Empfohlen: Gmail oder Exchange via E-Mail-Verbindung {#recommended-gmail-or-exchange-via-email-connection}

Marketo Sales ermöglicht eine optimierte Einrichtung und verbesserte Zustellbarkeit über unseren E-Mail-Verbindungsservice. Die E-Mail-Verbindung ermöglicht es jedem Benutzer, eine Verbindung zu seinem [Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)- oder [[!DNL Exchange]](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)-Konto zu Marketo Sales herzustellen, um als Versandkanal der Wahl für alle E-Mails vom Marketo Sales genutzt zu werden.

Die Verwendung von Gmail oder [!DNL Exchange] bietet einige deutliche Vorteile gegenüber anderen Versandkanaloptionen:

* Dies ist ein bewährter Versandkanal mit einer bewährten Reputation, die dazu beiträgt, die Zustellbarkeit hoch zu halten.
* Authentifizierungsmethoden wie SPF und DKIM werden bereits von Ihrem IT-Team konfiguriert und verwaltet, sodass es keine zusätzliche Einrichtung gibt.
* Das Senden von E-Mails innerhalb eines bestimmten E-Mail-Netzwerks (d. h. das Senden einer E-Mail als [!DNL Exchange] an ein Unternehmen, das E-Mails über [!DNL Exchange] erhält) kann die Zustellbarkeit weiter erhöhen.

Beachten Sie, dass diese Versandkanäle über eigene Versandbeschränkungen verfügen, die von Microsoft und Google durchgesetzt werden. Um dies zu bekämpfen, verwenden wir einen Drosselungsmechanismus, um Benutzern zu helfen, innerhalb dieser Grenzen zu bleiben. Weitere Informationen zu [E-Mail-Drosselung hier](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

>[!NOTE]
>
>Standardmäßig verwendet das O365-Plug-in immer Ihren Exchange-Versandkanal und das Gmail-Plug-in verwendet immer Ihren Gmail-Versandkanal, um E-Mails von den Plug-ins zu versenden.

**Bounce-Tracking**: Marketo Sales kann Bounces für Exchange Online- oder Gmail-Benutzer erkennen, indem die Bounce-Nachricht erkannt wird, die an den Posteingang des Absenders gesendet wird. Diese Bounce-Benachrichtigungen werden für Benutzer in den Bereichen Vorlagenanalyse, Campaign-Analyse und Live-Feed zusammengefasst. Das Bounce-Tracking wird für Exchange On-Premise-Kunden nicht unterstützt.

## Benutzerdefinierter Versandkanal über SMTP {#custom-delivery-channel-via-smtp}

Marketo Sales bietet die zusätzliche Option, einen SMTP-Server eines Drittanbieters zu verbinden, der als bevorzugter Versandkanal Ihres Vertriebsteams verwendet werden kann.

Die Verwendung eines SMTP-Drittanbieters ist eine hervorragende Option für Vertriebsteams, in denen das E-Mail-Volumen die höchste Priorität hat. SMTP-Anbieter wie Sendgrid und SparkPost sind optimiert, um die Bedürfnisse des Massen-E-Mail-Versands zu bedienen, und können skaliert werden, um die Bedürfnisse derjenigen zu erfüllen, die große E-Mail-Mengen bereitstellen möchten.

Darüber hinaus bieten SMTP-Drittanbieter eine Fülle von Funktionen, um die Zustellbarkeitserfordernisse Ihres Teams zu unterstützen (z. B. E-Mail-Versandberichte und dedizierte IP-Adressen). Dies ist eine großartige Option für diejenigen, die nach einer detaillierteren Kontrolle und Sichtbarkeit rund um ihren E-Mail-Versandkanal für den Verkauf suchen.

## Marketo-Verkaufsserver (veraltet) {#marketo-sales-servers-legacy}

Marketo Sales-Server sind nur für einige ältere ToutApp-Kunden verfügbar. Diese Kunden sehen in ihren E-Mail-Einstellungen Marketo-Vertriebs-Server. Alle Nicht-Legacy-Kunden sehen Marketo Sales nicht als Option und sollten ihr Gmail- oder [!DNL Outlook]-Konto mit Marketo Sales verbinden, um einen Versandkanal zu entsperren.

Marketo Sales-Server unterstützen keine DKIM- und SPF-Authentifizierungsmethoden, was die Zustellbarkeitsrate senken kann. Aus diesem Grund empfehlen wir allen Kunden, eine Verbindung zu Gmail oder [!DNL Outlook] herzustellen, um eine optimale Zustellbarkeit zu erzielen.

## MSC-Server (veraltet) {#msc-servers-legacy}

MSC-Server sind nur für einige ältere ToutApp-Kunden verfügbar. Diese Kunden sehen MSC-Server in ihren E-Mail-Einstellungen. Nicht-Legacy-Kunden sehen MSC nicht als Option und sollten ihr Gmail- oder Outlook-Konto mit Sales Connect verbinden, um einen Versandkanal zu entsperren.

MSC-Server unterstützen keine DKIM- und SPF-Authentifizierungsmethoden, was die Zustellbarkeitsrate senken kann. Aus diesem Grund empfehlen wir allen Kunden, eine Verbindung zu Gmail oder [!DNL Outlook] herzustellen, um eine optimale Zustellbarkeit zu erzielen.

## Marketo-Server {#marketo-servers}

E-Mail-Server von Marketo lassen sich nicht mit Marketo Sales integrieren. Marketo-Server sind für die Massenbereitstellung optimiert, damit sie an die Anforderungen von Marketing-Experten angepasst werden können. Gmail und [!DNL Exchange] weisen jedoch eine höhere Erfolgsrate für die 1:1-Verkaufskommunikation auf. Aus diesem Grund empfehlen wir, diese Server für Ihre Verkaufskommunikation zu verwenden.

>[!MORELIKETHIS]
>
>* [E-Mail-Verbindung für Gmail-Benutzer](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [E-Mail-Verbindung für [!DNL Outlook] Benutzer](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [Einrichten eines benutzerdefinierten Versandkanals](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [Drosselung der E-Mail-Verbindung](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)
