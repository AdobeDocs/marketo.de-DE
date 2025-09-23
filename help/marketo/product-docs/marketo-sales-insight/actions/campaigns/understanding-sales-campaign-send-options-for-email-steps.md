---
description: Grundlegendes zu Versandoptionen für Vertriebskampagnen bei E-Mail-Schritten - Marketo-Dokumente - Produktdokumentation
title: Grundlegendes zu den Versandoptionen für E-Mail-Schritte in Verkaufskampagnen
feature: Sales Insight Actions
exl-id: 775c6401-efb2-4940-a81c-be5d2759c7bd
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '740'
ht-degree: 4%

---

# Grundlegendes zu den Versandoptionen für E-Mail-Schritte in Verkaufskampagnen {#understanding-sales-campaign-send-options-for-email-steps}

Wenn Sie eine Verkaufskampagne erstellen, haben Sie mehrere Möglichkeiten, wie Ihre E-Mail-Schritte in [!DNL Sales Insight Actions] erstellt werden. Und je nachdem, wo Ihre E-Mail in Ihre Verkaufskampagne fällt, unterscheiden sich auch Ihre Optionen.

## Versandoptionen für den ersten Schritt {#first-step-send-options}

Wenn es Ihr erster Schritt und der erste Tag in Ihrer Verkaufskampagne ist, haben Sie die folgenden Optionen:

![](assets/understanding-sales-campaign-send-options-for-email-steps-1.png)

### Ich werde auswählen, wann diese E-Mail gesendet werden soll {#first-step-i-will-choose}

* Mit dieser Option können Sie den Sendezeitpunkt für die erste E-Mail in Ihrer Vertriebskampagne auswählen, wenn Sie die Verkaufskampagne starten, indem Sie Personen hinzufügen.

### Diese E-Mail zum folgenden Zeitpunkt senden {#first-step-following-time}

* Wenn Sie Ihre Verkaufskampagne starten, indem Sie Personen zu ihr hinzufügen, planen wir die E-Mail für diesen Zeitpunkt.
* Sie haben immer die Möglichkeit, beim Start Ihrer Verkaufskampagne einen neuen „Versand“ zu wählen.

### Eine Aufgabe erstellen: Ich werde diese E-Mail selbst senden {#first-step-create-a-task}

* Mit dieser Option wird eine E-Mail-Aufgabe erstellt (und mit [!DNL Salesforce] synchronisiert), die Sie nach Bedarf senden können.
* Sobald Sie diese Auswahl getroffen haben, werden wir diese Aufgaben beim Start Ihrer Vertriebskampagne in der Befehlszentrale und im Live-Feed für Sie in die Warteschlange stellen. Sie können dann jede E-Mail personalisieren und senden (oder planen), bevor sie gesendet wird.

   * Wenn Sie diese Aufgabe in unserer Web-Anwendung öffnen, wird ein Fenster zum Erstellen mit der E-Mail-Adresse Ihres Kontakts, der Betreffzeile Ihrer E-Mail und der von Ihnen ausgewählten Vorlage geöffnet.
   * Wenn Sie diese Aufgabe in Gmail oder [!DNL Outlook] öffnen, wird ein natives Fenster zum Erstellen geöffnet und die E-Mail-Adresse Ihres Kontakts, die Betreffzeile Ihrer E-Mail und die von Ihnen ausgewählte Vorlage werden dynamisch ausgefüllt.

## Optionen für den nachfolgenden Schritt „Senden“ {#subsequent-step-send-options}

Für alle nachfolgenden Tage/Schritte in Ihrer Verkaufskampagne haben Sie die folgenden Optionen:

### Diese E-Mail gleichzeitig mit der vorherigen E-Mail in dieser Verkaufskampagne senden {#subsequent-send-at-same-time}

* Mit dieser Option wird die E-Mail gleichzeitig mit der E-Mail direkt davor gesendet.
* Er sendet weiterhin an dem Tag, an dem er verknüpft ist.

>[!IMPORTANT]
>
>Das gleichzeitige Senden einer E-Mail und der vorherigen E-Mail wird nicht für E-Mails unterstützt, die am selben Tag gesendet werden. Stattdessen wird die E-Mail zum Zeitpunkt der E-Mail gesendet, die am Vortag gesendet wurde. Wenn diese Option am ersten Tag der Kampagne für eine E-Mail ausgewählt ist (nicht empfohlen), wird diese E-Mail sofort zu Beginn der Kampagne versendet.

### Diese E-Mail zum folgenden Zeitpunkt senden {#subsequent-send-at-following-time}

* Wenn Sie Ihre Verkaufskampagne starten, indem Sie Personen zu ihr hinzufügen, planen wir die E-Mail für diesen Zeitpunkt.
* Sie haben immer die Möglichkeit, beim Start Ihrer Verkaufskampagne einen neuen „Versand“ zu wählen.

### Eine Aufgabe erstellen: Ich werde diese E-Mail selbst senden {#subsequent-create-a-task}

* Mit dieser Option wird eine E-Mail-Aufgabe erstellt (und mit [!DNL Salesforce] synchronisiert), die Sie nach Bedarf senden können.
* Sobald Sie diese Auswahl getroffen haben, werden [!DNL Sales Insight Actions] diese Aufgaben beim Start Ihrer Vertriebskampagne in der Befehlszentrale und im Live-Feed für Sie in die Warteschlange stellen. Sie können dann jede E-Mail personalisieren und senden (oder planen), bevor sie gesendet wird.

   * Wenn Sie diese Aufgabe in unserer Web-Anwendung öffnen, wird ein Fenster zum Erstellen mit der E-Mail-Adresse Ihres Kontakts, der Betreffzeile Ihrer E-Mail und der von Ihnen ausgewählten Vorlage geöffnet.
   * Wenn Sie diese Aufgabe in Gmail oder [!DNL Outlook] öffnen, wird ein natives Fenster zum Erstellen geöffnet und die E-Mail-Adresse Ihres Kontakts, die Betreffzeile Ihrer E-Mail und die von Ihnen ausgewählte Vorlage werden dynamisch ausgefüllt.

### Erstellen Sie diese E-Mail als Folgemaßnahme zur vorherigen E-Mail in dieser Kampagne {#subsequent-create-this-email}

* Aktivieren Sie dieses Kontrollkästchen, wenn die vorherige E-Mail in Ihrer Verkaufskampagne an die nächste E-Mail angehängt werden soll, die Ihre Verkaufskampagne versendet.
* Für die angehängte Kopie der E-Mail wird die E-Mail-Vorlage in Ihrer Verkaufskampagne immer gesendet. Eventuelle Änderungen, die der Benutzer vor dem Versand vorgenommen hat, werden nicht in den Versand einbezogen.

>[!NOTE]
>
>Diese Option zum Erstellen einer E-Mail als Folgenachricht ist nur für einen E-Mail-Schritt verfügbar, wenn der vorherige Schritt auch eine E-Mail ist. Wenn der vorherige Schritt Call, InMail oder Custom ist, wird die Option zum Erstellen eines Follow-ups nicht angezeigt.

>[!MORELIKETHIS]
>
>[Erstellen einer Verkaufskampagne](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/create-a-sales-campaign.md){target="_blank"}
>>[Vertriebskampagne - Schritttypen und Erinnerungsaufgaben](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/sales-campaign-step-types-and-reminder-tasks.md){target="_blank"}
>>[Einstellungen für Verkaufskampagnen](/help/marketo/product-docs/marketo-sales-insight/actions/campaigns/sales-campaign-settings.md){target="_blank"}
