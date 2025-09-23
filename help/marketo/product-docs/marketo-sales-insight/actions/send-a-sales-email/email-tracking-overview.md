---
description: Übersicht über das E-Mail-Tracking - Marketo-Dokumente - Produktdokumentation
title: E-Mail-Tracking – Überblick
exl-id: 89437d22-d739-45ea-8a2e-046a7de80379
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 5%

---

# E-Mail-Tracking – Überblick {#email-tracking-overview}

## Funktionsweise der Antwortverfolgung {#how-reply-tracking-works}

Das Antwort-Tracking erfolgt anhand einer Nachrichten-ID in jeder gesendeten E-Mail. Jede E-Mail enthält eine eindeutige Nachrichten-ID, mit der wir einige der besten Antworten verfolgen können.

>[!PREREQUISITES]
>
>Verbindung mit E-Mail-Server: [!DNL Sales Connect] muss mit Ihrem Posteingang verbunden sein, damit wir wissen, wann eine neue Antwort eingetroffen ist. Ihr [!DNL Sales Connect]-Konto muss mit Gmail verbunden sein. Wenn Sie Outlook verwenden, müssen wir eine Integration mit Ihrem Exchange-Server vornehmen.

Wenn [!DNL Sales Connect] die Antwort Ihres Interessenten auf Ihre E-Mail nicht verfolgen können, kann er eine Kampagne nicht auf der Grundlage der Antworterkennung stoppen oder diese Antwort in Salesforce protokollieren. Was meinen wir damit, dass jede E-Mail-Adresse antworten kann?

Wenn Sie also eine E-Mail an <flynn@flynnsarcade.com> senden und er mit <kevinf@flynnsarcade.com> antwortet, können wir die Antwort verfolgen. Wenn Sie <flynn@flynnsarcade.com> und CC <alan@encom.com> per E-Mail senden und Alan Sie zurückschreibt, wird die Antwort ebenfalls erkannt und die Kampagne wird beendet.

## Verfolgen von E-Mail-Anhängen {#how-to-track-your-email-attachments}

[!DNL Sales Connect] bietet Tracking für Ihre Anlagen (.doc, .ppt, .pdf), damit Sie sehen können, wann diese geöffnet/heruntergeladen wurden, und sehen können, welche Seiten Ihre Empfängerin bzw. Ihr Empfänger durchsucht. Wir ermöglichen Ihnen die Verwendung unserer Funktion zum Tracking von Anhängen sowohl aus der [Web-Anwendung](https://toutapp.com/login) als auch aus Gmail (oder Google Apps).

>[!NOTE]
>
>Das Tracking von Anhängen ist nur für unsere Teampläne verfügbar (beginnend mit unserem g3startup-Plan).

**So senden Sie Ihren ersten verfolgbaren Anhang**

1. Erstellen Sie eine E-Mail oder bearbeiten Sie eine Vorlage und klicken Sie dann auf die Schaltfläche **[!UICONTROL Inhalt]**.

1. Laden Sie Ihren Anhang hoch und senden Sie ihn ab. Wir unterstützen PDFs, [!DNL Word] Dokumente und [!DNL Powerpoint].

1. Wählen Sie **[!UICONTROL Zu E-Mail hinzufügen]** aus.

1. Klicken Sie **[!UICONTROL Senden]** und starten Sie Ihren Live-Feed. Ihre Empfänger werden beim Öffnen angezeigt und durch Ihre Anhänge navigiert.

>[!TIP]
>
>Wenn Sie eine Anlage nicht verfolgen möchten, klicken Sie einfach auf Dateien anhängen und diese Anlage wird nicht verfolgt.

## Verfolgen von Ansichten {#how-view-tracking-works}

Wir verfolgen das Öffnen von E-Mails, indem wir ein unsichtbares Bild in die gesendeten E-Mails einfügen.

Wenn jemand auf Ihre E-Mail antwortet, aber [!DNL Sales Connect] sagt, dass sie nicht angezeigt wurde, besteht die Wahrscheinlichkeit, dass der Empfänger Bilder in seinem E-Mail-Client nicht aktiviert hat (d. h. in der E-Mail auf die Nachricht „Hier klicken, um Bilder herunterzuladen“ klicken).

Tipps für bessere Tracking-Statistiken in E-Mails:

* Fügen Sie Ihren E-Mails ein Bild hinzu (z. B. ein Logo), damit der Empfänger Bilder aktivieren kann, um Ihre Nachricht zu sehen.
* Fügen Sie einen Link als call to action in die E-Mail ein.

## Test-E-Mail wird nicht als gelesen angezeigt {#test-email-not-showed-as-viewed}

Selbst wenn Sie Ihre Nachricht an eine andere E-Mail-Adresse gesendet haben, werden wir Sie nicht beim Anzeigen von E-Mails protokollieren, die Sie sich selbst im Live-Feed gesendet haben. Unser Tracking ist gerätebasiert. Solange Sie einen Computer verwenden, mit dem Sie sich [!DNL Sales Connect] angemeldet haben, filtern wir diese Aktivität aus.

Der Grund? [!DNL Sales Connect] ist intelligent. Unsere aktiven Benutzer würden es uns nie verzeihen, wenn ihre eigenen Informationen in der Live-Feed-Aktivität jedes Mal angezeigt würden, wenn sie eine von ihnen gesendete E-Mail ansähen.
