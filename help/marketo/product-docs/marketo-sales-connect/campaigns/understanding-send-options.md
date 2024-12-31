---
unique-page-id: 14352621
description: Grundlegendes zu Sendeoptionen - Marketo-Dokumente - Produktdokumentation
title: Verstehen der Sendeoptionen
exl-id: acdee691-478e-4ffe-90e2-54cf559fa38d
feature: Marketo Sales Connect
source-git-commit: 832635c9e029754ce094e4137724bcc956dbcd35
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 0%

---

# Verstehen der Sendeoptionen {#understanding-send-options}

Wenn Sie eine Kampagne erstellen, haben Sie mehrere Möglichkeiten, wie Ihre E-Mail-Schritte in Sales Connect erstellt werden. Und je nachdem, wo Ihre E-Mail in Ihre Campaign-Kampagne fällt, unterscheiden sich auch Ihre Optionen.

Wenn es Ihr erster Schritt und der erste Tag in Ihrer Kampagne ist, haben Sie die folgenden Optionen:

![](assets/image2019-10-25-10-43-19.png)

**Ich werde den Zeitpunkt für den Versand dieser E-Mail wählen**

* Mit dieser Option können Sie den Sendezeitpunkt für die erste E-Mail in Ihrer Kampagne auswählen, wenn Sie die Kampagne starten, indem Sie Personen hinzufügen.

**Senden Sie diese E-Mail zum folgenden Zeitpunkt**

* Wenn Sie Ihre Kampagne starten, indem Sie Personen zu ihr hinzufügen, planen wir die E-Mail für diesen Zeitpunkt.
* Sie haben immer die Möglichkeit, beim Start Ihrer Kampagne einen neuen Versandzeitpunkt auszuwählen.

**Aufgabe erstellen; ich sende diese E-Mail selbst**

* Mit dieser Option wird eine E-Mail-Aufgabe erstellt (und mit Salesforce synchronisiert), die Sie nach Bedarf senden können.
* Sobald Sie diese Auswahl getroffen haben, werden wir diese Aufgaben beim Start Ihrer Kampagne in der Befehlszentrale und im Live-Feed für Sie in eine Warteschlange stellen. Sie können dann jede E-Mail personalisieren und senden (oder planen), bevor sie gesendet wird.

   * Wenn Sie diese Aufgabe in unserer Web-Anwendung öffnen, wird ein Fenster zum Erstellen mit der E-Mail-Adresse Ihres Kontakts, der Betreffzeile Ihrer E-Mail und der von Ihnen ausgewählten Vorlage geöffnet.
   * Wenn Sie diese Aufgabe in Gmail oder Outlook öffnen, wird ein natives Fenster zum Erstellen geöffnet und die E-Mail-Adresse Ihres Kontakts, die Betreffzeile Ihrer E-Mail und die ausgewählte Vorlage werden dynamisch ausgefüllt.

Für alle nachfolgenden Tage/Schritte in Ihrer Kampagne haben Sie die folgenden Optionen:

**Senden Sie diese E-Mail gleichzeitig mit der vorherigen E-Mail in dieser Kampagne**

* Mit dieser Option wird die E-Mail gleichzeitig mit der E-Mail direkt davor gesendet.
* Er sendet weiterhin an dem Tag, an dem er verknüpft ist.

>[!IMPORTANT]
>
>Das gleichzeitige Senden einer E-Mail und der vorherigen E-Mail wird nicht für E-Mails unterstützt, die am selben Tag gesendet werden. Stattdessen wird die E-Mail zum Zeitpunkt der E-Mail gesendet, die am Vortag gesendet wurde. Wenn diese Option am ersten Tag der Kampagne für eine E-Mail ausgewählt ist (nicht empfohlen), wird diese E-Mail sofort zu Beginn der Kampagne versendet.

**Senden Sie diese E-Mail zum folgenden Zeitpunkt**

* Wenn Sie Ihre Kampagne starten, indem Sie Personen zu ihr hinzufügen, planen wir die E-Mail für diesen Zeitpunkt.
* Sie haben immer die Möglichkeit, beim Start Ihrer Kampagne einen neuen Versandzeitpunkt auszuwählen.

**Aufgabe erstellen; ich sende diese E-Mail selbst**

* Mit dieser Option wird eine E-Mail-Aufgabe erstellt (und mit Salesforce synchronisiert), die Sie nach Bedarf senden können.
* Wenn Sie diese Auswahl getroffen haben, stellt Tout diese Aufgaben beim Start Ihrer Kampagne in der Kommandozentrale und im Live-Feed in eine Warteschlange. Sie können dann jede E-Mail personalisieren und senden (oder planen), bevor sie gesendet wird.

   * Wenn Sie diese Aufgabe in unserer Web-Anwendung öffnen, wird ein Fenster zum Erstellen mit der E-Mail-Adresse Ihres Kontakts, der Betreffzeile Ihrer E-Mail und der von Ihnen ausgewählten Vorlage geöffnet.
   * Wenn Sie diese Aufgabe in Gmail oder Outlook öffnen, wird ein natives Fenster zum Erstellen geöffnet und die E-Mail-Adresse Ihres Kontakts, die Betreffzeile Ihrer E-Mail und die ausgewählte Vorlage werden dynamisch ausgefüllt.

**Diese E-Mail in die vorherige E-Mail einfädeln**

* Diese Versandoption ist eine „Folgeoption“ zu Ihrer vorherigen E-Mail und hängt den vorherigen E-Mail-Textkörper an das Ende dieser E-Mail an.

