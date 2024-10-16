---
unique-page-id: 14352621
description: Verstehen der Sendeoptionen - Marketo-Dokumente - Produktdokumentation
title: Grundlagen zu Sendeoptionen
exl-id: acdee691-478e-4ffe-90e2-54cf559fa38d
feature: Marketo Sales Connect
source-git-commit: 832635c9e029754ce094e4137724bcc956dbcd35
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 0%

---

# Grundlagen zu Sendeoptionen {#understanding-send-options}

Beim Erstellen einer Kampagne haben Sie mehrere Optionen, wie Ihre E-Mail-Schritte in Sales Connect erstellt werden. Je nachdem, wo Ihre E-Mail in Ihre Kampagne fällt, unterscheiden sich auch Ihre Optionen.

Wenn es Ihr erster Schritt und der erste Tag in Ihrer Kampagne ist, haben Sie die folgenden Optionen:

![](assets/image2019-10-25-10-43-19.png)

**Ich werde wählen, wann diese E-Mail gesendet werden soll**

* Mit dieser Option können Sie beim Start der Kampagne den Zeitpunkt für den Versand der ersten E-Mail in Ihrer Kampagne festlegen, indem Sie Personen hinzufügen.

**Diese E-Mail zur folgenden Zeit senden**

* Wenn Sie Ihre Kampagne durch Hinzufügen von Personen starten, planen wir die E-Mail für diesen Zeitpunkt.
* Sie haben immer die Möglichkeit, einen neuen &quot;Versand am&quot;-Zeitpunkt zu wählen, wenn Sie Ihre Kampagne starten.

**Erstellen einer Aufgabe; ich werde diese E-Mail selbst senden**

* Mit dieser Option wird eine E-Mail-Aufgabe erstellt (und mit Salesforce synchronisiert), die Sie nach Belieben senden können.
* Nachdem Sie diese Auswahl getroffen haben, stellen wir diese Aufgaben beim Start Ihrer Kampagne im Command Center und im Live Feed für Sie in die Warteschlange. Sie können dann jede E-Mail personalisieren und senden (oder planen), bevor sie abläuft.

   * Wenn Sie diese Aufgabe in unserer Webanwendung öffnen, wird ein Komprimierungsfenster mit der E-Mail-Adresse Ihres Kontakts, der Betreffzeile Ihrer E-Mail und der von Ihnen ausgewählten Vorlage geöffnet.
   * Wenn Sie diese Aufgabe in Gmail oder Outlook öffnen, wird ein natives Komprimierungsfenster geöffnet, in dem Sie die E-Mail-Adresse Ihres Kontakts, die Betreffzeile Ihrer E-Mail und die von Ihnen ausgewählte Vorlage dynamisch ausfüllen.

Für alle nachfolgenden Tage/Schritte in Ihrer Kampagne haben Sie die folgenden Optionen:

**Diese E-Mail gleichzeitig mit der vorherigen E-Mail in dieser Kampagne senden**

* Diese Option sendet die E-Mail gleichzeitig mit der E-Mail direkt vor der E-Mail.
* Er wird weiterhin an dem Tag gesendet, an dem er verknüpft ist.

>[!IMPORTANT]
>
>Das Senden einer E-Mail zur selben Zeit wie die vorherige E-Mail wird für E-Mails, die am selben Tag gesendet werden, nicht unterstützt. Stattdessen wird die E-Mail zum Zeitpunkt des E-Mail-Versands vom Vortag gesendet. Wenn diese Option am ersten Tag der Kampagne für eine E-Mail ausgewählt wird (nicht empfohlen), wird diese E-Mail sofort zu Beginn der Kampagne gesendet.

**Diese E-Mail zur folgenden Zeit senden**

* Wenn Sie Ihre Kampagne durch Hinzufügen von Personen starten, planen wir die E-Mail für diesen Zeitpunkt.
* Sie haben immer die Möglichkeit, einen neuen &quot;Versand am&quot;-Zeitpunkt zu wählen, wenn Sie Ihre Kampagne starten.

**Erstellen einer Aufgabe; ich werde diese E-Mail selbst senden**

* Mit dieser Option wird eine E-Mail-Aufgabe erstellt (und mit Salesforce synchronisiert), die Sie nach Belieben senden können.
* Nachdem Sie diese Auswahl getroffen haben, stellt Tout diese Aufgaben beim Start Ihrer Kampagne in die Warteschlange und stellt sie im Command Center und im Live Feed für Sie bereit. Sie können dann jede E-Mail personalisieren und senden (oder planen), bevor sie abläuft.

   * Wenn Sie diese Aufgabe in unserer Webanwendung öffnen, wird ein Komprimierungsfenster mit der E-Mail-Adresse Ihres Kontakts, der Betreffzeile Ihrer E-Mail und der von Ihnen ausgewählten Vorlage geöffnet.
   * Wenn Sie diese Aufgabe in Gmail oder Outlook öffnen, wird ein natives Komprimierungsfenster geöffnet, in dem Sie die E-Mail-Adresse Ihres Kontakts, die Betreffzeile Ihrer E-Mail und die von Ihnen ausgewählte Vorlage dynamisch ausfüllen.

**Diese E-Mail an die vorherige E-Mail verschicken**

* Diese Versandoption ist eine &#39;Follow-up&#39;-Aktion zu Ihrer vorherigen E-Mail und hängt den vorherigen E-Mail-Textkörper an den Ende dieser E-Mail an.

