---
unique-page-id: 10096656
description: Erstellen Sie ein Ereignis mit dem Marketo ON24-Adapter - Marketo Docs - Produktdokumentation
title: Erstellen eines Ereignisses mit dem Marketo ON24-Adapter
exl-id: a240ff72-b12f-4e3a-8e14-94fddb02f944
source-git-commit: 40cfdddac66b7cd90e33bedf11888a7c5e3b38c9
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 1%

---

# Erstellen eines Ereignisses mit dem Marketo ON24-Adapter {#create-an-event-with-the-marketo-on-adapter}

>[!IMPORTANT]
>
>Ab August 2022 unterstützt ON24 keine neuen Marketo-Integrationen mehr. Die Informationen in diesem Artikel gelten nur für bestehende Benutzer.

Sie sollten sich mit den Bausteinen und der empfohlenen Reihenfolge für die Erstellung von Ereignissen in Marketo auskennen. Außerdem sollten Sie über Kenntnisse der folgenden Marketo-Konzepte verfügen:

* [Marketo-Programme](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md) sowie Ereignisse und die Unterschiede zwischen ihnen
* [Kanäle](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)
* [Lokale Assets](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md)
* [Untergeordnete Kampagnen](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md) und [Programmstatus](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md)

>[!NOTE]
>
>Weitere Informationen finden Sie unter [Dokumentation zur Marketo API](https://developers.marketo.com/documentation/rest/) Weitere Informationen zu Marketo-APIs.

## Voraussetzungen {#prerequisites}

Für die Verwendung der Marketo ON24-Integration ist Folgendes erforderlich:

* **Abonnement für ON24-Webcasts** - Wenn Sie kein aktuelles Abonnement haben, kontaktieren Sie ON24 direkt. **NOTE**: ON24 Hosted Edition ist erforderlich. ON24-Ereignisverwaltung ist nicht erforderlich.

* **Administratorrechte für ON24** - Sie benötigen diesen Connector, um Gäste im ON24-System zu erstellen.
* **ON24-Verbindungsdaten** - Sie müssen diese Informationen in Marketo eingeben, um die Integration zu aktivieren: Benutzername, Kennwort, Client-ID und Client-Schlüssel. Wenden Sie sich an Ihren ON24-Kundenbetreuer oder ON24-Support, wenn Sie Hilfe bei Ihren Anmeldedaten benötigen.
* **Registrierungsformular** - Verwenden Sie ein Marketo-Formular oder ein Nicht-Marketo-Formular zusammen mit der entsprechenden API, um sicherzustellen, dass Registrierungsdaten und Registrierungsinformationen an Marketo weitergeleitet werden.
* **Untergeordnete Registrierungskampagne** - Eine untergeordnete Registrierungskampagne in Ihrem Marketo-Ereignis muss ordnungsgemäß erstellt und konfiguriert sein, damit Ihre Partner-Integration funktioniert.

## Prozessfluss {#process-flow}

Führen Sie die folgenden Schritte aus, um ein Ereignis mit dem Marketo On24-Adapter zu erstellen:

1. [Webinar-Veranstaltung in ON24 erstellen](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md)
1. [Konfigurieren von Ereigniseinstellungen und Synchronisieren von Marketo mit Ihrem Webinar](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md)
1. [Erstellen untergeordneter Kampagnen und lokaler Assets](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md)
1. [Testen der ON24-Ereignisintegration](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md)
1. [Beispiel für eine ON24-Ereignisintegration](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
1. [Grundlegendes zum Webinar-Programmstatus](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md)
1. [Aktualisierungen der Ereignisregistrierung in ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md)
