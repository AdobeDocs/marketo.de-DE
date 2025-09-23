---
unique-page-id: 10096675
description: Erstellen untergeordneter Kampagnen und lokaler Assets - Marketo-Dokumente - Produktdokumentation
title: Erstellen untergeordneter Kampagnen und lokaler Assets
exl-id: 272105e1-43d6-455c-a533-aae65e859384
feature: Events
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 3%

---

# Erstellen untergeordneter Kampagnen und lokaler Assets {#create-child-campaigns-and-local-assets}

Erstellen Sie Ihre untergeordneten Kampagnen und lokalen Assets mit dem Design Studio.

## Landingpage und Formular {#landing-page-and-form}

Um sicherzustellen, dass Personen ordnungsgemäß bei ON24 registriert sind, müssen die folgenden Felder in Ihr Marketo-Formular aufgenommen werden:

* Vorname
* Nachname
* E-Mail-Adresse

Sie können auch die folgenden Felder auf ON24 pushen:

* Firmenname
* Jobtitel

Wenn der richtige Flussschritt zur Registrierungskampagne hinzugefügt wird, werden die Personen zu ON24 gepusht und als registriert markiert. Sie können dem Formular weitere Felder hinzufügen, und die Informationen werden in Marketo als Teil des Personendetaildatensatzes erfasst.

>[!CAUTION]
>
>Für eine erfolgreiche Integration müssen Sie entweder ein Marketo-Formular verwenden, um Ihre Mitarbeiter für die Veranstaltung zu registrieren, oder ein Nicht-Marketo-Formular mit der richtigen API-Integration, um Registrierungsdaten an Marketo zu senden.

## E-Mails und URL-Token {#emails-and-url-tokens}

Erstellen Sie die Einladungs-, Bestätigungs-, Follow-up- und Danksagungs-E-Mails mit Marketo.

## Marketo-Bestätigungs-E-Mail und URL-Token {#marketo-confirmation-email-and-url-token}

Verwenden Sie Marketo, um die Bestätigungs-E-Mail für Ihre Veranstaltung zu senden. Wenn sich eine Person registriert, erhält sie eine eindeutige URL, über die sie in das Ereignis eintreten kann.

>[!NOTE]
>
>Um Ihre Bestätigungs-E-Mail mit dieser eindeutigen URL zu füllen, verwenden Sie das folgende Token in Ihrer E-Mail: `{{member.webinar url}}`. Wenn Sie die Bestätigungs-URL senden, wird dieses Token automatisch zur eindeutigen Bestätigungs-URL der Person aufgelöst.
>
>Legen Sie den Typ Ihrer Bestätigungs-E **Mail auf** fest, um sicherzustellen, dass Personen, die sich registrieren, ihre Bestätigungsinformationen erhalten, auch wenn sie sich abgemeldet haben.

>[!TIP]
>
>Sie können ON24 so konfigurieren, dass Bestätigungs-, Erinnerungs- oder Follow-up-E-Mails gesendet werden. Weitere Informationen finden Sie auf [ON24](https://support.on24.com/hc/en-us/categories/26127314569115-Webcast-Elite){target="_blank"}Hilfeseite.

## Voraussetzungen für untergeordnete Kampagnen zur Registrierung {#registration-child-campaign-requirements}

Ereignisse enthalten eine oder mehrere untergeordnete Kampagnen, die alle zusammenarbeiten, um Personen durch die Programmstatus zu bewegen und die Leistung Ihres Ereignisses zu verfolgen.

Beispiele für untergeordnete Kampagnen sind eine Einladungskampagne, eine Registrierungskampagne und Folgekampagnen.

>[!CAUTION]
>
>Damit der Adapter seine Aufgabe erfüllen kann, MÜSSEN Sie eine Registrierungskampagne erstellen. Diese Kampagne muss von der Person ausgelöst werden, die ein Formular ausfüllt, und der erste Schritt muss den Programmstatus der Person in &quot;**&quot;**. Die Kampagne sendet dann eine Bestätigungs-E-Mail. Weitere Informationen finden Sie im Rest dieses Artikels.

**Anmeldung/Bestätigung (Trigger Campaign)**

* Intelligente Liste
* Trigger basierend auf **Formular ausfüllen**. Denken Sie daran, die Landingpage, auf der sich das Formular befindet, mithilfe von **Einschränkung hinzufügen** einzubeziehen, insbesondere wenn dasselbe Formular auf mehreren Landingpages verwendet wird.

>[!CAUTION]
>
>Sie müssen ein Marketo-Formular verwenden, um Ihre Personen für die Veranstaltung zu registrieren, oder ein Nicht-Marketo-Formular mit der richtigen API-Integration, um Registrierungsdaten an Marketo zu senden. Dies ist entscheidend für den Erfolg Ihrer Event-Partner-Integration.

>[!NOTE]
>
>Wenn Sie ein Marketo-Formular auf einer Landingpage verwenden, bei der es sich nicht um eine Marketo-Landingpage handelt, lautet Ihr Trigger **[!UICONTROL Formular ausfüllen]** mit dem [!UICONTROL Formularnamen].

![](assets/image2015-12-22-15-3a20-3a51.png)

**Fluss**

* **[!UICONTROL Programmstatus ändern]** - Auf Webinar setzen -> Registriert.

Dieser Flussschritt ist als ERSTER FLUSSSCHRITT beim Einrichten der untergeordneten Kampagne erforderlich. Wenn sich der Programmstatus einer Person in Registriert ändert, sendet Marketo die Registrierungsinformationen an ON24. Kein anderer Status überträgt die Person.

* **[!UICONTROL E-Mail]** - Bestätigungs-E-Mail. Legen Sie diese E **Mail auf &quot;**&quot; fest, damit Abgemeldete, die sich registriert haben, sie weiterhin erhalten.

Der **[!UICONTROL E-Mail senden]** Flussschritt MUSS der zweite Schritt sein. Die Bestätigungs-E-Mail enthält die `{{member.webinar url}}`, die mit Informationen gefüllt ist, die von ON24 an Marketo zurückgesendet werden.

![](assets/image2015-12-22-15-3a29-3a50.png)

>[!NOTE]
>
>Die Reihenfolge dieser Flussschritte ist aufgrund der Reihenfolge wichtig, in der die Aktionen in Marketo ausgeführt werden. Der **[!UICONTROL Programmstatus ändern]** sendet die Person zur Registrierung an ON24, und es wird eine eindeutige URL generiert. Danach können Sie mithilfe des `{{member.webinar URL}}`-Tokens die Bestätigungs-E-Mail versenden, die diese eindeutige URL enthält.
>
>Wenn der Person ein Registrierungsfehler zurückgegeben wird, erhält sie die E-Mail-Bestätigung nicht.

Ihr nächster Schritt besteht darin, [Ihre ON24-Ereignisintegration zu ](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Informationen zu Marketo ON24-Adapterereignissen](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
>* [Beispiel für die ON24-Ereignisintegration](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
>* [Grundlegendes zum Webinar-Programmstatus](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target="_blank"}
