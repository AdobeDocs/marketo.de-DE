---
unique-page-id: 10096675
description: Erstellen von untergeordneten Kampagnen und lokalen Assets - Marketo Docs - Produktdokumentation
title: Erstellen untergeordneter Kampagnen und lokaler Assets
exl-id: 272105e1-43d6-455c-a533-aae65e859384
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 1%

---

# Erstellen untergeordneter Kampagnen und lokaler Assets {#create-child-campaigns-and-local-assets}

Erstellen Sie Ihre untergeordneten Kampagnen und lokalen Assets mit Design Studio.

## Landingpage und Formular {#landing-page-and-form}

Um sicherzustellen, dass Personen ordnungsgemäß bei ON24 registriert sind, müssen die folgenden Felder in Ihr Marketo-Formular eingefügt werden:

* Vorname
* Nachname
* E-Mail-Adresse

Sie können auch die folgenden Felder an ON24 senden:

* Unternehmensname
* Jobtitel

Wenn der richtige Flussschritt zur Registrierungskampagne hinzugefügt wird, werden die Personen auf ON24 gepusht und als registriert markiert. Sie können dem Formular weitere Felder hinzufügen. Die Informationen werden dann in Marketo als Teil des Personendetaildatensatzes erfasst.

>[!CAUTION]
>
>Für eine erfolgreiche Integration müssen Sie entweder ein Marketo-Formular verwenden, um Ihre Personen für das Ereignis zu registrieren, oder ein Nicht-Marketo-Formular mit der entsprechenden API-Integration, um Registrierungsdaten an Marketo zu senden.

## E-Mails und URL-Token {#emails-and-url-tokens}

Erstellen Sie die Einladungs-, Bestätigungs-, Follow-up- und Danksagungs-E-Mails mit Marketo.

## Marketo-Bestätigungs-E-Mail und URL-Token {#marketo-confirmation-email-and-url-token}

Verwenden Sie Marketo , um die Bestätigungs-E-Mail für Ihr Ereignis zu senden. Wenn sich eine Person registriert, erhält sie eine eindeutige URL, über die sie das Ereignis aufruft.

>[!NOTE]
>
>Um Ihre Bestätigungs-E-Mail mit dieser eindeutigen URL zu füllen, verwenden Sie das folgende Token in Ihrer E-Mail: `{{member.webinar url}}`. Wenn Sie die Bestätigungs-URL senden, wird dieses Token automatisch zur eindeutigen Bestätigungs-URL der Person aufgelöst.
>
>Stellen Sie den Typ Ihrer Bestätigungs-E-Mail auf **Operativ** ein, um sicherzustellen, dass Personen, die sich registrieren, ihre Bestätigungsinformationen erhalten, selbst wenn sie sich abgemeldet haben.

>[!TIP]
>
>Sie können ON24 so konfigurieren, dass Bestätigungs-, Erinnerungsschreiben- oder Folgenachrichten gesendet werden. Weitere Informationen finden Sie auf der [ON24 Help Site](https://www.on24.com/live-webcast-elite/){target="_blank"} .

## Voraussetzungen für die Registrierung untergeordneter Kampagnen {#registration-child-campaign-requirements}

Ereignisse enthalten eine oder mehrere untergeordnete Kampagnen, die alle zusammenarbeiten, um Personen durch den Programmstatus zu bewegen und die Leistung Ihres Ereignisses zu verfolgen.

Beispiele für untergeordnete Kampagnen sind eine Einladungskampagne, eine Registrierungs-Kampagne und Folgekampagnen.

>[!CAUTION]
>
>Damit der Adapter seinen Auftrag erledigen kann, MÜSSEN Sie eine Registrierungs-Kampagne erstellen. Diese Kampagne muss von der Person ausgelöst werden, die ein Formular ausfüllt. Im ersten Schritt muss der Programmstatus der Person in **Registered** geändert werden. Die Kampagne sendet dann eine Bestätigungs-E-Mail. Weitere Informationen finden Sie im Rest dieses Artikels.

**Registrierung/Bestätigung (Trigger Campaign)**

* Smart List
* Trigger basierend auf **Ausfüllformular ausfüllen**. Stellen Sie sicher, dass Sie die Landingpage einschließen, auf der das Formular ausgeführt wird, indem Sie **Beschränkung hinzufügen** verwenden, insbesondere wenn dasselbe Formular auf mehreren Landingpages verwendet wird.

>[!CAUTION]
>
>Sie müssen ein Marketo-Formular verwenden, um Ihre Personen für die Veranstaltung zu registrieren, oder ein Nicht-Marketo-Formular mit der entsprechenden API-Integration, um Registrierungsdaten an Marketo zu senden. Dies ist von entscheidender Bedeutung für den Erfolg Ihrer Partner-Integration.

>[!NOTE]
>
>Wenn Sie ein Marketo-Formular auf einer Nicht-Marketo-Landingpage verwenden, lautet Ihr Trigger **Formular ausfüllen** mit dem Formularbennamen.

![](assets/image2015-12-22-15-3a20-3a51.png)

**Fluss**

* **Programmstatus ändern** - Auf Webinar festlegen -> Eingezeichnet.

Dieser Flussschritt ist als ERSTER FLUSS-SCHRITT beim Einrichten Ihrer untergeordneten Kampagne erforderlich. Wenn sich der Programmstatus einer Person in Registered ändert, überträgt Marketo die Registrierungsinformationen an ON24. Kein anderer Status wird die Person überstürzen.

* **E-Mail senden** - Bestätigungs-E-Mail. Setzen Sie diese E-Mail auf &quot;**Operativ**&quot;, damit abgemeldete Benutzer, die sich angemeldet haben, sie weiterhin erhalten.

Der Schritt &quot;**E-Mail senden**&quot; MUSS der zweite Schritt sein. Die Bestätigungs-E-Mail enthält den Wert &quot;`{{member.webinar url}}`&quot;, der mit Informationen gefüllt ist, die von ON24 an Marketo zurückgesendet werden.

![](assets/image2015-12-22-15-3a29-3a50.png)

>[!NOTE]
>
>Die Reihenfolge dieser Flussschritte ist aufgrund der Reihenfolge, in der Aktionen in Marketo ausgeführt werden, wichtig. Der Schritt **Programmstatus ändern** sendet die Person zur Registrierung an ON24 und es wird eine eindeutige URL generiert. Danach können Sie die Bestätigungs-E-Mail mit dieser eindeutigen URL mithilfe des Tokens `{{member.webinar URL}}` versenden.
>
>Wenn die Person mit einem Registrierungsfehler zurückgegeben wird, erhält sie keine E-Mail-Bestätigung.

Der nächste Schritt besteht darin, die ON24-Ereignisintegration [zu testen](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Grundlegendes zu Marketo ON24-Adapterereignissen](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
>* [Beispiel für ON24-Ereignisintegration](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
>* [Grundlegendes zum Programmstatus eines Webinars](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target="_blank"}
