---
unique-page-id: 2949158
description: Integrieren von RTP mit Google Analytics - Marketo Docs - Produktdokumentation
title: RTP in Google Analytics integrieren
exl-id: a2bc0c17-dc23-435e-9480-857e97e6fd50
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 0%

---

# RTP in Google Analytics integrieren {#integrate-rtp-with-google-analytics}

>[!NOTE]
>
>Universal Analytics ist jetzt der Betriebsstandard und alle Eigenschaften in Google wurden auf Universal Analytics aktualisiert.
>
>Dieser Artikel zeigt, wie Sie die alte Google Standard Analytics verwenden. Es wird jedoch empfohlen, zu Universal Analytics zu wechseln.
>
>Wenn Sie den Trackingcode [analytics.js](https://developers.google.com/analytics/devguides/collection/analyticsjs/) noch nicht verwenden, empfiehlt Google dringend, Ihre Site erneut mit Tags zu versehen, um ihn zu verwenden. Google stellt Folgendes ein:
>
>* ga.js
>* urchin.js
>* WAP-/Server-seitige Snippets
>* YT/MO
>* Benutzerdefinierte Variablen
>* Benutzerdefinierte Variablen
>
>Erfahren Sie, wie Sie [Web Personalization mit Universal Analytics integrieren](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

## Einführung {#introduction}

Analysieren Sie Ihre Webanalysen unter Verwendung des direkten Datenflusses von Marketo Real-Time Personalization (RTP) zu Ihrem Google Analytics-Konto (GA). Messen Sie Ihre Webbesuche in GA nach Organisationen, Branchen und RTP-Kampagnen. Zeigen Sie Metriken wie Branchen- oder RTP-Segmente in der allgemeinen Verfügbarkeit an und zeigen Sie anhand verschiedener Traffic-Quellen (Social, Paid, Organic), analysieren Sie Klickraten für Kampagnen und messen Sie die Wirkung von Personalisierungskampagnen auf Ihrer Website. Nutzen Sie diese Möglichkeit, um den größtmöglichen Nutzen aus Ihrem RTP-Konto zu ziehen.

**RTP-Audience Analytics**

Mit der Integration haben Sie eine neue Dimension in Ihrem GA-Konto. RTP verbessert Ihre Dashboards automatisch mit:

1. Organisationen und Industrie
1. Benutzerdefinierte Segmente in RTP
1. Account-Based Marketing-Listen

Konzentrieren Sie sich auf Ihre wichtigsten B2B-Perspektiven. Analysieren Sie Kanäle nach Branchen und Segmenten mit Zielgruppen.

## Kanalbericht {#channel-report}

![](assets/image2014-11-28-16-3a39-3a28.png)

Das RTP B2B Dashboard hilft Ihnen, die Aufschlüsselung Ihrer Besucher nach Vertikalen und RTP-Segmentierung zu verstehen. Sie können die Leistung Ihrer Besucher entsprechend der Finanzbranche und den verschiedenen Marketing-Kampagnen (gebührenpflichtig, organisch, sozial) anzeigen. Das Dashboard bietet außerdem einen allgemeinen Überblick über die Leistung Ihrer RTP-Segmente und zeigt die wichtigsten Organisationen, die Ihre Site besuchen, anhand von Drilldown an.

## Verhaltensfluss {#behavioral-flow}

![](assets/image2014-11-28-16-3a40-3a43.png)

Der Bericht &quot;Verhaltensfluss&quot;(siehe Bild) visualisiert den Pfad, den Besucher von einer Seite oder einem Ereignis zur nächsten navigieren. Das Bildbeispiel zeigt den Pfad aller Besucher aus dem Finanzsektor. Dieser Bericht kann Ihnen dabei helfen festzustellen, durch welche Inhalte Besucher mit Ihrer Site interagieren.

## RTP-Leistung {#rtp-performance}

Messen Sie Ihre RTP-Kampagnen und ordnen Sie sie Ihrem gesamten Site-Durchschnitt zu. Erfahren Sie, wie sich diese Kampagnen auf Ihre Website-Metriken auswirken, und nutzen Sie diese Daten, um Ihre Personalisierungsbemühungen auf die richtigen Ziele zu konzentrieren. Erstellen Sie benutzerspezifische Berichte, um die Leistung Ihrer Personalisierungskampagnen besser zu verstehen.

![](assets/image2014-11-28-16-3a47-3a0.png)

## Einrichten von RTP mit Google Analytics {#setting-up-rtp-with-google-analytics}

1. Fügen Sie die E-Mail rtp.ga2@gmail.com als Benutzer Lesen und Analysieren zu Ihrem GA-Konto hinzu. Weitere Informationen finden Sie unter [hier](https://support.google.com/analytics/answer/2884495?hl=en).

1. In Ihrem RTP-Konto. Wechseln Sie zu **Kontoeinstellungen**.

   ![](assets/image2014-11-28-16-3a54-3a40.png)

1. Unter &quot;**Kontoeinstellungen**&quot;, &quot;**Domäne**&quot;und &quot;**Analytics**&quot;.

1. Klicken Sie auf **Google Analytics**.

1. Aktivieren Sie die relevanten **benutzerdefinierten Variablen** und **Ereignisse**, um diese Daten von RTP an Google Analytics anzuhängen.

1. Geben Sie die Nummer **Steckplatz** ein, um benutzerdefinierte Variablendaten zu senden (standardmäßig 1,2).

![](assets/image2014-11-28-17-3a0-3a17.png)

1. Klicken Sie auf **Speichern**.

>[!NOTE]
>
>Um Segmentdaten an GA zu senden, aktivieren Sie auf der Seite [Segment bearbeiten](/help/marketo/product-docs/web-personalization/using-web-segments/create-a-basic-web-segment.md) der RTP-Plattform das Kontrollkästchen **Ereignis bei Segmentübereinstimmung an Google Analytics senden**.

## Einrichten von Google Analytics-Berichten mit RTP-Daten {#setting-up-google-analytics-reports-with-rtp-data}

In Google Analytics können Sie Dashboards, GA-Segmentierung und Berichte verwenden, um Ihre RTP-Daten anzuzeigen:

* [Dashboards](https://support.google.com/analytics/answer/1068216?hl=en) bieten einen Überblick über die Leistung der Website.
* Ein GA-Segment dient dazu, Besucher in der GA-Oberfläche zu filtern und den Traffic pro Segment anzuzeigen. Erfahren Sie, wie Sie [hier](https://support.google.com/analytics/answer/3124493?hl=en) ein Segment erstellen.
* Erstellen von [benutzerdefinierten Berichten](https://support.google.com/analytics/answer/1033013?hl=en) zum Anzeigen und/oder Einrichten geplanter E-Mails. Siehe unter Anpassung > Neuer benutzerdefinierter Bericht.
