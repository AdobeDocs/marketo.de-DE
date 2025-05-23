---
unique-page-id: 10096656
description: Erstellen eines Ereignisses mit dem Marketo ON24-Adapter - Marketo-Dokumentation - Produktdokumentation
title: Erstellen eines Ereignisses mit dem Marketo ON24-Adapter
exl-id: a240ff72-b12f-4e3a-8e14-94fddb02f944
feature: Events
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# Erstellen eines Ereignisses mit dem Marketo ON24-Adapter {#create-an-event-with-the-marketo-on-adapter}

Sie sollten mit den Bausteinen und der empfohlenen Reihenfolge zum Erstellen von Ereignissen in Marketo vertraut sein. Außerdem sollten Sie praktische Kenntnisse der folgenden Marketo-Konzepte haben:

* [Marketo](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target="_blank"}Programme und -Ereignisse und die Unterschiede zwischen ihnen
* [Kanäle](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}
* [Lokaler Assets](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md){target="_blank"}
* [Untergeordnete Kampagnen](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target="_blank"} und [Programmstatus](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md){target="_blank"}

>[!NOTE]
>
>Weitere Informationen zu Marketo-APIs finden [&#128279;](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/rest/rest-api){target="_blank"} in der Dokumentation zur Marketo-APIs.

## Voraussetzungen {#prerequisites}

Für die Verwendung der Marketo ON24-Integration ist Folgendes erforderlich:

* **Abonnement für ON24-Webcasts** - Wenn Sie noch kein aktuelles Abonnement haben, wenden Sie sich direkt an ON24. **HINWEIS**: ON24 Hosted Edition ist erforderlich. Die ON24-Ereignisverwaltung ist nicht erforderlich.

* **Administratorrechte für ON24** - Sie benötigen diese, um diesen Connector zu verwenden und Gäste im ON24-System zu erstellen.
* **ON24-**: Sie müssen diese Informationen in Marketo eingeben, um die Integration zu aktivieren: Benutzername, Kennwort, Client-ID und Client-Schlüssel. Wenden Sie sich an Ihren ON24-Kundenbetreuer oder an den ON24-Support, wenn Sie Hilfe zu Ihren Anmeldedaten benötigen.
* **Registrierungsformular** - Verwenden Sie ein Marketo-Formular oder ein Nicht-Marketo-Formular zusammen mit der richtigen API, um sicherzustellen, dass Registrierungsdaten und Informationen zu Registrierenden an Marketo übergeben werden.
* **Untergeordnete Kampagne zur Registrierung** - Sie müssen eine untergeordnete Registrierungskampagne in Ihrem Marketo-Ereignis erstellen und ordnungsgemäß konfiguriert haben, damit Ihre Event Partner-Integration funktioniert.

## Prozessablauf {#process-flow}

Führen Sie die folgenden Schritte aus, um mit dem Marketo On24-Adapter ein Ereignis zu erstellen:

1. [Erstellen Sie Ihre Webinar-Veranstaltung in ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md){target="_blank"}
1. [Ereigniseinstellungen konfigurieren und Marketo mit Ihrem Webinar synchronisieren](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target="_blank"}
1. [Erstellen von untergeordneten Kampagnen und lokalen Assets](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md){target="_blank"}
1. [Testen der ON24-Ereignisintegration](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target="_blank"}
1. [Beispiel für die ON24-Ereignisintegration](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
1. [Grundlegendes zum Webinar-Programmstatus](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target="_blank"}
1. [On24-Aktualisierungen zur Ereignisregistrierung](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target="_blank"}
