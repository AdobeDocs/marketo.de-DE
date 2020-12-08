---
unique-page-id: 2949160
description: Integration mit Adobe Analytics - Marketing Docs - Produktdokumentation
title: Integration mit Adobe Analytics
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '1130'
ht-degree: 0%

---


# Integration mit Adobe Analytics {#integrate-with-adobe-analytics}

## Intro {#intro}

Analysieren Sie Ihre Webanalyse aus der Perspektive von B2B, indem Sie die Daten zur Kampagne von Unternehmen, Branche und Marketing-to-Real-Time Personalization (RTP) in Ihrem Adobe Analytics-Konto anzeigen.

Dieses Dokument ermöglicht die Integration von Marketo Real-Time Personalization (RTP) und Adobe Adobe Analytics. Mit Daten von RTP können Sie Trends in allen Branchensegmenten und Organisationen, die Ihre Site besuchen, erkennen und analysieren und die Effektivität Ihrer RTP-Kampagnen messen. So erhalten Sie Einblicke und Analyse, um optimale Ergebnisse zu erzielen.

Sie können dies erreichen, indem Sie Metriken wie die Anzahl der neuen oder wiederkehrenden Besucher in den einzelnen Segmenten betrachten, Klickraten auf Kampagnen analysieren und herausfinden, welche Branchen und benutzerspezifischen Segmente und Echtzeit-Kampagnen die besten UmrechnungsInteressenten generiert haben. Nutzen Sie diese Möglichkeit, um den größtmöglichen Nutzen aus Ihrem RTP-Konto zu ziehen.

## RTP-Audience Analytics {#rtp-audience-analytics}

Mit der RTP - Eine Integration haben Sie eine neue Dimension in Ihrer Webanalyse-Oberfläche. RTP verbessert Ihre Webanalyse-Dashboard automatisch durch:

1. Organisations- und Industriedaten
1. Benutzerdefinierte RTP-Segmente
1. Benannte Listen für Konten (kontobasiertes Marketing)

Dadurch verbessern Sie Ihre B2B-Daten und können sich auf relevante Besucher konzentrieren, indem Sie:

1. Ausgehende Kanal
1. Inhalt
1. Retargeting

## Kanal-Bericht {#channel-report}

![](assets/image2014-11-29-12-3a0-3a26.png)

Das RTP-Dashboard hilft Ihnen, die Aufschlüsselung Ihrer Besucher nach Vertikalen und RTP-Segmenten zu verstehen. Sie können die Performance Ihres Besuchers nach Branchen und verschiedenen Marketing-Kampagnen (gebührenpflichtig, kostenlos, sozial) in Bezug auf diese Branche sehen. Das Dashboard bietet außerdem einen Überblick darüber, welche Site-Abschnitte Ihre Besucher je nach Branchentyp anzeigen.

## Verhaltensbericht {#behavioral-report}

Unterschiedliche Verhaltensberichte können in Adobe Analytics auf der Grundlage von Unternehmens-, Industrie- und RTP-Segmentdaten erstellt werden. Diese Flussberichte zeigen den Pfad an, den Besucher von einer Seite oder einem Ereignis zur nächsten nehmen. Dieser Bericht kann Ihnen dabei helfen, herauszufinden, welcher Inhalt Besucher mit Ihrer Site in Kontakt hält.

## RTP-Leistung {#rtp-performance}

Ansicht RTP Kampagne Impressionen und Konversionen unter Benutzerspezifische Links in Adobe Analytics.

Dieser Bericht zu benutzerspezifischen Links zeigt Impressionen und Konversionen von Kampagnen im folgenden Benennungsformat an:

* Impression ISegment: [RTP-Segmentname], ICampaign: [RTP-Kampagne]
* Konversions-ISegment: [RTP-Segmentname], ICampaign: [RTP-Kampagne]

![](assets/custom-links-report.png)

## Einrichtung in Adobe Analytics {#set-up-in-adobe-analytics}

Die Integration verwendet die JavaScript-API, die Adobe Analytics-Angebot verwenden. Bei der Integration werden benutzerspezifische Konversionsvariablen (eVar), benutzerdefinierte Ereignis (Ereignis) und Traffic-Variablen verwendet. Alle müssen innerhalb von AA Admin aktiviert werden. Sie müssen die Konversionsvariablen, benutzerdefinierten Ereignis und Traffic-Variablen in AA festlegen, oder Sie können keine Daten in der Suite sehen, selbst wenn Sie sie in RTP aktiviert haben.

Führen Sie die folgenden Schritte aus, um diese Variablen in AA einzurichten:

1. Gehen Sie zu **Admin Tools** in Ihrem AA-Konto.
1. Wählen Sie die **Report Suite** aus, die bei der Integration verwendet werden soll.
1. Wechseln Sie unter &quot;Einstellungen **bearbeiten&quot;zur** Umrechnung **und wählen Sie **** Umrechnungsvariablen [](http://microsite.omniture.com/t2/help/en_US/reference/#Edit_conversion_variables)**.\
   Wählen Sie die [Umrechnungsvariablennummer](http://microsite.omniture.com/t2/help/en_US/reference/#Conversion_Variables_eVar) aus (wir empfehlen):

   1. 

      1. eVar # 20 für benutzerdefinierte Konvertierungen in der Branche
      1. eVar Nr. 21 für benutzerdefinierte Konversionen in Unternehmen

         >[!NOTE]
         >
         >Wenn diese Anzahl genommen wird, wählen Sie eine andere verfügbare Zahl aus. Richten Sie diese Zahl an der Steckplatznummer in den RTP-Kontoeinstellungen aus.

      1. Status ändern in* aktiviert*

         1. Ändern Sie den Namen in **Industrie** und **Organisation**. (So wird es in der Report Suite angezeigt.)

         1. Ändern Sie &quot;Läuft ab nach&quot;in &quot; **Besuch&quot;.**

1. Wählen Sie unter **Einstellungen bearbeiten **die Option** Umrechnung **und wählen Sie ** [Erfolgsereignisse](http://microsite.omniture.com/t2/help/en_US/reference/#Configure_success_events)**.

1. Wählen Sie die Ereignis-Nummer des benutzerspezifischen Erfolgserfolgs-Ereignisses aus (wir empfehlen):

   1. ereignis20 für RTP-Kampagnen
   1. ereignis21 für RTP-Segmente

      >[!NOTE]
      >
      >Wenn diese Anzahl genommen wird, wählen Sie eine andere verfügbare Zahl aus. Richten Sie diese Zahl an der Steckplatznummer in den RTP-Kontoeinstellungen aus.

   1. Ändern Sie die Namen der beiden Ereignis in **RTP-Kampagnen** und **RTP-Segmente**. Dieser Name wird in der Report Suite angezeigt.

1. Wählen Sie das Feld Typ* *als **Zähler aus (keine Subrelationen)**

1. Gehen Sie unter **Einstellungen** bearbeiten zu ** [Traffic](http://microsite.omniture.com/t2/help/en_US/reference/#Traffic_Variable) **und wählen Sie ** [Traffic-Variablen](http://microsite.omniture.com/t2/help/en_US/reference/#Enable_traffic_variable_reports)**.

   1. Wählen Sie die Eigenschaftennummer der Traffic-Variablen aus (wir empfehlen):

      1. Eigenschaft Nr. 20 - Name: RTP-Segmentorganisation
      1. Eigenschaft Nr. 21 - Name: RTP-Segmentbranche
      1. Eigenschaft Nr. 25 - Name: Kampagne
      1. Eigenschaft Nr. 26 - Name: RTP Kampagne Industry

         >[!NOTE]
         >
         >Wenn diese Anzahl genommen wird, wählen Sie eine andere verfügbare Zahl aus. Diese Zahl an der Steckplatznummer in den RTP-Kontoeinstellungen ausrichten)

      1. Ändern Sie die Namen der 4-Eigenschaften. Dieser Name wird in der Report Suite angezeigt.
   1. Feld Aktiviert zu **aktivieren**
   1. Feld Pfadberichte **aktivieren**


## Einrichtung in Marketing-Echtzeit-Personalisierung (RTP) {#set-up-in-marketo-real-time-personalization-rtp}

1. Wechseln Sie auf der RTP-Plattform zu **Kontoeinstellungen**.

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. Klicken Sie unter **Kontoeinstellungen** auf **Domäne**.
1. Klicken Sie unter **Analytics auf** **Adobe Analytics**.
1. Aktivieren Sie **An **die Variable &quot;Konversion&quot;, &quot;Benutzerdefiniert&quot;und &quot;Traffic&quot;.
1. Weisen Sie die **Slot-Nummern** für Konversions-, Ereignis- und Traffic-Variablen den in AA erstellten Slot-Nummern zu
1. Klicken Sie auf **SPEICHERN**.

![](assets/image2014-11-29-12-3a24-3a42.png)

>[!NOTE]
>
>Unsere empfohlenen Einstellungen für Slots sind
>
>**Konversionsvariablen**
>
>* Branche: Benutzerdefinierte Konvertierungen - Steckplatz 20
>* Benutzerdefinierte Konvertierungen in Unternehmen - Steckplatz 21

>
>
**Benutzerdefinierte Ereignis**
>
>* Benutzerdefiniertes Ereignis der Kampagne - Steckplatz 20
>* Benutzerdefiniertes Segment-Ereignis - Slot 21

>
>
**Traffic-Variablen**
>
>* Traffic-Variable für die Segmentorganisation - Steckplatz 20
>* Traffic-Variable für die Segmentbranche - Steckplatz 21
>* Traffic-Variable der Kampagne - Steckplatz 22
>* Traffic-Variable &quot;Kampagne Industry&quot;- Steckplatz 23

>
>
**Stellen Sie sicher, dass diese Steckplatznummern mit den Variablen und Ereignissen übereinstimmen, die in AA erstellt wurden.**

## Berichte {#reports}

Erstellen Sie erweiterte SiteAdobe Analytics-Berichte gemäß Unternehmensnamen, Branchen- und RTP-Segmenten und Echtzeitdaten zu Kampagnen.

Beispiele für benutzerspezifische Berichte und Dashboard in AA:

* Leistung nach Branche oder definiertem Segment (kontobasierte benannte Listen)
* Aufschlüsselung nach Branche pro KPI-Leistung
* Nach Organisation angezeigte Seiten
* Performance von Marketing-Kanälen nach Unternehmen, Branche, Segmenten

**Berichtsbeispiele**

**Bericht &quot;Top-Branchen&quot;**

** ![](assets/top-industries-report.png)

**

**Organisationsbericht**

![](assets/image2014-11-29-12-3a29-3a42.png)

**RTP-Dashboard erstellen**

Erstellen Sie ein [neues Dashboard](http://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add.html)mit dem Namen **RTP-Dashboard**. Dieses Dashboard hilft Ihnen, die Aufschlüsselung Ihrer Besucher nach Vertikalen und RTP-Segmenten zu verstehen.

1. Klicken Sie auf **Dashboard,** klicken Sie auf** Hinzufügen Dashboard**

1. Benennen des Dashboard **RTP-Dashboards**
1. Wählen Sie das **Dashboard in der Größe** 3 x 2, 2 x 2
1. Erstellen des [Reportlets](http://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add_report.html#task_EC3AFBBAA51C45CEBAF632F841C305B3) und Hinzufügen von [Inhalten zum Dashboard](https://docs.marketo.com/Add%2520content%2520to%2520a%2520dashboard)

Hinzufügen des Reportlets &quot;Industries&quot;zum Dashboard

1. Gehen Sie zu **Custom Conversions**, klicken Sie auf **Industry**

1. Diagramm in **Kreisdiagramm konfigurieren**
1. Klicken Sie auf **Dashboard**, **Reportlet hinzufügen**

1. Benennen Sie den Bericht **Top-Branchen**
1. Ort im Dashboard **RTP-Dashboard**
1. Erstellen Sie **Neu**.

Hinzufügen des Segments-Reportlets zum Dashboard

1. Gehen Sie zu **Site-Metriken, **Klicken Sie auf **Benutzerspezifische Ereignis, Segmente**

1. Diagramm in **Vertikalbalken konfigurieren**
1. Klicken Sie auf **Dashboard**, **Reportlet hinzufügen**

1. Benennen des Berichts **Top-Segmente**
1. Ort im Dashboard **RTP-Dashboard**
1. Erstellen Sie **Neu.**

Ihre Reportlets werden im Dashboard angezeigt.

## Ansicht Impressions and Click (Conversions) in Adobe Analytics {#view-impressions-and-clicks-conversions-in-adobe-analytics}

1. Klicken Sie auf Benutzerspezifische Links.

   ![](assets/sitecatalyst1-1.png)

1. Suchen Sie nach Impressionen zu Segmentnamen und Kampagnen, die die Anzahl der Impressionen für die Kampagne darstellen.\
   ![](assets/sitecatalyst1.png)

1. Suchen Sie nach Konversions- in Ansichten- und Kampagnen-Namen, die die Anzahl der Klicks für die Kampagne darstellen.

   ![](assets/sitecatalyst2.png)

