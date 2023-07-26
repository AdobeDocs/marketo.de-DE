---
description: Übersicht über das E-Mail-Tracking - Marketo-Dokumente - Produktdokumentation
title: Übersicht über das E-Mail-Tracking
exl-id: 89437d22-d739-45ea-8a2e-046a7de80379
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Übersicht über das E-Mail-Tracking {#email-tracking-overview}

## Funktionsweise der Antwortverfolgung {#how-reply-tracking-works}

Das Tracking der Antworten erfolgt durch Überprüfen einer Nachrichten-ID, die in jeder gesendeten E-Mail enthalten ist. Jede E-Mail enthält eine eindeutige Nachrichten-ID, mit der wir die beste Antwort-Tracking-Funktion nutzen können.

>[!PREREQUISITES]
>
>Verbindung mit E-Mail-Server: Sales Connect muss mit Ihrem Posteingang verbunden sein, damit wir wissen, wann eine neue Antwort eingetroffen ist. Sie müssen Ihr Sales Connect-Konto mit Gmail verbinden. Wenn Sie Outlook verwenden, müssen wir in Ihren Exchange-Server integrieren.

Wenn Sales Connect die Antwort Ihres potenziellen Kunden auf Ihre E-Mail nicht verfolgen kann, kann eine Kampagne nicht aufgrund der Antworterkennung angehalten oder die Antwort an Salesforce protokolliert werden. Was bedeutet, dass jede E-Mail-Adresse antworten kann?

Wenn Sie also flynn@flynnsarcade.com per E-Mail senden und er mit kevinf@flynnsarcade.com antwortet, können wir die Antwort verfolgen. Wenn Sie außerdem eine E-Mail an flynn@flynnsarcade.com und CC alan@encom.com senden und Alan Sie zurückschreibt, wird auch die Antwort erkannt und die Kampagne beendet.

## Verfolgen Ihrer E-Mail-Anhänge {#how-to-track-your-email-attachments}

Sales Connect bietet Tracking für Ihre Anhänge (.doc, .ppt, .pdf), sodass Sie sehen können, wann sie geöffnet/heruntergeladen wurden, und sehen, durch welche Seiten Ihr Empfänger sucht. Wir ermöglichen Ihnen die Verwendung unserer Funktion für nachverfolgte Anlagen aus beiden [Webanwendung](https://toutapp.com/login) und Gmail (oder Google Apps).

>[!NOTE]
>
>Die Anlagenverfolgung ist nur für unsere Teampläne verfügbar (beginnend mit unserem G3startup-Plan).

**Senden Ihrer ersten nachverfolgten Anlage**

1. Erstellen Sie eine E-Mail oder bearbeiten Sie eine Vorlage und klicken Sie auf die Schaltfläche **Inhalt** Schaltfläche.

1. Laden Sie den Anhang hoch und senden Sie ihn ab. Wir unterstützen PDF-, Word- und PowerPoint-Präsentationen.

1. Auswählen **Hinzufügen zu E-Mail**.

1. Klicks **Senden** und starten Sie Ihren Live-Feed. Ihre Empfänger werden angezeigt, wenn sie geöffnet und durch Ihre Anlagen navigiert werden.

>[!TIP]
>
>Wenn Sie eine Anlage nicht verfolgen möchten, klicken Sie einfach auf Dateien anhängen . Diese Anlage wird nicht verfolgt.

## Funktionsweise des Tracking-Anzeigentracks {#how-view-tracking-works}

Wir verfolgen E-Mail-Öffnungen, indem wir in den gesendeten E-Mails ein unsichtbares Bild einfügen.

Wenn jemand auf Ihre E-Mail antwortet, aber Sales Connect darauf hinweist, dass sie nicht angezeigt wurde, besteht die Gefahr, dass der Empfänger keine Bilder in seinem E-Mail-Client aktiviert hat (d. h., er klickt in der E-Mail auf die Nachricht &quot;Hier klicken, um Bilder herunterzuladen&quot;).

Einige Tipps für bessere Trackingstatistiken in E-Mails:

* Fügen Sie ein Bild (wie ein Logo) in Ihre E-Mails ein, damit der Empfänger die Bilder zum Anzeigen Ihrer Nachricht aktivieren kann.
* Fügen Sie einen Link als Aktionsaufruf in die E-Mail ein.

## Test-E-Mail nicht angezeigt als {#test-email-not-showed-as-viewed}

Selbst wenn Sie Ihre Nachricht an eine andere E-Mail-Adresse gesendet haben, werden wir Sie nicht beim Anzeigen von E-Mails, die Sie selbst im Live Feed gesendet haben, anmelden. Unser Tracking basiert auf Geräten. Solange Sie einen Computer verwenden, mit dem Sie sich bei Sales Connect angemeldet haben, filtern wir diese Aktivität heraus.

Der Grund? Sales Connect ist intelligent, und unsere aktiven Benutzer würden uns nie verzeihen, wenn ihre eigenen Informationen jedes Mal, wenn sie eine von ihnen gesendete E-Mail ansehen, in der Live-Feed-Aktivität angezeigt würden.
