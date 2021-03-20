---
description: Einschränken der E-Mail-Verbindung - Marketing-Dokumente - Produktdokumentation
title: Einschränken der E-Mail-Verbindung
translation-type: tm+mt
source-git-commit: f3e3efc1cc480e9c6501b7e808f53c3a8bdc93d8
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---


# Einschränken der E-Mail-Verbindung {#email-connection-throttling}

Durch die Integration Ihres Sales Connect-Kontos, das über Exchange- oder Gmail-E-Mail-Provider-Angebote gesendet wird, wird die Einrichtung optimiert und die E-Mail-Zustellbarkeit für die 1:1-Verkaufskommunikation optimiert. Um die Systeme jedoch gesund und sicher zu halten, setzen Gmail und Exchange E-Mail-Senden-Beschränkungen ein. Diese Beschränkungen können nach Ermessen der Anbieter erhöht oder verringert werden.

## Email Connection Throttling (Beta) {#email-connection-throttling-beta}

>[!AVAILABILITY]
>
>Diese Funktion ist derzeit in der Beta-Version verfügbar. Wenden Sie sich zur Teilnahme an dieser Betaversion an Ihren Kundenbetreuer.

Mit der Funktion zum Einschränken der E-Mail-Verbindung können VertriebsConnect-Administratoren die E-Mail-Versand-Rate konfigurieren, wenn sie Gmail oder Exchange als Versand-Kanal verwenden, sodass die Übermittlungsrate der E-Mails an den Versand Kanal Provider die erzwungenen Grenzwerte nicht überschreitet.

Wenn die Grenzwerte durchgängig überschritten werden, kann dies manchmal als verdächtiges Verhalten des Versand Kanal Providers betrachtet werden, wodurch E-Mails fehlschlagen und manchmal sogar ein Konto deaktiviert wird.

**Hinweise/Highlights**

* Wird automatisch aktiviert, sobald ein Benutzer eine Verbindung zu Gmail oder Exchange herstellt
* Kann angepasst werden, wenn Sie die Einstellungen der Empfehlung an Ihre Anforderungen anpassen möchten
* Nur durch Google Mail oder Exchange gesendete Schildblätter werden nicht für den Kanal benutzerdefinierter Versand gedrosselt
* Die E-Mail-Verbindung schränkt die Warteschlangen für die einzelnen Benutzer einzeln ein, da jeder Benutzer über eine eigene Verbindung mit seinem E-Mail-Anbieter verfügt

**Konfigurieren der Einstellungen für die Einschränkung der E-Mail-Verbindung**

1. Klicken Sie auf das Zahnradsymbol und wählen Sie **Einstellungen**.

   ![](assets/email-connection-throttling-1.png)

1. Klicken Sie auf **Allgemein**.

   ![](assets/email-connection-throttling-2.png)

1. Geben Sie in der Karte &quot;Einschränken der E-Mail-Verbindung&quot;die gewünschte Stapelgröße der E-Mails ein, die an den E-Mail-Kanal-Provider gesendet werden.

   ![](assets/email-connection-throttling-3.png)

1. Legen Sie fest, wie lange gewartet werden soll, bevor jeder Stapel gesendet wird. In diesem Beispiel wählen wir 25 E-Mails alle 45 Sekunden.

   ![](assets/email-connection-throttling-4.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/email-connection-throttling-5.png)

Nachdem die Änderungen gespeichert wurden, werden alle Benutzer ihre E-Mails in Batches an ihr angeschlossenes Google Mail- oder Exchange-Konto zum Versand gesendet.

## E-Mail-Provider-Beschränkungen {#email-provider-limits}

**Outlook 365**

Geschäft/Unternehmen

* 10.000 pro Tag
* 30 pro Minute
* 500 Empfänger pro E-Mail

Weitere Informationen finden Sie hier.[](https://docs.microsoft.com/en-us/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#RecipientLimits)

**Gmail**

* 2000 pro Tag (500 für Test- und Kennzeichnungskonten)
* 2 E-Mails pro Sekunde (API-Limit)
* 2.000 Empfänger pro Nachricht (maximal 500 für externe Empfänger)

Weitere Informationen finden Sie hier.[](https://support.google.com/a/answer/166852?hl=en)

**Microsoft Exchange Server (2010, 2013)**

Beschränkungen werden von der IT-Abteilung des Unternehmens festgelegt, da der Server von der Organisation gehostet wird. Wenden Sie sich für weitere Informationen an den Netzwerk- oder Systemadministrator.

>[!MORELIKETHIS]
>
>* [Übersicht über Versand Kanal](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/delivery-channel-overview.md)
>* [E-Mail-Verbindung für Gmail-Benutzer](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [E-Mail-Verbindung für Outlook-Benutzer](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)

