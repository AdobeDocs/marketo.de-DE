---
unique-page-id: 7504238
description: Benutzerdefinierte RTP-Dashboards in Google Universal Analytics - Marketo Docs - Produktdokumentation
title: Benutzerdefinierte RTP-Dashboards in Google Universal Analytics
exl-id: 712c71b6-74eb-4743-9ca8-50c912278e62
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# Benutzerdefinierte RTP-Dashboards in Google Universal Analytics {#custom-rtp-dashboards-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[Integrieren von RTP in Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

In diesem Beitrag wird erläutert, wie RTP-Dashboards in Google Universal Analytics (GUA) eingerichtet werden. Die Daten, die von RTP an GUA gesendet werden, können als zwei separate benutzerdefinierte Dashboards namens eingerichtet werden:

* RTP B2B
* RTP-Interaktion

## Einrichten eines benutzerdefinierten Dashboards {#setting-up-a-custom-dashboard}

1. Melden Sie sich bei Google Analytics an. Klicken Sie im oberen Menü auf **Berichterstellung** . Klicken Sie auf **Dashboards** und **+Neues benutzerdefiniertes Dashboard**.

   ![](assets/image2015-3-22-16-3a41-3a29.png)

1. Wählen Sie **Leere Arbeitsfläche** aus, fügen Sie einen **Dashboard-Namen** hinzu und klicken Sie auf **Dashboard erstellen**.

1. Klicken Sie auf **Widget hinzufügen** , um ein neues Widget zu erstellen.

   ![](assets/image2015-3-22-16-3a46-3a48.png)

## RTP B2B Dashboard {#rtp-b-b-dashboard}

Mit diesem Dashboard können Benutzer die Leistung ihrer Website aus B2B-Sicht analysieren.

Sie enthält Informationen wie Besuchsquelle und Verhalten vor Ort nach Branche, Umsatz, Größe, kontobasierten Listen und Zielsegmenten.

Das Dashboard besteht aus drei Spalten

* Traffic-Quelle
* Segmentierung
* Firmographie-Drilldown

1. Erstellen Sie ein neues Dashboard mit dem Namen **RTP B2B Dashboard** und definieren Sie die folgenden Widgets:

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
     <li>Widget-Typ: Balken<br></li> 
     <li>Erstellen Sie ein Balkendiagramm, das Folgendes anzeigt: Sitzung</li> 
     <li>Gruppiert nach: Ereignisbezeichnung</li> 
     <li>Pivot nach: Standard-Kanalgruppierung</li> 
     <li>Filter: <br>Nur anzeigen | Ereigniskategorie (enthält) RTP-Segmente</li> 
    </ul><p><img width="300" src="assets/image2015-3-23-11-3a32-3a13.png" data-linked-resource-id="7504247" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Name: Anzahl segmentierter RTP-Benutzer</li> 
     <li>Typ: 2,1 Metrik</li> 
     <li>Anzeigen der folgenden Metrik: Benutzer<br></li> 
     <li>Filter: <br>Nur anzeigen | Ereigniskategorie (enthält) RTP-Segmente</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a6.png" data-linked-resource-id="7504249" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Name: Sitzungen nach Branche</li> 
     <li>Typ: Kreis<br></li> 
     <li>Erstellen Sie ein Tortendiagramm mit folgenden Daten: Sitzungen</li> 
     <li>Gruppiert nach: RTP-Industrie</li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a33-3a27.png" data-linked-resource-id="7504250" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <th> 
    <ul> 
     <li><strong>Name: Sitzungen nach Branche und Kanälen</strong></li> 
     <li><strong>Widget-Typ: Balken</strong></li> 
     <li><strong>Erstellen Sie ein Balkendiagramm, das Folgendes anzeigt: Sitzung</strong></li> 
     <li><strong>Gruppiert nach: RTP-Industrie</strong></li> 
     <li><strong>Pivot nach: Standard-Kanalgruppierung</strong><br><img width="300" src="assets/image2015-3-23-11-3a33-3a52.png" data-linked-resource-id="7504252" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></li> 
    </ul></th> 
   <th> 
    <ul> 
     <li><strong>Name: Segmentierte Sitzungen nach Land</strong></li> 
     <li><strong>Typ: Geomap</strong></li> 
     <li><strong>Metrik "Plot ausgewählt": Land | Sitzungen</strong></li> 
     <li><strong>Wählen Sie eine Region aus: Die Welt</strong></li> 
     <li><strong>Filter: Nur anzeigen | Ereigniskategorie (enthält) RTP-Segmente</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a34-3a18.png" data-linked-resource-id="7504253" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li><strong>Name: Sitzungen nach RTP-Kategorie</strong></li> 
     <li><strong>Typ: Kreis</strong></li> 
     <li><strong>Erstellen Sie ein Tortendiagramm mit folgenden Daten: Sitzungen</strong></li> 
     <li><strong>Gruppiert nach: RTP-Kategorie</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a35-3a1.png" data-linked-resource-id="7504254" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Name: Top-Zielsegmente</li> 
     <li>Typ: Balken</li> 
     <li>Erstellen Sie ein Balkendiagramm, das Folgendes anzeigt: Benutzer</li> 
     <li>Gruppiert nach: Ereignisaktion</li> 
     <li>Filter: Nur anzeigen | Ereigniskategorie (enthält) RTP-Segmente</li> 
    </ul><p><img width="350" src="assets/add-a-widget.png" data-linked-resource-id="11382874" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></th> 
   <th> 
    <ul> 
     <li>Name: Sitzungen von RTP-Gruppen</li> 
     <li>Typ: Balken<br></li> 
     <li>Ein Balkendiagramm mit folgenden Elementen erstellen: Sitzungen</li> 
     <li>Gruppiert nach: RTP-Gruppe</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a35-3a54.png" data-linked-resource-id="7504256" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
  </tr> 
  <tr> 
   <th> </th> 
   <th> 
    <ul> 
     <li>Name: Sitzungen und Ziele nach wichtigsten Segmenten</li> 
     <li>Typ: Tabelle<br></li> 
     <li>Zeigen Sie die folgenden Spalten an: <br>Ereignisbezeichnung | Sitzungen | Zielkonversionsrate</li> 
     <li>Filter: <br>Nur anzeigen | Ereigniskategorie (enthält) RTP-Segmente</li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a36-3a15.png" data-linked-resource-id="7504257" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></th> 
   <th> </th> 
  </tr> 
 </tbody> 
</table>

## RTP-Interaktions-Dashboard {#rtp-engagement-dashboard}

Dieses Dashboard ermöglicht Benutzern die Analyse der RTP-Kampagnenleistung und der Interaktionen mit der Empfehlungsmaschine. Es bietet einen Vergleich von avg. Sitzungsdauer und Seiten pro Sitzung zwischen:

* Nicht aktiviert
* Interagiert (Impressionen und Klicks auf eine personalisierte Kampagne)
* Klicks auf die Recommendations-Engine und die am häufigsten empfohlenen Inhalte

Erstellen Sie ein neues Dashboard mit dem Namen **RTP Engagement Dashboard** und definieren Sie die folgenden Widgets:

![](assets/image2015-3-22-17-3a7-3a19.png)

<table> 
 <thead> 
  <tr> 
   <th> 
    <div> <strong>Spalte 1 Kampagnenexponierung</strong> 
    </div></th> 
   <th> 
    <div> <strong>Spalte 2 Kampagnen-Clickthrough</strong> 
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
     <li>Typ: <strong>2,1 Metrik </strong></li> 
     <li>Zeigt die folgende Metrik an: <strong>Gesamtereignisse</strong></li> 
     <li>Filter:<br><strong>[nur zeigen] Ereigniskategorie (enthält): RTP-Kampagnen</strong><br><strong>[nur zeigen] Ereignisaktion (genau passend): Impression</strong><strong>[zeigen nicht an] Ereignisbezeichnung (enthält): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a37-3a55.png" data-linked-resource-id="7504259" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>Name: <strong>CTA insgesamt (Clickthrough)</strong></li> 
     <li>Typ: <strong>2,1 Metrik </strong></li> 
     <li>Zeigt die folgende Metrik an: <strong>Gesamtereignisse</strong></li> 
     <li>Filter:<br><strong>[nur zeigen] Ereigniskategorie (enthält): RTP-Kampagnen</strong><br><strong>[nur zeigen] Ereignisaktion (genau übereinstimmend): Klicks</strong><strong>[zeigen nicht an] Ereignisbezeichnung (enthält): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a38-3a12.png" data-linked-resource-id="7504261" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> 
    <ul> 
     <li>Name: <strong>CRE - Gesamtklicks</strong></li> 
     <li>Typ: <strong>2,1 Metrik</strong><br></li> 
     <li>Zeigt die folgende Metrik an: <strong>Seitenansichten</strong></li> 
     <li>Filter: <strong>[nur zeigen] Seite (enthält): rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a38-3a30.png" data-linked-resource-id="7504262" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td colspan="1"> 
    <ul> 
     <li>Name: <strong>Durchschnittl. Sitzungsdauer (Interaktion)</strong></li> 
     <li>Typ: <strong>2,1 Metrik </strong></li> 
     <li>Zeigt die folgende Metrik an: <strong>Durchschnittl. Sitzungsdauer</strong></li> 
     <li>Filter:<br><strong>[nur zeigen] Ereigniskategorie (genau übereinstimmend): RTP-Kampagnen</strong><br><strong>[nur zeigen] Ereignisaktion (genau übereinstimmend): impression</strong><strong>[Keine Anzeige] Ereignisbezeichnung (enthalten): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a21.png" data-linked-resource-id="7504264" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Name: <strong>Durchschnittl. Sitzungsdauer (Clickthrough)</strong></li> 
     <li>Typ: <strong>2,1 Metrik </strong></li> 
     <li>Zeigt die folgende Metrik an: <strong>Durchschnittl. Sitzungsdauer</strong></li> 
     <li>Filter:<br><strong>[nur zeigen] Ereigniskategorie (genau übereinstimmend): RTP-Kampagnen</strong><br><strong>[nur zeigen] Ereignisaktion (genau übereinstimmend): Klicks</strong><strong>[Nicht anzeigen] Ereignisbezeichnung (enthalten): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a41-3a37.png" data-linked-resource-id="7504265" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td colspan="1"> 
    <ul> 
     <li>Name: <strong>CRE - Top Recommended Content</strong></li> 
     <li>Typ: <strong>Tabelle</strong><br></li> 
     <li>Zeigen Sie die folgenden Spalten an: <br><strong>Seitentitel | Seitenansichten</strong><br></li> 
     <li>Filter:<br>Filter: <strong>[nur zeigen] Seite (enthält): rcmd</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a41-3a51.png" data-linked-resource-id="7504266" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Name: <strong>Seiten / Sitzung (Interaktion)</strong></li> 
     <li>Typ: <strong>2,1 Metrik </strong></li> 
     <li>Zeigt die folgende Metrik an: <strong>Seiten / Sitzung</strong></li> 
     <li>Filter:<br><strong>[nur zeigen] Ereigniskategorie (genau passend): RTP-Kampagnen</strong></li> 
     <li><strong>[nur zeigen] Ereignisaktion (exakt Übereinstimmung): impression</strong></li> 
     <li><strong>[Nicht anzeigen] Ereignisbezeichnung (enthält): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a10.png" data-linked-resource-id="7504267" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Name: <strong>Seiten/Sitzung (Clickthrough)</strong></li> 
     <li>Typ: <strong>2,1 Metrik </strong></li> 
     <li>Zeigt die folgende Metrik an: <strong>Seiten / Sitzung</strong></li> 
     <li>Filter:<br><strong>[nur zeigen] Ereigniskategorie (genau passend): RTP-Kampagnen</strong></li> 
     <li><strong>[nur zeigen] Ereignisaktion (exakt Übereinstimmung): Klicks</strong></li> 
     <li><strong>[Nicht anzeigen] Ereignisbezeichnung (enthält): #</strong></li> 
    </ul><p><strong><img width="350" src="assets/image2015-3-23-11-3a42-3a32.png" data-linked-resource-id="7504268" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></strong></p></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> 
    <ul> 
     <li>Name: <strong>Impressionen durch CTA</strong></li> 
     <li>Typ: <strong>Tabelle</strong></li> 
     <li>Zeigen Sie die folgenden Spalten an: <strong>Ereignisbezeichnung | Gesamtereignisse | Benutzer</strong></li> 
     <li>Filter:<br><strong>[nur zeigen] Ereigniskategorie (genau übereinstimmend): RTP-Kampagnen</strong><br><strong>[nur zeigen] Ereignisaktion (genau übereinstimmend): impression</strong><strong>[Keine Anzeige] Ereignisbezeichnung (enthalten): #</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a42-3a48.png" data-linked-resource-id="7504269" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> 
    <ul> 
     <li>Name: <strong>Clickthrough by CTA</strong></li> 
     <li>Typ: <strong>Tabelle</strong></li> 
     <li>Zeigen Sie die folgenden Spalten an: <strong>Ereignisbezeichnung | Gesamtereignisse | Benutzer</strong></li> 
     <li>Filter:<br><strong>[nur zeigen] Ereigniskategorie (genau passend): RTP-Kampagnen</strong><br><strong>[nur zeigen] Ereignisaktion (genau passend): Klicks</strong></li> 
    </ul><p><img width="350" src="assets/image2015-3-23-11-3a43-3a4.png" data-linked-resource-id="7504270" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504238"></p></td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>[Integrieren von RTP in Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
>
>[Benutzerspezifische RTP-Berichte in Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-reports-in-google-universal-analytics.md)
