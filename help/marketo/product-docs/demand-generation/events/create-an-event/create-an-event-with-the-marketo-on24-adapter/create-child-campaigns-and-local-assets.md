---
unique-page-id: 10096675
description: Erstellen von untergeordneten Kampagnen und lokalen Elementen - Marketing Docs - Produktdokumentation
title: Untergeordnete Kampagnen und lokale Assets erstellen
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '675'
ht-degree: 0%

---


# Untergeordnete Kampagnen und lokale Assets erstellen {#create-child-campaigns-and-local-assets}

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

## E-Mails und URL-Token {#emails-and-url-tokens}

Erstellen Sie die Einladung, Bestätigung, Follow-up und Dankeschön-E-Mails mit Marketo.

## Marketing-Bestätigungs-E-Mail- und URL-Token {#marketo-confirmation-email-and-url-token}

Verwenden Sie Marketo, um die Bestätigungs-E-Mail für Ihr Ereignis zu senden. Wenn sich eine Person registriert, erhält sie eine eindeutige URL, die für die Eingabe des Ereignisses verwendet werden kann.

>[!NOTE]
>
>**Erinnerung**
>
>Um Ihre Bestätigungs-E-Mail mit dieser eindeutigen URL zu füllen, verwenden Sie das folgende Token in Ihrer E-Mail: `{{member.webinar url}}`. Wenn Sie die Bestätigungs-URL senden, wird dieses Token automatisch zur eindeutigen Bestätigungs-URL der Person aufgelöst.
>
>Stellen Sie den Typ Ihrer Bestätigungs-E-Mail auf **Operational** ein, um sicherzustellen, dass Personen, die sich registrieren, ihre Bestätigungsinformationen erhalten, auch wenn sie sich nicht abonnieren.

>[!TIP]
>
>Sie können ON24 so konfigurieren, dass es Bestätigungs-, Erinnerungs- oder Follow-up-E-Mails sendet. Weitere Informationen finden Sie auf der [ON24-Hilfeseite](http://webcastelitehelp.on24.com) .

## Anforderungen an die Kinderregistrierung - Kampagne {#registration-child-campaign-requirements}

Ereignis enthalten eine oder mehrere untergeordnete Kampagnen, die alle zusammen arbeiten, um Menschen durch die Programm-Status zu bewegen und die Leistung Ihres Ereignisses zu verfolgen.

Beispiele für untergeordnete Kampagnen sind eine Einladungs-Kampagne, eine Registrierungs-Kampagne und Kampagnen zur Weiterverfolgung.

>[!CAUTION]
>
>Damit der Adapter seinen Auftrag ausführen kann, MÜSSEN Sie eine Registrierungs-Kampagne erstellen. Diese Kampagne muss von der Person ausgelöst werden, die ein Formular ausfüllt, und der erste Schritt muss den Status des Programms der Person in &quot; **Registriert**&quot;ändern. Die Kampagne sendet dann eine Bestätigungs-E-Mail. Weitere Informationen finden Sie in diesem Artikel.

**Registrierung/Bestätigung (Auslöser-Kampagne)**

* Intelligente Liste
* Auslöser basierend auf **Ausfüllformular**. Stellen Sie sicher, dass Sie die Landingpage, mit der das Formular ausgeführt wird, mit **Hinzufügen Einschränkung** einschließen, insbesondere wenn dasselbe Formular auf mehreren Landingpages verwendet wird.

>[!CAUTION]
>
>Sie müssen ein Marketo-Formular verwenden, um Ihre Personen für das Ereignis zu registrieren, oder ein Nicht-Marketo-Formular mit der richtigen API-Integration, um Registrierungsdaten an Marketo zu senden. Dies ist von entscheidender Bedeutung für den Erfolg Ihrer Ereignis-Partnerintegration.

>[!NOTE]
>
>Wenn Sie ein Marketo-Formular für eine Nicht-Marketo-Landingpage verwenden, wird als Auslöser das Formular **mit dem Formulardamen** ausgefüllt.

![](assets/image2015-12-22-15-3a20-3a51.png)

**Fluss**

* **Ändern Sie den Status** des Programms - Auf Webinar einstellen -> Registriert.

Dieser Flussschritt ist beim Einrichten der untergeordneten Kampagne als ERSTER FLOW-SCHRITT erforderlich. Wenn sich der Status des Programms einer Person in &quot;Registered&quot;ändert, setzt Marketo die Registrierungsinformationen auf ON24. Kein anderer Status wird die Person übertreiben.

* **E-Mail** senden - Bestätigungs-E-Mail. Stellen Sie diese E-Mail auf **Operational** ein, damit nicht abonnierte Personen, die sich registriert haben, sie weiterhin erhalten.

Der Schritt **E-Mail** senden MUSS der zweite Schritt sein. Die Bestätigungs-E-Mail enthält die `{{member.webinar url}}`, die mit Informationen gefüllt wird, die von ON24 an Marketo zurückgesendet werden.

![](assets/image2015-12-22-15-3a29-3a50.png)

>[!NOTE]
>
>Die Reihenfolge dieser Flussschritte ist wichtig, weil die Aktionen in Marketo ausgeführt werden. Der Schritt zum **Ändern des Status** des Programms sendet die Person zur Registrierung an ON24 und es wird eine eindeutige URL generiert. Danach können Sie die Bestätigungs-E-Mail mit dieser eindeutigen URL mit dem `{{member.webinar URL}}` Token senden.
>
>Wenn die Person mit einem Registrierungsfehler zurückgegeben wird, erhält sie keine E-Mail-Bestätigung.

Der nächste Schritt besteht darin, Ihre ON24-Ereignis-Integration zu [testen](test-your-on24-event-integration.md).

>[!NOTE]
>
>**Verwandte Artikel**
>
>* [Ereignisse des Marketo ON24-Adapters](understanding-marketo-on24-adapter-events.md)
>* [Beispiel für eine ON24-Ereignis-Integration](example-on24-event-integration.md)
>* [Erläuterungen zu Webinar-Programm-Status](understanding-webinar-program-statuses.md)
>* [On24-Ereignis-Integration testen](test-your-on24-event-integration.md)

>



