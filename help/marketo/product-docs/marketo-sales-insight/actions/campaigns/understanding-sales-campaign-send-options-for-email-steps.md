---
description: Verstehen der Versandoptionen von Verkaufskampagnen für E-Mail-Schritte - Marketo-Dokumente - Produktdokumentation
title: Grundlagen zu den Versandoptionen von Vertriebskampagnen für E-Mail-Schritte
exl-id: 775c6401-efb2-4940-a81c-be5d2759c7bd
source-git-commit: a0a2c93b89738c048f7aac658be9fa95b5e87f89
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 3%

---

# Grundlagen zu den Versandoptionen von Vertriebskampagnen für E-Mail-Schritte {#understanding-sales-campaign-send-options-for-email-steps}

Beim Erstellen einer Vertriebskampagne haben Sie mehrere Optionen, wie Ihre E-Mail-Schritte in Sales Insight-Aktionen erstellt werden. Und je nachdem, wo Ihre E-Mail in Ihre Vertriebskampagne fällt, unterscheiden sich auch Ihre Optionen.

## Optionen zum Senden eines ersten Schritts {#first-step-send-options}

Wenn es Ihr erster Schritt und der erste Tag in Ihrer Vertriebskampagne ist, haben Sie die folgenden Optionen:

![](assets/understanding-sales-campaign-send-options-for-email-steps-1.png)

Ich werde entscheiden, wann diese E-Mail gesendet werden soll

* Mit dieser Option können Sie die &quot;Versandzeit&quot;für die erste E-Mail in Ihrer Vertriebskampagne auswählen, wenn Sie die Verkaufskampagne starten, indem Sie Personen hinzufügen.

Diese E-Mail zum folgenden Zeitpunkt senden

* Wenn Sie Ihre Vertriebskampagne durch Hinzufügen von Personen starten, planen wir die E-Mail für diese Zeit.
* Sie haben immer die Möglichkeit, einen neuen &quot;Versand am&quot;-Zeitpunkt zu wählen, wenn Sie Ihre Vertriebskampagne starten.

Eine Aufgabe erstellen: Ich werde diese E-Mail selbst senden

* Mit dieser Option wird eine E-Mail-Aufgabe (und eine Synchronisation mit Salesforce) erstellt, die Sie nach Belieben versenden können.
* Wenn Sie diese Auswahl getroffen haben und Ihre Vertriebskampagne starten, werden wir diese Aufgaben im Command Center und im Live Feed für Sie in die Warteschlange stellen. Sie können dann jede E-Mail personalisieren und senden (oder planen), bevor sie abläuft.

   * Wenn Sie diese Aufgabe in unserer Webanwendung öffnen, wird ein Komprimierungsfenster mit der E-Mail-Adresse Ihres Kontakts, der Betreffzeile Ihrer E-Mail und der von Ihnen ausgewählten Vorlage geöffnet.
   * Wenn Sie diese Aufgabe in Gmail oder Outlook öffnen, wird ein natives Komprimierungsfenster geöffnet, in dem Sie die E-Mail-Adresse Ihres Kontakts, die Betreffzeile Ihrer E-Mail und die von Ihnen ausgewählte Vorlage dynamisch ausfüllen.

## Optionen für nachfolgenden Schritt-Versand {#subsequent-step-send-options}

Für alle nachfolgenden Tage/Schritte in Ihrer Verkaufskampagne stehen folgende Optionen zur Verfügung:

Senden Sie diese E-Mail gleichzeitig mit der vorherigen E-Mail in dieser Verkaufskampagne

* Diese Option sendet die E-Mail gleichzeitig mit der E-Mail direkt vor der E-Mail.
* Er wird weiterhin an dem Tag gesendet, an dem er verknüpft ist.

Diese E-Mail zum folgenden Zeitpunkt senden

* Wenn Sie Ihre Vertriebskampagne durch Hinzufügen von Personen starten, planen wir die E-Mail für diese Zeit.
* Sie haben immer die Möglichkeit, einen neuen &quot;Versand am&quot;-Zeitpunkt zu wählen, wenn Sie Ihre Vertriebskampagne starten.

Eine Aufgabe erstellen: Ich werde diese E-Mail selbst senden

* Mit dieser Option wird eine E-Mail-Aufgabe (und eine Synchronisation mit Salesforce) erstellt, die Sie nach Belieben versenden können.
* Sobald Sie diese Auswahl getroffen haben, werden diese Aufgaben beim Start Ihrer Sales Campaign mit Sales Insight Actions im Command Center und im Live Feed in die Warteschlange gestellt. Sie können dann jede E-Mail personalisieren und senden (oder planen), bevor sie abläuft.

   * Wenn Sie diese Aufgabe in unserer Webanwendung öffnen, wird ein Komprimierungsfenster mit der E-Mail-Adresse Ihres Kontakts, der Betreffzeile Ihrer E-Mail und der von Ihnen ausgewählten Vorlage geöffnet.
   * Wenn Sie diese Aufgabe in Gmail oder Outlook öffnen, wird ein natives Komprimierungsfenster geöffnet, in dem Sie die E-Mail-Adresse Ihres Kontakts, die Betreffzeile Ihrer E-Mail und die von Ihnen ausgewählte Vorlage dynamisch ausfüllen.

Diese E-Mail an die vorherige E-Mail senden

* Diese Versandoption ist eine &#39;Follow-up&#39;-Aktion zu Ihrer vorherigen E-Mail und hängt den vorherigen E-Mail-Textkörper an den Ende dieser E-Mail an.

>[!MORELIKETHIS]
>
>[Erstellen einer Verkaufskampagne](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/create-a-sales-campaign.md){target=&quot;_blank&quot;}
>[Schritttypen und Erinnerungsaufgaben für Vertriebskampagnen](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/sales-campaign-step-types-and-reminder-tasks.md){target=&quot;_blank&quot;}
>[Einstellungen für Vertriebskampagnen](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/sales-campaign-settings.md){target=&quot;_blank&quot;}