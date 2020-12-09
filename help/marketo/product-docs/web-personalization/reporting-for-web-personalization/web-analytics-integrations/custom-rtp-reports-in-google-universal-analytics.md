---
unique-page-id: 7504218
description: Benutzerspezifische RTP-Berichte in Google Universal Analytics - Marketing Docs - Produktdokumentation
title: Benutzerspezifische RTP-Berichte in Google Universal Analytics
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---


# Benutzerspezifische RTP-Berichte in Google Universal Analytics {#custom-rtp-reports-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[RTP in Google Universal Analytics integrieren](integrate-rtp-with-google-universal-analytics.md)

In diesem Beitrag wird beschrieben, wie RTP-benutzerspezifische Berichte für Google Universal Analytics (GUA) eingerichtet werden.  Die Daten, die von RTP an GUA gesendet werden, können als zwei separate benutzerspezifische Berichte eingerichtet werden:

* RTP B2B
* RTP-Interaktion

## Einrichten eines benutzerspezifischen Berichts {#setting-up-a-custom-report}

1. Melden Sie sich bei Google Analytics an.
1. Klicken Sie auf **Anpassung **im oberen Menü.
1. Klicken Sie auf **+Neuer benutzerdefinierter Bericht.**

** ![](assets/image2015-3-22-16-3a10-3a48.png)

**

## RTP B2B-Bericht {#rtp-b-b-report}

1. Benennen Sie den Bericht **RTP B2B Report**.
1. Name der ersten Registerkarte **Branche **

   1. (Hinweis: Sie werden diese Registerkarte **** Duplikat nehmen und weitere ähnliche erstellen - Schritt 5)

1. Wählen Sie den Berichtstyp** Explorer*.\
   ** ![](assets/image2015-3-22-16-3a15-3a25.png)

   **

1. Wählen Sie im Abschnitt **Metrikgruppen** die Metriken aus, die für Ihr Geschäft relevant sind.

   1. Wir empfehlen Folgendes:\
      ** ![](assets/image2015-3-22-16-3a16-3a40.png)

      **

1. Duplikat dieses Registers viermal und benennen Sie sie:

   1. **Branche**
   1. **Gruppe**
   1. **Kategorie**
   1. **ABM**
   1. **Organisationen**

   ![](assets/image2015-3-22-16-3a17-3a41.png)

1. Legen Sie im Abschnitt **Dimensionen-Drilldowns** die entsprechenden Dimensionen für jede Registerkarte wie unten beschrieben fest.

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Registerkartenname 
    </div></th> 
   <th> 
    <div>
      Dimensionen-Drilldowns 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Branche</td> 
   <td><img src="assets/1.png" data-linked-resource-id="7514675" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Gruppe</td> 
   <td><img src="assets/2.png" data-linked-resource-id="7514674" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Kategorie</td> 
   <td><img src="assets/3.png" data-linked-resource-id="7514673" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>ABM</td> 
   <td><img src="assets/5.png" data-linked-resource-id="7514677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Organisationen</td> 
   <td><img src="assets/5.png" data-linked-resource-id="7514677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
 </tbody> 
</table>

1. Stellen Sie keine Filter ein und stellen Sie sicher, dass dieser Bericht für **Alle Website-Daten ** verfügbar ist (oder ändern Sie ihn gegebenenfalls entsprechend dem jeweiligen Analytics-Konto).
1. Klicken Sie auf **Speichern**.\
   ![](assets/image2015-3-22-16-3a21-3a23.png)

## RTP-Interaktionsbericht {#rtp-engagement-report}

1. Benennen Sie den Bericht &quot; **RTP-Interaktion&quot;.**
1. Name der ersten Registerkarte auf &quot; **Alle Interaktionen&quot;**

   1. (Hinweis: Sie werden diese Registerkarte Duplikat und weitere ähnliche erstellen - Schritt 5)

1. Wählen Sie den Berichtstyp **Explorer** aus.\
   ![](assets/image2015-3-22-16-3a23-3a36.png)

1. Wählen Sie im Abschnitt Metrikgruppen die Metriken aus, die für Ihr Geschäft relevant sind. Hier eine Empfehlung:\
   ![](assets/image2015-3-22-16-3a24-3a57.png)

1. Duplikat dieses Registers viermal und benennen Sie sie:

   1. **Alle Interaktionen**
   1. **Engagement der Branche**
   1. **Interaktion nach Gruppe**
   1. **Interaktion nach Kategorie**
   1. **Interaktion durch ABM**

   ** ![](assets/image2015-3-22-16-3a26-3a21.png)\**

1. Legen Sie im Abschnitt **Dimensionen-Drilldowns** die entsprechenden Dimensionen für jede Registerkarte wie folgt fest:

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Registerkartenname 
    </div></th> 
   <th> 
    <div>
      Dimensionen-Drilldowns 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Alle Interaktionen</td> 
   <td><img src="assets/a.png" data-linked-resource-id="7514683" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Interaktion durch ABM</td> 
   <td><img width="277" src="assets/4.png" data-linked-resource-id="7514678" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Interaktion nach Kategorie</td> 
   <td><img src="assets/a.png" data-linked-resource-id="7514683" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Interaktion nach Gruppe</td> 
   <td><img src="assets/c.png" data-linked-resource-id="7514681" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
  <tr> 
   <td>Engagement der Branche</td> 
   <td><img src="assets/b.png" data-linked-resource-id="7514682" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
 </tbody> 
</table>

1. Legen Sie die folgenden Filter fest:
1. 

<table> 
 <thead> 
  <tr> 
   <th> 
    <div>
      Inc/Exc 
    </div></th> 
   <th> 
    <div>
      Feld 
    </div></th> 
   <th> 
    <div>
      Übereinstimmungstyp 
    </div></th> 
   <th> 
    <div>
      Werte 
    </div></th> 
   <th colspan="1"> 
    <div>
      Kommentare 
    </div></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><p>Einschließen</p></td> 
   <td><p>Ereignis-Kategorie</p></td> 
   <td>Regex</td> 
   <td>RTP-Kampagnen|RTP-Recommendations|RTP-Segmente</td> 
   <td colspan="1">Filtert alle anderen benutzerspezifischen Ereignis, die nicht mit RTP in Zusammenhang stehen</td> 
  </tr> 
  <tr> 
   <td>Ausschließen</td> 
   <td>Ereignis</td> 
   <td>Regex</td> 
   <td>#</td> 
   <td colspan="1">Ermöglicht das Filtern aus der Kampagne der Berichte mit # im Namen der Kampagne</td> 
  </tr> 
 </tbody> 
</table>

1. Setzen Sie diesen Bericht auf verfügbar für **Alle Website-Daten **(oder ändern Sie ihn gegebenenfalls)

   ![](assets/image2015-3-22-16-3a29-3a5.png)

1. Klicken Sie auf **Speichern**.

![](assets/image2015-3-22-16-3a30-3a0.png)

>[!NOTE]
>
>**Verwandte Artikel**
>
>[RTP in Google Universal Analytics integrieren](integrate-rtp-with-google-universal-analytics.md)
>
>[Benutzerdefinierte RTP-Dashboard in Google Universal Analytics](custom-rtp-dashboards-in-google-universal-analytics.md)

