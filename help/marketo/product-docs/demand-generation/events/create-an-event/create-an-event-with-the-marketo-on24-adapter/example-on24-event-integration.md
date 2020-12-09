---
unique-page-id: 10096679
description: Beispiel für eine ON24-Ereignis-Integration - Marketing Docs - Produktdokumentation
title: Beispiel für eine ON24-Ereignis-Integration
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---


# Beispiel für eine ON24-Ereignis-Integration {#example-on-event-integration}

Hier ist ein Beispiel für ein Ereignis, einschließlich Kampagnen, für ein ON24-Webinar. Stellen Sie beim Erstellen Ihres Ereignisses sicher, dass Sie Ihre Kampagnen vor dem Ausführen testen.

## Neues Ereignis in Marketing-Aktivitäten erstellen {#create-a-new-event-in-marketing-activities}

1. Wählen Sie **Neu** > **Neues Programm**.

   ![](assets/image2015-12-22-15-3a35-3a15.png)

1. Wählen Sie einen **Kampagnen-Ordner** aus, in dem das Ereignis live geschaltet werden soll.

   ![](assets/image2015-12-22-15-3a39-3a51.png)

1. Geben Sie einen **Namen** für das Ereignis ein.

   ![](assets/image2015-12-22-15-3a43-3a4.png)

1. Wählen Sie **Ereignis **als **Programm-Typ**.

   ![](assets/image2015-12-22-15-3a44-3a41.png)

1. Wählen Sie **Webinar **als **Kanal **für das Ereignis.

   ![](assets/image2015-12-22-15-3a46-3a34.png)

1. Klicken Sie auf **Erstellen**.

   ![](assets/image2015-12-22-15-3a48-3a20.png)

## Einladung (Batch-Kampagne)  {#invite-batch-campaign}

* **Intelligente Liste** - Definieren Sie, wen Sie zum Ereignis einladen möchten.
* **Fluss**

   * E-Mail senden - Wenn es sich um eine E-Mail mit einem lokalen Asset handelt, gilt folgende Benennungsregel: EventName.EmailName. Sie können auch globale E-Mails verwenden.
   * Status in Progression ändern - Auf Webinar > Eingeladen festlegen.

* **Plan** : Legen Sie das Datum für den Versand der Einladung fest.

## Registrierung/Bestätigung (Auslöser-Kampagne) {#registration-confirmation-trigger-campaign}

* **Intelligente Liste**

   * Auslösen der Kampagne anhand des Formulars **&quot;Ausfüllen&quot;**. Stellen Sie sicher, dass Sie die Landingpage einschließen, die das Formular ausfüllt, indem Sie **Hinzufügen Einschränkung** verwenden, insbesondere wenn das Formular auf mehreren Landingpages verwendet wird.

>[!CAUTION]
>
>Sie müssen ein Marketo-Formular verwenden, um Personen für das Ereignis zu registrieren, oder ein Nicht-Marketo-Formular mit der richtigen API-Integration, um Registrierungsdaten an Marketo zu senden. Dies ist von entscheidender Bedeutung für den Erfolg Ihrer Ereignis-Partnerintegration. **HINWEIS**: Wenn Sie ein Marketo-Formular für eine Nicht-Marketo-Landingpage verwenden, wird als Auslöser **das Ausfüllen des Formulars** mit dem Formularnamen verwendet.

![](assets/image2015-12-22-15-3a50-3a22.png)

* **Fluss**

   * **Status in Progression** ändern - Auf Webinar > Registriert einstellen. **VORSICHT**: Dieser Flussschritt ist beim Einrichten der untergeordneten Kampagne erforderlich. Wenn sich der Status des Fortschritts einer Person in &quot; **Registriert**&quot;ändert, setzt Marketo die Registrierungsinformationen auf ON24.

   * **E-Mail** senden - Bestätigungs-E-Mail (auf &quot; **Operational** &quot;eingestellt, damit nicht abonnierte Personen, die sich registriert haben, diese immer noch erhalten).

![](assets/image2015-12-22-15-3a52-3a9.png)

**HINWEIS**: Wenn die Person mit einem Registrierungsfehler zurückgegeben wird, erhält sie keine E-Mail-Bestätigung.

## Erinnerung (Batch-Kampagne) {#reminder-batch-campaign}

* **Intelligente Liste** - Filtern Sie nach dem **Mitglied des Programms** und legen Sie den Status auf &quot; **Registriert**&quot;fest.

* **Fluss** - E-Mail senden (Erinnerungsmail).

**HINWEIS**: Sie können eine ähnliche Kampagne verwenden, um eine *andere* Follow-up-E-Mail an eingeladene, aber noch nicht registrierte Benutzer zu senden.

## Follow-up-Kampagne (Stapel- oder Auslöser-Kampagne) {#follow-up-campaign-batch-or-trigger-campaign}

* **Intelligente Liste** - Auslöser basierend auf Änderungen im Programm-Status.

![](assets/image2015-12-22-15-3a57-3a25.png)

* **Fluss** - E-Mail senden. Verwenden Sie Auswahlmöglichkeiten, um je nach Programm verschiedene E-Mails zu senden.

![](assets/ten.png)

>[!MORELIKETHIS]
>
>* [Ereignisse des Marketo ON24-Adapters](understanding-marketo-on24-adapter-events.md)

>



