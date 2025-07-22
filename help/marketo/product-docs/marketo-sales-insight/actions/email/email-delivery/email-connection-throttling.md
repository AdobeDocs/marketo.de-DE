---
description: Drosselung der E-Mail-Verbindung - Marketo-Dokumente - Produktdokumentation
title: Drosselung der E-Mail-Verbindung
exl-id: 02450a1e-5b30-4057-b204-19fab1a7d6c9
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Drosselung der E-Mail-Verbindung {#email-connection-throttling}

Die Integration Ihres [!DNL Sales Connect]-Kontos zum Versand über [!DNL Exchange]- oder Gmail-E-Mail-Anbieter bietet eine optimierte Einrichtung und optimiert die E-Mail-Zustellbarkeit für 1:1-Verkaufskommunikation. Um jedoch die Systemintegrität und die Sicherheit der Konten zu gewährleisten, setzen Gmail und [!DNL Exchange] Grenzwerte für den E-Mail-Versand durch. Diese Obergrenzen können nach Ermessen des Anbieters erhöht oder gesenkt werden.

## Drosselung der E-Mail-Verbindung (Beta) {#email-connection-throttling-beta}

Mit der Drosselung der E-Mail-Verbindung können Sales Connect-Administratoren die Versandrate von E-Mails konfigurieren, wenn sie Gmail oder Exchange als Versandkanal verwenden, sodass die Rate, mit der E-Mails an den Versandkanalanbieter übergeben werden, die erzwungenen Grenzwerte nicht überschreitet.

Wenn Limits durchgängig überschritten werden, kann dies manchmal als verdächtiges Verhalten des Versandkanalanbieters angesehen werden, was dazu führt, dass E-Mails fehlschlagen und manchmal sogar ein Konto deaktiviert wird.

**Hinweise/Highlights**

* Automatisch aktiviert, sobald ein Benutzer eine Verbindung zu Gmail oder [!DNL Exchange] herstellt
* Kann angepasst werden, wenn Sie die Einstellungen von der Empfehlung ausgehend entsprechend Ihren Anforderungen erhöhen oder verringern möchten
* Drosselt nur über Gmail oder [!DNL Exchange] gesendete E-Mails, nicht jedoch den benutzerdefinierten Versandkanal
* Die Drosselung der E-Mail-Verbindung stellt für jeden einzelnen Benutzer separate E-Mails in eine Warteschlange, da jeder Benutzer eine eigene Verbindung mit seinem E-Mail-Anbieter hat

**Konfigurieren der Drosselungseinstellungen für Ihre E-Mail-Verbindung**

1. Klicken Sie auf das Zahnradsymbol und wählen Sie **[!UICONTROL Einstellungen]** aus.

   ![](assets/email-connection-throttling-1.png)

1. Klicken [!UICONTROL  unter &quot;]&quot; auf **[!UICONTROL Allgemein]**.

   ![](assets/email-connection-throttling-2.png)

1. Klicken Sie auf der rechten Seite in der Karte „E-Mail-Verbindungsbegrenzung“ auf den Schieberegler **[!UICONTROL E-Mail]** Drosselung aktivieren.

   ![](assets/email-connection-throttling-3.png)

1. Geben Sie auf der rechten Seite in der Karte Drosselung der E-Mail-Verbindung die gewünschte Batch-Größe der E-Mails ein, die an den E-Mail-Kanalanbieter gesendet werden.

   ![](assets/email-connection-throttling-4.png)

1. Die Wartezeit festlegen, bevor jeder Batch gesendet wird. In diesem Beispiel wählen wir 25 E-Mails alle 45 Sekunden.

   ![](assets/email-connection-throttling-5.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/email-connection-throttling-6.png)

Mit den gespeicherten Änderungen werden alle Benutzer ihre E-Mails in Batches an ihr verbundenes Gmail- oder [!DNL Exchange]-Konto senden lassen, um sie zu versenden.

## Beschränkungen für E-Mail-Anbieter {#email-provider-limits}

**[!DNL Outlook 365]**

Unternehmen/Unternehmen

* 10.000 pro Tag
* 30 pro Minute
* 500 Empfänger pro E-Mail

Weitere Informationen [finden Sie hier](https://docs.microsoft.com/en-us/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#RecipientLimits).

**Gmail**

* 2000 pro Tag (500 für Testkonten und gekennzeichnete Konten)
* 2 E-Mails pro Sekunde (API-Limit)
* 2.000 Empfänger pro Nachricht (maximal 500 für externe Empfänger)

Weitere Informationen [finden Sie hier](https://support.google.com/a/answer/166852?hl=en).

**[!DNL Microsoft Exchange Server (2010, 2013)]**

Einschränkungen werden von der IT-Abteilung des Unternehmens festgelegt, da der Server von dem Unternehmen gehostet wird. Weitere Informationen erhalten Sie vom Netzwerk- oder Systemadministrator.

>[!MORELIKETHIS]
>
>* [Versandkanal - Übersicht](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/delivery-channel-overview.md)
>* [E-Mail-Verbindung für Gmail-Benutzer](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [E-Mail-Verbindung für Outlook-Benutzer](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
