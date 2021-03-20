---
unique-page-id: 14352407
description: Übersicht über Versand Kanal - Marketing-Dokumente - Produktdokumentation
title: Übersicht über Versand Kanal
translation-type: tm+mt
source-git-commit: f3e3efc1cc480e9c6501b7e808f53c3a8bdc93d8
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Übersicht über Versand-Kanal {#delivery-channel-overview}

Marketo Sales Connect bietet mehrere Optionen zur Bereitstellung von E-Mails. In diesem Artikel werden die Kanal des Versands, die Sie nutzen können, sowie die Auswahlmöglichkeiten und der Zeitpunkt der Auswahl der  überprüft.

## Empfohlen: Google Mail oder Exchange über E-Mail-Verbindung {#recommended-gmail-or-exchange-via-email-connection}

Sales Connect ermöglicht ein optimiertes Setup und die verbesserte Lieferbarkeit über unseren E-Mail-Verbindungsdienst. Die E-Mail-Verbindung ermöglicht es jedem Benutzer, eine Verbindung zu seinem [Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)- oder [Exchange](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)-Konto zu Sales Connect herzustellen, um als bevorzugten Versand für alle Sales Connect-E-Mails verwendet zu werden.

Die Verwendung von Gmail oder Exchange hat einige deutliche Vorteile gegenüber anderen Versand-Kanal-Optionen:

* Dies ist ein bewährter Versand Kanal mit einem etablierten Ruf, der dazu beiträgt, die Lieferbarkeit hoch zu halten.
* Authentifizierungsmethoden wie SPF und DKIM werden bereits von Ihrem IT-Team konfiguriert und verwaltet, sodass kein zusätzliches Setup vorhanden ist.
* Das Senden von E-Mails innerhalb eines bestimmten E-Mail-Netzwerks (d. h. das Senden einer E-Mail als Exchange-Benutzer an eine Firma, die E-Mails über Exchange erhält) kann die Zustellbarkeit weiter erhöhen.

Es ist wichtig zu beachten, dass diese Versand-Kanal ihre eigenen Sendeschränkungen haben, die von Microsoft und Google erzwungen werden. Um dies zu bekämpfen, verwenden wir einen Drosselungsmechanismus, der Benutzern hilft, sich innerhalb dieser Grenzen zu halten. Erfahren Sie mehr über [E-Mail-Einschränkungen hier](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

>[!NOTE]
>
>Standardmäßig verwendet das O365-Plugin immer Ihren Exchange-Versand-Kanal und das Gmail-Plugin verwendet immer Ihren Gmail-Versand-Kanal, um E-Mails von den Plugins zu senden.

**Absprungverfolgung**: MSC kann Absprünge für Exchange Online- oder Gmail-Benutzer erkennen, indem die Absprungmeldung erkannt wird, die an den Posteingang des Absenders gesendet wird. Diese Absprungbenachrichtigungen werden in Vorlagenanalysen, Kampagnen-Analysen und Live-Feed-Benachrichtigungen für Benutzer aggregiert. Die Absprungverfolgung wird für Exchange-On-Prem-Kunden nicht unterstützt.

## Benutzerdefinierter Versand-Kanal über SMTP {#custom-delivery-channel-via-smtp}

Sales Connect Angebot die zusätzliche Option, einen Drittanbieter-SMTP-Server anzuschließen, der als bevorzugter Versand-Kanal Ihres Vertriebsteams verwendet werden kann.

Die Nutzung eines Drittanbieter-SMTP-Providers ist eine großartige Option für Vertriebsteams, in denen das E-Mail-Volumen die höchste Priorität hat. SMTP-Anbieter wie Sendgrid und Sparkpost sind optimiert, um die Anforderungen von Massen-E-Mail-Versänden zu bedienen und können skaliert werden, um die Anforderungen derjenigen zu erfüllen, die große E-Mail-Mengen bereitstellen möchten.

Darüber hinaus bieten SMTP-Anbieter von Drittanbietern eine Vielzahl von Funktionen, die die Bereitstellungsanforderungen Ihres Teams unterstützen (z. B. E-Mail-Versandberichte und dedizierte IP-Adressen). Dies ist eine großartige Option für diejenigen, die auf der Suche nach detaillierteren Steuerelementen und Sichtbarkeit für ihren E-Mail-Versand-Kanal sind.

## MSC-Server (Legacy) {#msc-servers-legacy}

MSC-Server stehen nur für ältere ToutApp-Kunden zur Verfügung. Diese Kunden sehen die MSC-Server in ihren E-Mail-Einstellungen. Alle Nicht-Legacy-Kunden sehen MSC nicht als Option und sollten ihr Gmail- oder Outlook-Konto mit Sales Connect verbinden, um einen Versand-Kanal zu entsperren.

MSC-Server unterstützen keine DKIM- und SPF-Authentifizierungsmethoden, wodurch die Bereitstellungsrate gesenkt werden kann. Daher empfehlen wir allen Kunden, sich mit Gmail oder Outlook zu verbinden, um die bestmögliche Lieferbarkeit zu erreichen.

## Marketo-Server {#marketo-servers}

Marketing-E-Mail-Server werden nicht in Sales Connect integriert. Marketo-Server sind für den Massenzugriff optimiert, damit sie an die Anforderungen von Marketingexperten angepasst werden können. Gmail und Exchange haben jedoch eine höhere Erfolgsrate bei der Kommunikation über den 1:1-Vertrieb, weshalb wir empfehlen, diese Server für Ihre Vertriebskommunikation zu verwenden.

>[!MORELIKETHIS]
>
>* [E-Mail-Verbindung für Gmail-Benutzer](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [E-Mail-Verbindung für Outlook-Benutzer](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [Einrichten eines benutzerspezifischen Versand-Kanals](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [Einschränken der E-Mail-Verbindung](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)

