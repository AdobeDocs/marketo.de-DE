---
unique-page-id: 10096679
description: Beispielhafte ON24-Ereignisintegration - Marketo Docs - Produktdokumentation
title: Beispiel für eine ON24-Ereignisintegration
exl-id: 9d34d1bf-1ff8-4b26-906e-4a6bb9d5f3f6
source-git-commit: 40cfdddac66b7cd90e33bedf11888a7c5e3b38c9
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 1%

---

# Beispiel für eine ON24-Ereignisintegration {#example-on-event-integration}

>[!IMPORTANT]
>
>Ab August 2022 unterstützt ON24 keine neuen Marketo-Integrationen mehr. Die Informationen in diesem Artikel gelten nur für bestehende Benutzer.

Hier finden Sie ein Beispielereignis mit Kampagnen für ein ON24-Webinar. Stellen Sie beim Erstellen Ihres Ereignisses sicher, dass Sie Ihre Kampagnen testen, bevor Sie sie ausführen.

## Erstellen eines neuen Ereignisses in Marketingaktivitäten {#create-a-new-event-in-marketing-activities}

1. Auswählen **Neu** > **Neues Programm**.

   ![](assets/image2015-12-22-15-3a35-3a15.png)

1. Wählen Sie eine **Kampagnenordner** wo das Ereignis live sein wird.

   ![](assets/image2015-12-22-15-3a39-3a51.png)

1. Geben Sie einen **Name** für das Ereignis.

   ![](assets/image2015-12-22-15-3a43-3a4.png)

1. Auswählen **Ereignis** als **Programmtyp**.

   ![](assets/image2015-12-22-15-3a44-3a41.png)

1. Auswählen **Webinar** als **Kanal** für das Ereignis.

   ![](assets/image2015-12-22-15-3a46-3a34.png)

1. Klicken Sie auf **Erstellen**.

   ![](assets/image2015-12-22-15-3a48-3a20.png)

## Einladen (Batch-Kampagne)  {#invite-batch-campaign}

* **Smart List** - Definieren Sie, wen Sie zur Veranstaltung einladen.
* **Flow**

   * E-Mail senden - Wenn es sich um eine lokale Asset-E-Mail handelt, wird die folgende Namenskonvention verwendet: EventName.EmailName. Sie können auch globale E-Mails verwenden.
   * Status ändern in Progression - Auf Webinar > Eingeladen einstellen.

* **Zeitplan** - Legen Sie das Datum für den Versand der Einladung fest.

## Registrierung/Bestätigung (Trigger Campaign) {#registration-confirmation-trigger-campaign}

* **Intelligente Liste**

   * Trigger der Kampagne basierend auf **Formular ausfüllen**. Stellen Sie sicher, dass Sie die Landingpage einschließen, auf der das Formular aktiv ist, indem Sie **Beschränkung hinzufügen**, insbesondere wenn das Formular auf mehreren Landingpages verwendet wird.

>[!CAUTION]
>
>Sie müssen ein Marketo-Formular verwenden, um Personen für die Veranstaltung zu registrieren, oder ein Nicht-Marketo-Formular mit der entsprechenden API-Integration, um Registrierungsdaten an Marketo zu senden. Dies ist von entscheidender Bedeutung für den Erfolg Ihrer Partner-Integration. **NOTE**: Wenn Sie ein Marketo-Formular auf einer Landingpage ohne Marketo verwenden, wird Ihr Trigger **Formular ausfüllen** mit dem Formularnamen.

![](assets/image2015-12-22-15-3a50-3a22.png)

* **Fluss**

   * **Änderungsstatus in Progression** - Auf Webinar > Registriert einstellen. **VORSICHT**: Dieser Flussschritt ist beim Einrichten Ihrer untergeordneten Kampagne erforderlich. Wenn sich der Fortschritt einer Person in **Angemeldet**&#x200B;überträgt Marketo die Registrierungsinformationen an ON24.

   * **E-Mail senden** - Bestätigungs-E-Mail (festgelegt auf **Betrieb** sodass abgemeldete Personen, die sich registriert haben, diese noch erhalten).

![](assets/image2015-12-22-15-3a52-3a9.png)

**NOTE**: Wenn die Person mit einem Registrierungsfehler zurückgegeben wird, erhält sie keine E-Mail-Bestätigung.

## Erinnerung (Batch-Kampagne) {#reminder-batch-campaign}

* **Smart List** - Filtern mit **Programmteilnehmer** und legen Sie den Status auf **Angemeldet**.

* **Fluss** - E-Mail senden (Reminder Email).

**NOTE**: Sie können eine ähnliche Kampagne verwenden, um eine *distinct* Follow-up-E-Mail an eingeladene Personen, die sich aber noch nicht registriert haben.

## Folgenachrichten-Kampagnen (Batch- oder Trigger-Kampagnen) {#follow-up-campaign-batch-or-trigger-campaign}

* **Smart List** - Trigger basierend auf Änderungen des Programmstatus.

![](assets/image2015-12-22-15-3a57-3a25.png)

* **Fluss** - E-Mail senden. Verwenden Sie Optionen, um je nach Programmstatus unterschiedliche E-Mails zu versenden.

![](assets/ten.png)

>[!MORELIKETHIS]
>
>[Grundlegendes zu Marketo ON24-Adapterereignissen](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
