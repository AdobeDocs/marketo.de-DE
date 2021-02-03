---
unique-page-id: 10096656
description: Erstellen Sie ein Ereignis mit dem Marketo ON24 Adapter - Marketing Docs - Produktdokumentation
title: Erstellen eines Ereignisses mit dem Marketo ON24-Adapter
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---


# Erstellen Sie ein Ereignis mit dem Marketo ON24-Adapter {#create-an-event-with-the-marketo-on-adapter}

## Bevor Sie mit {#before-you-begin} beginnen

Sie sollten sich mit den Bausteinen und der empfohlenen Reihenfolge für die Erstellung von Ereignissen in Marketo auskennen. Sie sollten außerdem über Kenntnisse der folgenden Marketo-Konzepte verfügen:

* [Marketo-](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md) Programme und -Ereignisse und ihre Unterschiede
* [Kanal](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)
* [Lokale Assets](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md)
* [Status ](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md) von untergeordneten Kampagnen und  [Programmen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md)

>[!NOTE]
>
>Weitere Informationen zu Marketing-APIs finden Sie in der [Marketing-API-Dokumentation](https://developers.marketo.com/documentation/rest/).

## Voraussetzungen {#prerequisites}

Zur Verwendung der Integration von Marketo ON24 sind folgende Anforderungen erforderlich:

* **Abonnement zu ON24 Webcasts**  - Wenn Sie kein aktuelles Abonnement haben, wenden Sie sich direkt an ON24. **HINWEIS**: ON24 Hosted Edition ist erforderlich. ON24 Ereignis Management ist nicht erforderlich.

* **Administratorrechte auf ON24**  - Sie benötigen diese, um diesen Connector zu verwenden und Gäste im ON24-System zu erstellen.
* **ON24-Verbindungsdaten**  - Sie müssen diese Informationen in Marketing eingeben, um die Integration zu aktivieren: Benutzername, Kennwort, Client-ID und Client-Schlüssel. Wenden Sie sich an Ihren ON24-Kundenbetreuer oder an den ON24-Support, wenn Sie Hilfe bei Ihren Anmeldeinformationen benötigen.
* **Registrierungsformular**  - Verwenden Sie ein Marketo-Formular oder ein Nicht-Marketo-Formular zusammen mit der richtigen API, um sicherzustellen, dass Registrierungsdaten und Registrierungsdaten an Marketo weitergeleitet werden.
* **Kampagne**  des untergeordneten Registrierungsformulars - Eine untergeordnete Kampagne zur Registrierung in Ihrem Marketing-Ereignis muss ordnungsgemäß erstellt und konfiguriert werden, damit Ihre Ereignis-Partnerintegration funktioniert.

## Prozessfluss {#process-flow}

Führen Sie die folgenden Schritte aus, um ein Ereignis mit dem Marketo On24-Adapter zu erstellen:

1. [Geben Sie Ihre ON24-Anmeldeinformationen in Marketing ein](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/enter-your-on24-credentials-in-marketo.md)
1. [Webinar-Ereignis in ON24 erstellen](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md)
1. [Ereignis-Einstellungen konfigurieren und Marketing mit Ihrem Webinar synchronisieren](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md)
1. [Untergeordnete Kampagnen und lokale Assets erstellen](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md)
1. [On24-Ereignis-Integration testen](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md)
1. [Beispiel für eine ON24-Ereignis-Integration](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
1. [Erläuterungen zu Webinar-Programm-Status](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md)
1. [ON24-Ereignis-Registrierungsaktualisierungen](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md)
