---
unique-page-id: 10096679
description: Beispielhafte ON24-Ereignisintegration - Marketo Docs - Produktdokumentation
title: Beispiel für eine ON24-Ereignisintegration
exl-id: 9d34d1bf-1ff8-4b26-906e-4a6bb9d5f3f6
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# Beispiel für eine ON24-Ereignisintegration {#example-on-event-integration}

Hier finden Sie ein Beispielereignis mit Kampagnen für ein ON24-Webinar. Stellen Sie beim Erstellen Ihres Ereignisses sicher, dass Sie Ihre Kampagnen testen, bevor Sie sie ausführen.

## Erstellen eines neuen Ereignisses in Marketingaktivitäten {#create-a-new-event-in-marketing-activities}

1. Wählen Sie **Neu** > **Neues Programm** aus.

   ![](assets/image2015-12-22-15-3a35-3a15.png)

1. Wählen Sie einen **Kampagnenordner** aus, in dem das Ereignis live sein soll.

   ![](assets/image2015-12-22-15-3a39-3a51.png)

1. Geben Sie einen **Namen** für das Ereignis ein.

   ![](assets/image2015-12-22-15-3a43-3a4.png)

1. Wählen Sie **Ereignis** als **Programmtyp** aus.

   ![](assets/image2015-12-22-15-3a44-3a41.png)

1. Wählen Sie **Webinar** als **Kanal** für das Ereignis aus.

   ![](assets/image2015-12-22-15-3a46-3a34.png)

1. Klicken Sie auf **Erstellen**.

   ![](assets/image2015-12-22-15-3a48-3a20.png)

## Einladen (Batch-Kampagne)  {#invite-batch-campaign}

* **Smart List** - Definieren Sie, wen Sie zum Ereignis einladen möchten.
* **Fluss**

   * E-Mail senden - Wenn es sich um eine lokale Asset-E-Mail handelt, wird die folgende Namenskonvention verwendet: EventName.EmailName. Sie können auch globale E-Mails verwenden.
   * Status ändern in Progression - Auf Webinar > Eingeladen einstellen.

* **Zeitplan** - Legt das Datum für den Versand der Einladung fest.

## Registrierung/Bestätigung (Trigger Campaign) {#registration-confirmation-trigger-campaign}

* **Smart List**

   * Trigger der Kampagne basierend auf **Ausfüllen des Formulars**. Stellen Sie sicher, dass Sie die Landingpage einschließen, auf der das Formular ausgeführt wird, indem Sie **Beschränkung hinzufügen** verwenden, insbesondere wenn das Formular auf mehreren Landingpages verwendet wird.

>[!CAUTION]
>
>Sie müssen ein Marketo-Formular verwenden, um Personen für die Veranstaltung zu registrieren, oder ein Nicht-Marketo-Formular mit der entsprechenden API-Integration, um Registrierungsdaten an Marketo zu senden. Dies ist von entscheidender Bedeutung für den Erfolg Ihrer Partner-Integration. **HINWEIS**: Wenn Sie ein Marketo-Formular auf einer Nicht-Marketo-Landingpage verwenden, lautet Ihr Trigger **Formular ausfüllen** mit dem Formularnamen.

![](assets/image2015-12-22-15-3a50-3a22.png)

* **Fluss**

   * **Status in Progression ändern** - Setzen Sie es auf Webinar > Registriert. **VORSICHT**: Dieser Flussschritt ist beim Einrichten Ihrer untergeordneten Kampagne erforderlich. Wenn sich der Fortschritt einer Person in &quot;**Registered**&quot; ändert, überträgt Marketo die Registrierungsinformationen an ON24.

   * **E-Mail senden** - Bestätigungs-E-Mail (auf **Operativ** gesetzt, damit abgemeldete Benutzer, die sich registriert haben, diese weiterhin erhalten).

![](assets/image2015-12-22-15-3a52-3a9.png)

**HINWEIS**: Wenn die Person mit einem Registrierungsfehler zurückgegeben wird, erhält sie keine E-Mail-Bestätigung.

## Erinnerung (Batch-Kampagne) {#reminder-batch-campaign}

* **Smart List** - Filtern Sie mit **Member of Program** und legen Sie den Status auf **Registered** fest.

* **Fluss** - E-Mail senden (Erinnerungsmail).

**HINWEIS**: Sie können eine ähnliche Kampagne verwenden, um eine *andere* Follow-up-E-Mail an Personen zu senden, die eingeladen wurden, sich aber noch nicht registriert haben.

## Folgenachrichten-Kampagnen (Batch- oder Trigger-Kampagnen) {#follow-up-campaign-batch-or-trigger-campaign}

* **Smart List** - Trigger basierend auf Änderungen im Programmstatus.

![](assets/image2015-12-22-15-3a57-3a25.png)

* **Fluss** - E-Mail senden. Verwenden Sie Optionen, um je nach Programmstatus unterschiedliche E-Mails zu versenden.

![](assets/ten.png)

>[!MORELIKETHIS]
>
>[Grundlegendes zu Marketo ON24-Adapterereignissen](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
