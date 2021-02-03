---
unique-page-id: 10096675
description: Erstellen von untergeordneten Kampagnen und lokalen Elementen - Marketing Docs - Produktdokumentation
title: Untergeordnete Kampagnen und lokale Assets erstellen
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 0%

---


# Untergeordnete Kampagnen und lokale Elemente erstellen {#create-child-campaigns-and-local-assets}

Erstellen Sie untergeordnete Kampagnen und lokale Assets mit Design Studio.

## Landingpage und Formular {#landing-page-and-form}

Um sicherzustellen, dass Personen korrekt bei ON24 registriert sind, müssen die folgenden Felder in Ihrem Marketing-Formular enthalten sein:

* Vorname
* Nachname
* Email-Adresse

Sie können die folgenden Felder auch auf ON24 verschieben:

* Name der Firma
* Auftragstitel

Wenn der entsprechende Flussschritt zur Kampagne der Registrierung hinzugefügt wird, werden die Personen auf ON24 verschoben und als registriert markiert. Sie können dem Formular weitere Felder hinzufügen, und die Informationen werden in Marketo als Teil des Personendetaildatensatzes erfasst.

>[!CAUTION]
>
>Für eine erfolgreiche Integration müssen Sie entweder ein Marketo-Formular verwenden, um Ihre Mitarbeiter für das Ereignis zu registrieren, oder ein Nicht-Marketo-Formular mit der richtigen API-Integration, um Registrierungsdaten an Marketo zu senden.

## E-Mails und URL-Tokens {#emails-and-url-tokens}

Erstellen Sie die Einladung, Bestätigung, Follow-up und Dankeschön-E-Mails mit Marketo.

## E-Mail-Bestätigung und URL-Token {#marketo-confirmation-email-and-url-token}

Verwenden Sie Marketo, um die Bestätigungs-E-Mail für Ihr Ereignis zu senden. Wenn sich eine Person registriert, erhält sie eine eindeutige URL, die für die Eingabe des Ereignisses verwendet werden kann.

>[!NOTE]
>
>Um Ihre Bestätigungs-E-Mail mit dieser eindeutigen URL zu füllen, verwenden Sie das folgende Token in Ihrer E-Mail: `{{member.webinar url}}`. Wenn Sie die Bestätigungs-URL senden, wird dieses Token automatisch zur eindeutigen Bestätigungs-URL der Person aufgelöst.
>
>Stellen Sie den Typ Ihrer Bestätigungs-E-Mail auf **Operational** ein, um sicherzustellen, dass Personen, die sich registrieren, ihre Bestätigungsinformationen erhalten, auch wenn sie sich abmelden.

>[!TIP]
>
>Sie können ON24 so konfigurieren, dass es Bestätigungs-, Erinnerungs- oder Follow-up-E-Mails sendet. Weitere Informationen finden Sie auf der Hilfeseite [ON24](https://webcastelitehelp.on24.com).

## Voraussetzungen für die Kampagne des untergeordneten Registrierungsformulars {#registration-child-campaign-requirements}

Ereignis enthalten eine oder mehrere untergeordnete Kampagnen, die alle zusammen arbeiten, um Menschen durch die Programm-Status zu bewegen und die Leistung Ihres Ereignisses zu verfolgen.

Beispiele für untergeordnete Kampagnen sind eine Einladungs-Kampagne, eine Registrierungs-Kampagne und Kampagnen zur Weiterverfolgung.

>[!CAUTION]
>
>Damit der Adapter seinen Auftrag ausführen kann, MÜSSEN Sie eine Registrierungs-Kampagne erstellen. Diese Kampagne muss von der Person ausgelöst werden, die ein Formular ausfüllt. Der erste Schritt muss den Status des Programms der Person in **Registered** ändern. Die Kampagne sendet dann eine Bestätigungs-E-Mail. Weitere Informationen finden Sie in diesem Artikel.

**Registrierung/Bestätigung (Kampagne des Triggers)**

* Intelligente Liste
* Trigger basierend auf **Fügt Formular** aus. Stellen Sie sicher, dass Sie die Landingpage, auf der sich das Formular befindet, mit **Hinzufügen Constraint** einschließen, insbesondere wenn dasselbe Formular auf mehreren Landingpages verwendet wird.

>[!CAUTION]
>
>Sie müssen ein Marketo-Formular verwenden, um Ihre Personen für das Ereignis zu registrieren, oder ein Nicht-Marketo-Formular mit der richtigen API-Integration, um Registrierungsdaten an Marketo zu senden. Dies ist von entscheidender Bedeutung für den Erfolg Ihrer Ereignis-Partnerintegration.

>[!NOTE]
>
>Wenn Sie ein Marketo-Formular in einer Nicht-Marketo-Landingpage verwenden, lautet Ihr Trigger **Ausfüllen des Formulars** mit dem Formularbennamen.

![](assets/image2015-12-22-15-3a20-3a51.png)

**Fluss**

* **Ändern Sie den Status**  des Programms - Auf Webinar einstellen -> Registriert.

Dieser Flussschritt ist beim Einrichten der untergeordneten Kampagne als ERSTER FLOW-SCHRITT erforderlich. Wenn sich der Status des Programms einer Person in &quot;Registered&quot;ändert, setzt Marketo die Registrierungsinformationen auf ON24. Kein anderer Status wird die Person übertreiben.

* **E-Mail**  - Bestätigung per E-Mail senden. Stellen Sie diese E-Mail auf **Operational** ein, damit nicht abonnierte Personen, die sich registriert haben, sie weiterhin erhalten.

Der Schritt **E-Mail senden** MUSS der zweite Schritt sein. Die Bestätigungs-E-Mail enthält das `{{member.webinar url}}`, das mit Informationen gefüllt wird, die von ON24 an Marketo zurückgesendet werden.

![](assets/image2015-12-22-15-3a29-3a50.png)

>[!NOTE]
>
>Die Reihenfolge dieser Flussschritte ist wichtig, weil die Aktionen in Marketo ausgeführt werden. Der Schritt **Change Programm Status** sendet die Person zur Registrierung an ON24 und es wird eine eindeutige URL generiert. Danach können Sie die Bestätigungs-E-Mail mit dieser eindeutigen URL mit dem Token `{{member.webinar URL}}` senden.
>
>Wenn die Person mit einem Registrierungsfehler zurückgegeben wird, erhält sie keine E-Mail-Bestätigung.

Der nächste Schritt ist [Testen Sie Ihre ON24-Ereignis-Integration](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md).

>[!MORELIKETHIS]
>
>* [Ereignisse des Marketo ON24-Adapters](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
>* [Beispiel für eine ON24-Ereignis-Integration](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
>* [Erläuterungen zu Webinar-Programm-Status](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md)

