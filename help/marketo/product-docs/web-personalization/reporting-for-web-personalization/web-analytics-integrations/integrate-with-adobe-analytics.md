---
unique-page-id: 2949160
description: Integration mit Adobe Analytics - Marketo Docs - Produktdokumentation
title: Integration mit Adobe Analytics
exl-id: 6ea35811-6f3d-4dc8-91aa-877d613f8e93
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Integration mit Adobe Analytics {#integrate-with-adobe-analytics}

## Einführung {#intro}

Analysieren Sie Ihre Webanalyse aus B2B-Perspektive, indem Sie die Kampagnendaten für Organisation, Branche und Marketo Real-Time Personalization (RTP) in Ihrem Adobe Analytics-Konto anzeigen.

Dieses Dokument ermöglicht die Integration zwischen Marketo Real-Time Personalization (RTP) und Adobe Adobe Analytics. Mithilfe von RTP-Daten können Sie Trends in allen auf Ihre Site besuchten Branchensegmenten und Organisationen erkennen und analysieren sowie die Effektivität Ihrer RTP-Kampagnen messen. So erhalten Sie Einblicke und Analysen, um optimale Ergebnisse zu erzielen.

Sie können dies erreichen, indem Sie sich Metriken wie die Anzahl neuer oder wiederkehrender Besucher in den einzelnen Segmenten ansehen, Klickraten für Kampagnen analysieren und herausfinden, welche Branchen und benutzerdefinierten Segmente und Echtzeit-Kampagnen zu den besten Konversion-Leads führten. Nutzen Sie diese Fähigkeit, um den größtmöglichen Nutzen aus Ihrem RTP-Konto zu ziehen.

## RTP-Audience Analytics {#rtp-audience-analytics}

Mit der RTP - AA-Integration haben Sie eine neue Dimension in Ihrer Web-Analytics-Oberfläche. RTP verbessert Ihre Web-Analyse-Dashboards automatisch mit:

1. Organisations- und Industriedaten
1. Benutzerdefinierte RTP-Segmente
1. Listen mit benannten Konten (Account-Based Marketing)

Dadurch werden Ihre B2B-Daten verbessert und Sie können sich durch Optimierung auf relevante Besucher konzentrieren:

1. Ausgehende Kanäle
1. Inhalt
1. Retargeting

## Kanalbericht {#channel-report}

![](assets/image2014-11-29-12-3a0-3a26.png)

Das RTP-Dashboard hilft Ihnen, die Aufschlüsselung Ihrer Besucher nach Vertikalen und RTP-Segmenten zu verstehen. Sie können die Leistung Ihrer Besucher entsprechend der Branche und den verschiedenen mit dieser Branche verbundenen Marketing-Kampagnen (gebührenpflichtig, kostenlos, sozial) anzeigen. Das Dashboard bietet außerdem einen allgemeinen Überblick darüber, welche Sitebereiche Ihre Besucher je nach Branchentyp anzeigen.

## Verhaltensbericht {#behavioral-report}

In Adobe Analytics können basierend auf Unternehmens-, Branchen- und RTP-Segmentdaten verschiedene Verhaltensberichte erstellt werden. Diese Flussberichte visualisieren den Pfad, den Besucher von einer Seite oder einem Ereignis zur nächsten nehmen. Dieser Bericht kann Ihnen dabei helfen festzustellen, durch welche Inhalte Besucher mit Ihrer Site interagieren.

## RTP-Leistung {#rtp-performance}

Zeigen Sie die RTP-Kampagnenimpressionen und -konversionen unter Benutzerspezifische Links in Adobe Analytics an.

Dieser Bericht zu benutzerspezifischen Links zeigt Impressionen und Konversionen von Kampagnen im folgenden Namensformat:

* Impression ISegment: [RTP-Segmentname], ICampaign: [RTP-Kampagnenname]
* Konversions-ISegment: [RTP-Segmentname], ICampaign: [RTP-Kampagnenname]

![](assets/custom-links-report.png)

## Einrichtung in Adobe Analytics {#set-up-in-adobe-analytics}

Die Integration verwendet die von Adobe Analytics angebotene JavaScript-API. Benutzerdefinierte Konversionsvariablen (eVar), benutzerspezifische Ereignisse (Ereignis) und Traffic-Variablen werden in der Integration verwendet. Alle müssen in einem Administrator aktiviert werden. Sie müssen die Konversionsvariablen, benutzerdefinierten Ereignisse und Traffic-Variablen in AA festlegen. Andernfalls werden keine Daten in der Suite angezeigt, selbst wenn Sie sie in RTP aktiviert haben.

Führen Sie die folgenden Schritte aus, um diese Variablen in AA einzurichten:

1. Navigieren Sie zu **Admin Tools** in Ihrem AA-Konto.
1. Wählen Sie die **Report Suite** für die Integration verwendet werden.
1. under **Einstellungen bearbeiten**, gehen Sie zu **Konversion** und wählen **[Konversionsvariablen](https://microsite.omniture.com/t2/help/en_US/reference/#Edit_conversion_variables)**.\
   Wählen Sie die [Konversionsvariable](https://microsite.omniture.com/t2/help/en_US/reference/#Conversion_Variables_eVar) number (empfohlen):

   1. eVar # 20 für benutzerdefinierte Branchen-Konversionen
   1. eVar # 21 für benutzerspezifische Unternehmenskonversionen

   >[!NOTE]
   >
   >Wenn diese Anzahl angenommen wird, wählen Sie eine andere verfügbare Zahl aus. Richten Sie diese Zahl an der Steckplatznummer in den RTP-Kontoeinstellungen aus.

   1. Status ändern in _Aktiviert_.

      1. Name ändern in **Branche** und **Einrichtung**. (So wird er in der Report Suite angezeigt.)

      1. Ändern Sie das Feld Ablauf nach in **Besuch**.

1. under **Einstellungen bearbeiten** gehen Sie zu **Konversion** und wählen **[Erfolgsereignisse](https://microsite.omniture.com/t2/help/en_US/reference/#Configure_success_events)**.

   1. Wählen Sie die Ereignisnummer für benutzerspezifische Erfolgsereignisse aus (wir empfehlen):

      1. event20 für RTP-Kampagnen
      1. event21 für RTP-Segmente

      >[!NOTE]
      >
      >Wenn diese Anzahl angenommen wird, wählen Sie eine andere verfügbare Zahl aus. Richten Sie diese Zahl an der Steckplatznummer in den RTP-Kontoeinstellungen aus.

      1. Ändern Sie die beiden Ereignisnamen in **RTP-Kampagnen** und **RTP-Segmente**. Dieser Name wird in der Report Suite angezeigt.

   1. Wählen Sie das Feld Typ aus, das **Zähler (keine Subrelationen)**

1. under **Einstellungen bearbeiten** gehen Sie zu **[Traffic](https://microsite.omniture.com/t2/help/en_US/reference/#Traffic_Variable)** und wählen **[Traffic-Variablen](https://microsite.omniture.com/t2/help/en_US/reference/#Enable_traffic_variable_reports)**.

   1. Wählen Sie die Eigenschaftsnummer der Traffic-Variablen aus (wir empfehlen Ihnen):

      1. Eigenschaft Nr. 20 - Name: RTP Segment Organization
      1. Eigenschaft Nr. 21 - Name: RTP Segment Industry
      1. Eigenschaft Nr. 25 - Name: Campaign Organization
      1. Eigenschaft Nr. 26 - Name: RTP Campaign Industry

      >[!NOTE]
      >
      >Wenn diese Anzahl angenommen wird, wählen Sie eine andere verfügbare Zahl aus. Stellen Sie diese Zahl mit der Nummer des Slots in den RTP-Kontoeinstellungen ein.)

      1. Ändern Sie die vier Eigenschaftsnamen. Dieser Name wird in der Report Suite angezeigt.

   1. Wählen Sie das Feld Aktiviert für **Aktiviert**.

   1. Wählen Sie das Feld Pfadberichte aus **Aktiviert**.

## Einrichtung in Marketo Real-Time Personalization (RTP) {#set-up-in-marketo-real-time-personalization-rtp}

1. Navigieren Sie in der RTP-Plattform zu **Kontoeinstellungen**.

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. under **Kontoeinstellungen** klicken **Domäne**.
1. under **Analytics, klicken Sie** **Adobe Analytics**.
1. drehen **on** Die Variablen &quot;Konversion&quot;, &quot;Benutzerdefiniert&quot;und &quot;Traffic&quot;werden umgeschaltet.
1. Zuweisen von Konversions-, Ereignis- und Traffic-Variablen **Zeitnischen** , um die in AA erstellten Slotnummern zu erhalten.
1. Klicks **Speichern**.

![](assets/image2014-11-29-12-3a24-3a42.png)

>[!NOTE]
>
>Unsere empfohlenen Einstellungen für Slots sind
>
>**Konversionsvariablen**
>
>* Benutzerdefinierte Konversion in der Branche - Steckplatz 20
>* Benutzerdefinierte Konversionen der Organisation - Steckplatz 21
>
>**Benutzerspezifische Ereignisse**
>
>* Benutzerdefiniertes Kampagnenereignis - Steckplatz 20
>* Benutzerdefiniertes Segmentereignis - Steckplatz 21
>
>**Traffic-Variablen**
>
>* Traffic-Variable der Segmentorganisation - Steckplatz 20
>* Traffic-Variable der Segmentbranche - Steckplatz 21
>* Traffic-Variable der Campaign-Organisation - Steckplatz 22
>* Traffic-Variable der Kampagnenbranche - Steckplatz 23
>
>**Stellen Sie sicher, dass diese Slot-Zahlen mit den in AA erstellten Variablen und Ereignisnummern übereinstimmen.**

## Berichte {#reports}

Erstellen Sie erweiterte SiteAdobe Analytics-Berichte entsprechend den Organisationsnamen, Branchen und RTP-Segmenten sowie Echtzeitkampagnendaten.

Beispiele für benutzerdefinierte Berichte und Dashboards in AA:

* Leistung nach Branche oder definiertem Segment (kontobasierte spezifische Listen)
* Aufschlüsselung nach Branche nach KPI-Leistung
* Angesehene Seiten pro Organisation
* Marketing-Kanal-Performance nach Organisation, Branche, Segmenten

**- Berichtsbeispiele -**

**Bericht &quot;Topbranchen&quot;**

![](assets/top-industries-report.png)

**Organisationsbericht**

![](assets/image2014-11-29-12-3a29-3a42.png)

**RTP-Dashboard erstellen**

Erstellen Sie eine [neues Dashboard](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add.html)aufgerufen **RTP-Dashboard**. Dieses Dashboard hilft Ihnen, die Aufschlüsselung Ihrer Besucher nach Vertikalen und RTP-Segmenten zu verstehen.

1. Klicks **Dashboard,** click **Dashboard hinzufügen**.

1. Benennen Sie das Dashboard. **RTP-Dashboard**.

1. Wählen Sie die **Dashboard-Größe** 3 x 2, 2 x 2.

1. Erstellen Sie die [Reportlet](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add_report.html#task_EC3AFBBAA51C45CEBAF632F841C305B3) und hinzufügen [Inhalt des Dashboards](https://docs.marketo.com/Add%2520content%2520to%2520a%2520dashboard).

Hinzufügen des Branchen-Reportlets zum Dashboard

1. Navigieren Sie zu **Benutzerdefinierte Konversionen**, klicken Sie auf **Branche**.

1. Konfigurieren des Diagramms zu **Tortendiagramm**.

1. Klicken Sie auf **Dashboard**, hinzufügen **Reportlet**.

1. Benennen des Berichts **Topbranchen**.

1. Im Dashboard platzieren **RTP-Dashboard**.

1. Erstellen **Neu**.

Hinzufügen des Segments-Reportlets zum Dashboard

1. Navigieren Sie zu **Site-Metriken**. Klicken Sie auf **Benutzerspezifische Ereignisse**, **Segmente**.

1. Konfigurieren des Diagramms zu **Vertikalbalken**.

1. Klicken Sie auf **Dashboard**, hinzufügen **Reportlet**.

1. Benennen des Berichts **Top-Segmente**.

1. Im Dashboard platzieren **RTP-Dashboard**.

1. Erstellen **Neu**.

Ihre Reportlets werden im Dashboard angezeigt.

## Impressionen und Klicks (Konversionen) in Adobe Analytics anzeigen {#view-impressions-and-clicks-conversions-in-adobe-analytics}

1. Klicks **Benutzerspezifische Links**.

   ![](assets/sitecatalyst1-1.png)

1. Suchen Sie nach Impressionen , um Segment- und Kampagnennamen anzuzeigen, die die Anzahl der Impressionen für die Kampagne darstellen.\
   ![](assets/sitecatalyst1.png)

1. Suchen Sie nach Konversion , um Segment- und Kampagnennamen anzuzeigen, die die Anzahl der Klicks für die Kampagne darstellen.

   ![](assets/sitecatalyst2.png)
