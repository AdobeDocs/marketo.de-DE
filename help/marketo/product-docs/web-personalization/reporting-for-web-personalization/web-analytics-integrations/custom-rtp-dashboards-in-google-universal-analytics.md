---
unique-page-id: 7504238
description: Benutzerspezifische RTP-Dashboard in Google Universal Analytics - Marketing Docs - Produktdokumentation
title: Benutzerdefinierte RTP-Dashboard in Google Universal Analytics
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 0%

---


# Benutzerdefinierte RTP-Dashboard in Google Universal Analytics {#custom-rtp-dashboards-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[RTP in Google Universal Analytics integrieren](integrate-rtp-with-google-universal-analytics.md)

In diesem Beitrag wird das Einrichten von RTP-Dashboards in Google Universal Analytics (GUA) erläutert.  Die Daten, die von RTP an GUA gesendet werden, können als zwei separate benutzerdefinierte Dashboard eingerichtet werden:

* RTP B2B
* RTP-Interaktion

## Einrichten eines benutzerspezifischen Dashboards {#setting-up-a-custom-dashboard}

1. Melden Sie sich bei Google Analytics an. Klicken Sie auf **Berichte **im oberen Menü. Klicken Sie auf **Dashboards **und **+Neues benutzerdefiniertes Dashboard.**

   ![](assets/image2015-3-22-16-3a41-3a29.png)

1. Wählen Sie &quot; **Leere Arbeitsfläche**&quot;, fügen Sie einen **Dashboard-Namen** hinzu und klicken Sie auf &quot;Dashboard **erstellen&quot;**.

1. Klicken Sie auf **Hinzufügen Widget** , um ein neues Widget zu erstellen.\
   ![](assets/image2015-3-22-16-3a46-3a48.png)

## RTP B2B-Dashboard {#rtp-b-b-dashboard}

Dieses Dashboard ermöglicht es Benutzern, ihre Website-Performance aus einer B2B-Perspektive zu analysieren.

Es bietet Informationen wie Besuchsquelle und Onsite-Verhalten nach Branche, Umsatz, Größe, Kontobasierte Listen und Zielgruppe-Segmenten.

Das Dashboard besteht aus 3 Spalten

* Traffic-Quelle
* Segmentierung
* Firmografischer Drilldown

1. Erstellen Sie ein neues Dashboard mit dem Namen **RTP B2B-Dashboard **und definieren Sie die folgenden Widgets:

![](assets/image2015-3-22-16-3a50-3a3.png)

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Spalte 1 - Traffic-Quellen 
    </div></th> 
   <th> 
    <div> <strong>Spalte 2 - Segmentierung</strong> 
    </div></th> 
   <th> 
    <div> <strong>Spalte 3 - Firmografischer Drilldown</strong> 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Name: Sitzungen nach Segmenten und Kanälen</li> 
     <li>Widget-Typ: Bar<br></li> 
     <li>Erstellen Sie ein Balkendiagramm, das Folgendes zeigt: Sitzung</li> 
     <li>Gruppiert nach: Beschriftung des Ereignisses</li> 
     <li>Pivot nach: Standardmäßige Kanal-Gruppierung</li> 
     <li>Filter: <br>Nur anzeigen | Ereignis Kategorie (enthält) RTP-Segmente</li> 
    </ul><p><img width="300" src="assets/image2015-3-23-11-3a32-3a13.png" data-linked-resource-id="7504247" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Name: Anzahl der segmentierten RTP-Benutzer</li> 
     <li>Typ: 2.1 Metrik</li> 
     <li>Zeigt die folgende Metrik an: Benutzer<br></li> 
     <li>Filter: <br>Nur anzeigen | Ereignis Kategorie (enthält) RTP-Segmente</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a6.png" data-linked-resource-id="7504249" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Name: Sitzungen nach Branchen</li> 
     <li>Typ: Kuchen<br></li> 
     <li>Erstellen Sie ein Kreisdiagramm, das Folgendes zeigt: Sitzungen</li> 
     <li>Gruppiert nach: RTP-Branche</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a27.png" data-linked-resource-id="7504250" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <th> 
    <ul> 
     <li><strong>Name: Sitzungen der Industrie und der Kanal</strong></li> 
     <li><strong>Widget-Typ: Bar</strong></li> 
     <li><strong>Erstellen Sie ein Balkendiagramm, das Folgendes zeigt: Sitzung</strong></li> 
     <li><strong>Gruppiert nach: RTP-Branche</strong></li> 
     <li><strong>Pivot nach: Standardmäßige Kanal-Gruppierung</strong><br><img width="300" src="assets/image2015-3-23-11-3a33-3a52.png" data-linked-resource-id="7504252" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></li> 
    </ul></th> 
   <th> 
    <ul> 
     <li><strong>Name: Segmentierte Sitzungen nach Land</strong></li> 
     <li><strong>Typ: Geomap</strong></li> 
     <li><strong>Ausgewählte Metrik zeichnen: Land | Sitzungen</strong></li> 
     <li><strong>Wählen Sie einen Bereich aus: Die Welt</strong></li> 
     <li><strong>Filter: Nur anzeigen | Ereignis Kategorie (enthält) RTP-Segmente</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a34-3a18.png" data-linked-resource-id="7504253" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li><strong>Name: Sitzungen der RTP-Kategorie</strong></li> 
     <li><strong>Typ: Kuchen</strong></li> 
     <li><strong>Erstellen Sie ein Kreisdiagramm, das Folgendes zeigt: Sitzungen</strong></li> 
     <li><strong>Gruppiert nach: RTP-Kategorie</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a1.png" data-linked-resource-id="7504254" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Name: Wichtigste Zielgruppen</li> 
     <li>Typ: Bar</li> 
     <li>Erstellen Sie ein Balkendiagramm, das Folgendes zeigt: Benutzer</li> 
     <li>Gruppiert nach: Ereignis-Aktion</li> 
     <li>Filter: Nur anzeigen | Ereignis Kategorie (enthält) RTP-Segmente</li> 
    </ul><p><img width="350" src="assets/add-a-widget.png" data-linked-resource-id="11382874" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li>Name: Sitzungen nach RTP-Gruppen</li> 
     <li>Typ: Bar<br></li> 
     <li>Erstellen Sie ein Balkendiagramm, das Folgendes zeigt: Sitzungen</li> 
     <li>Gruppiert nach: RTP-Gruppe</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a35-3a54.png" data-linked-resource-id="7504256" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Name: Sitzungen und Ziele nach Hauptsegmenten</li> 
     <li>Typ: Verzeichnis<br></li> 
     <li>Zeigen Sie die folgenden Spalten an: <br>Ereignis | Sitzungen | Ziel Konversionsrat</li> 
     <li>Filter: <br>Nur anzeigen | Ereignis Kategorie (enthält) RTP-Segmente</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a36-3a15.png" data-linked-resource-id="7504257" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
   <th> </th> 
  </tr> 
 </tbody> 
</table>

## RTP-Interaktions-Dashboard {#rtp-engagement-dashboard}

Dieses Dashboard ermöglicht es Benutzern, ihre RTP-Kampagne-Performance und Empfehlungs-Engine-Interaktionen zu analysieren. Es bietet einen Vergleich von Avg. Sitzungsdauer und Seiten pro Sitzung zwischen:

* 

   * Nicht aktiviert
   * Interagiert (Impressionen und Klicks auf eine personalisierte Kampagne)
   * Klicks auf die Recommendations-Engine und die am häufigsten empfohlenen Inhalte

Erstellen Sie ein neues Dashboard mit dem Namen **RTP-Interaktions-Dashboard** und definieren Sie die folgenden Widgets:

![](assets/image2015-3-22-17-3a7-3a19.png)

<table> 
 <thead> 
  <tr> 
   <th> 
    <div> <strong>Spalte 1 Kampagnen Exposition</strong> 
    </div></th> 
   <th> 
    <div> <strong>Spalte 2 Kampagnen Clickthrough</strong> 
    </div></th> 
   <th> 
    <div> <strong>Spalte 3 Recommendations-Engine</strong> 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Name: <strong>CTA insgesamt (Interaktion)</strong></li> 
     <li>Typ: <strong>2.1 Metrik </strong></li> 
     <li>Zeigt die folgende Metrik an: <strong>Ereignisse insgesamt</strong></li> 
     <li>Filter:<br><strong>[nur anzeigen] Ereignis-Kategorie (enthält): RTP-Kampagnen</strong><br><strong>[nur anzeigen] Ereignis-Aktion (exakt Übereinstimmung): Impression</strong><strong>[not show] Ereignis Label (contains): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a37-3a55.png" data-linked-resource-id="7504259" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>Name: <strong>CTA insgesamt (Durchklickrate)</strong></li> 
     <li>Typ: <strong>2.1 Metrik </strong></li> 
     <li>Zeigt die folgende Metrik an: <strong>Ereignisse insgesamt</strong></li> 
     <li>Filter:<br><strong>[nur anzeigen] Ereignis-Kategorie (enthält): RTP-Kampagnen</strong><br><strong>[nur anzeigen] Ereignis-Aktion (exakt Übereinstimmung): Clicks</strong><strong>[Keine Anzeige] Ereignis Label (enthält): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a38-3a12.png" data-linked-resource-id="7504261" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>Name: <strong>CRE - Gesamtklicks</strong></li> 
     <li>Typ: <strong>2.1 Metrik</strong><br></li> 
     <li>Zeigt die folgende Metrik an: <strong>Seitenansichten</strong></li> 
     <li>Filter: <strong>[nur anzeigen] Seite (enthält): rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a30.png" data-linked-resource-id="7504262" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> 
    <ul> 
     <li>Name: <strong>Durchschn. Sitzungsdauer (Einsatz)</strong></li> 
     <li>Typ: <strong>2.1 Metrik </strong></li> 
     <li>Zeigt die folgende Metrik an: <strong>Durchschn. Sitzungsdauer</strong></li> 
     <li>Filter:<br><strong>[nur anzeigen] Ereignis-Kategorie (exakt Übereinstimmung): RTP-Kampagnen</strong><br><strong>[nur anzeigen] Ereignis-Aktion (exakt Übereinstimmung): impression</strong><strong>[Nicht anzeigen] Ereignis Label (enthält): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a21.png" data-linked-resource-id="7504264" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Name: <strong>Durchschn. Sitzungsdauer (Durchklickrate)</strong></li> 
     <li>Typ: <strong>2.1 Metrik </strong></li> 
     <li>Zeigt die folgende Metrik an: <strong>Durchschn. Sitzungsdauer</strong></li> 
     <li>Filter:<br><strong>[nur anzeigen] Ereignis-Kategorie (exakt Übereinstimmung): RTP-Kampagnen</strong><br><strong>[nur anzeigen] Ereignis-Aktion (exakt Übereinstimmung): klickt</strong><strong>[Keine Anzeige] Ereignis Label (enthält): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a37.png" data-linked-resource-id="7504265" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Name: <strong>CRE - Empfohlene Inhalte</strong></li> 
     <li>Typ: <strong>Verzeichnis</strong><br></li> 
     <li>Zeigen Sie die folgenden Spalten an: <br><strong>Seitentitel | Seitenansichten</strong><br></li> 
     <li>Filter:<br>Filter: <strong>[nur anzeigen] Seite (enthält): rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a51.png" data-linked-resource-id="7504266" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Name: <strong>Seiten/Sitzung (Interaktion)</strong></li> 
     <li>Typ: <strong>2.1 Metrik </strong></li> 
     <li>Zeigt die folgende Metrik an: <strong>Seiten/Sitzung</strong></li> 
     <li>Filter:<br><strong>[nur anzeigen] Ereignis-Kategorie (exakt Übereinstimmung): RTP-Kampagnen</strong></li> 
     <li><strong>[nur anzeigen] Ereignis-Aktion (exakt Übereinstimmung): impression</strong></li> 
     <li><strong>[Nicht anzeigen] Ereignis-Beschriftung (enthält): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a10.png" data-linked-resource-id="7504267" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Name: <strong>Seiten/Sitzung (Clickthrough)</strong></li> 
     <li>Typ: <strong>2.1 Metrik </strong></li> 
     <li>Zeigt die folgende Metrik an: <strong>Seiten/Sitzung</strong></li> 
     <li>Filter:<br><strong>[nur anzeigen] Ereignis-Kategorie (exakt Übereinstimmung): RTP-Kampagnen</strong></li> 
     <li><strong>[nur anzeigen] Ereignis-Aktion (exakt Übereinstimmung): Klicks</strong></li> 
     <li><strong>[Nicht anzeigen] Ereignis-Beschriftung (enthält): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a42-3a32.png" data-linked-resource-id="7504268" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Name: <strong>Impressionen nach CTA</strong></li> 
     <li>Typ: <strong>Verzeichnis</strong></li> 
     <li>Zeigen Sie die folgenden Spalten an: <strong>Ereignis | Ereignisse insgesamt | Benutzer</strong></li> 
     <li>Filter:<br><strong>[nur anzeigen] Ereignis-Kategorie (exakt Übereinstimmung): RTP-Kampagnen</strong><br><strong>[nur anzeigen] Ereignis-Aktion (exakt Übereinstimmung): impression</strong><strong>[Nicht anzeigen] Ereignis Label (enthält): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a48.png" data-linked-resource-id="7504269" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Name: <strong>Clickthrough nach CTA</strong></li> 
     <li>Typ: <strong>Verzeichnis</strong></li> 
     <li>Zeigen Sie die folgenden Spalten an: <strong>Ereignis | Ereignisse insgesamt | Benutzer</strong></li> 
     <li>Filter:<br><strong>[nur anzeigen] Ereignis-Kategorie (exakt Übereinstimmung): RTP-Kampagnen</strong><br><strong>[nur anzeigen] Ereignis-Aktion (exakt Übereinstimmung): Klicks</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a43-3a4.png" data-linked-resource-id="7504270" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**Verwandte Artikel**
>
>[RTP in Google Universal Analytics integrieren](integrate-rtp-with-google-universal-analytics.md)
>
>[Benutzerspezifische RTP-Berichte in Google Universal Analytics](custom-rtp-reports-in-google-universal-analytics.md)

