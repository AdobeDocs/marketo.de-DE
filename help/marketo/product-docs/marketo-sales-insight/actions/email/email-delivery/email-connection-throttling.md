---
description: Einschränken der E-Mail-Verbindung - Marketo-Dokumente - Produktdokumentation
title: Einschränken der E-Mail-Verbindung
exl-id: 02450a1e-5b30-4057-b204-19fab1a7d6c9
feature: Sales Insight Actions
source-git-commit: 19f60f58ae4de26536b304eb8ae9677ecc221993
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Einschränken der E-Mail-Verbindung {#email-connection-throttling}

Die Integration Ihres Sales Connect-Kontos für den Versand über Exchange oder Gmail-E-Mail-Anbieter bietet eine optimierte Einrichtung und Optimierung der E-Mail-Zustellbarkeit für die 1:1-Verkaufskommunikation. Um jedoch gesunde Systeme und sichere Konten zu gewährleisten, setzen Gmail und Exchange die Versandbeschränkungen von E-Mails um. Diese Beschränkungen können nach Ermessen der Anbieter erhöht oder verringert werden.

## Einschränken der E-Mail-Verbindung (Beta) {#email-connection-throttling-beta}

Durch die Einschränkung der E-Mail-Verbindung können Sales Connect-Administratoren die Senderate von E-Mails bei Verwendung von Gmail oder Exchange als Versandkanal konfigurieren, sodass die Rate, mit der E-Mails an den Versandkanalanbieter weitergeleitet werden, die erzwungenen Beschränkungen nicht überschreitet.

Wenn die Grenzwerte durchgängig überschritten werden, kann dies manchmal als verdächtiges Verhalten des Versandkanalanbieters betrachtet werden, das dazu führt, dass E-Mails fehlschlagen und manchmal sogar ein Konto deaktiviert wird.

**Hinweise/Highlights**

* Automatisch aktiviert, sobald ein Benutzer eine Verbindung zu Gmail oder Exchange herstellt
* Können angepasst werden, wenn Sie die Einstellungen der Empfehlung erhöhen oder verringern möchten, um Ihre Anforderungen zu erfüllen
* Nur E-Mails, die über Gmail oder Exchange gesendet werden, werden beim benutzerdefinierten Versandkanal nicht gedrosselt
* Die Funktion &quot;Einschränken der E-Mail-Verbindung&quot;stellt für jeden einzelnen Benutzer eine separate E-Mail-Adresse in die Warteschlange, da jeder Benutzer über eine eigene Verbindung mit seinem E-Mail-Anbieter verfügt

**Konfigurieren der Einschränkungseinstellungen für E-Mail-Verbindungen**

1. Klicken Sie auf das Zahnradsymbol und wählen Sie **Einstellungen**.

   ![](assets/email-connection-throttling-1.png)

1. Klicken Sie unter &quot;Admin Settings&quot;auf **Allgemein**.

   ![](assets/email-connection-throttling-2.png)

1. Klicken Sie auf der Karte &quot;E-Mail-Verbindungs-Drosselung&quot;auf der rechten Seite auf das **Aktivieren der E-Mail-Einschränkung** festlegen.

   ![](assets/email-connection-throttling-3.png)

1. Geben Sie auf der Karte &quot;Einschränken der E-Mail-Verbindung&quot;auf der rechten Seite die gewünschte Stapelgröße der E-Mails ein, die an den E-Mail-Kanal-Provider gesendet werden.

   ![](assets/email-connection-throttling-4.png)

1. Legen Sie die Wartezeit fest, bevor jeder Batch gesendet wird. In diesem Beispiel wählen wir 25 E-Mails alle 45 Sekunden.

   ![](assets/email-connection-throttling-5.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/email-connection-throttling-6.png)

Nachdem die Änderungen gespeichert wurden, werden alle Benutzer ihre E-Mails in Batches an ihr verbundenes Gmail- oder Exchange-Konto zur Bereitstellung senden.

## Einschränkungen des E-Mail-Anbieters {#email-provider-limits}

**Outlook 365**

Business/Enterprise

* 10.000 pro Tag
* 30 pro Minute
* 500 Empfänger pro E-Mail

Weitere Informationen [finden Sie hier .](https://docs.microsoft.com/en-us/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#RecipientLimits).

**Gmail**

* 2000 pro Tag (500 für Test- und Kennzeichnungs-Konten)
* 2 E-Mails pro Sekunde (API-Limit)
* 2.000 Empfänger pro Nachricht (maximal 500 für externe Empfänger)

Weitere Informationen [finden Sie hier .](https://support.google.com/a/answer/166852?hl=en).

**Microsoft Exchange Server (2010, 2013)**

Beschränkungen werden von der IT-Abteilung des Unternehmens festgelegt, da der Server von der Organisation gehostet wird. Wenden Sie sich für weitere Informationen an den Netzwerk- oder Systemadministrator.

>[!MORELIKETHIS]
>
>* [Versandkanal-Übersicht](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/delivery-channel-overview.md)
>* [E-Mail-Verbindung für Gmail-Benutzer](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [E-Mail-Verbindung für Outlook-Benutzer](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
