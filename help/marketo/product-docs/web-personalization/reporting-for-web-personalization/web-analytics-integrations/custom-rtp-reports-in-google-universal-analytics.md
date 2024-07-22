---
unique-page-id: 7504218
description: Benutzerdefinierte RTP-Berichte in Google Universal Analytics - Marketo Docs - Produktdokumentation
title: Benutzerdefinierte RTP-Berichte in Google Universal Analytics
exl-id: c8b1e653-03b8-48bc-b80d-3e6cdf3485c3
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 4%

---

# Benutzerdefinierte RTP-Berichte in Google Universal Analytics {#custom-rtp-reports-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[Integrieren von RTP in Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

In diesem Artikel wird beschrieben, wie Sie benutzerdefinierte RTP-Berichte für Google Universal Analytics (GUA) einrichten.  Die Daten, die von RTP an GUA gesendet werden, können in zwei separaten benutzerdefinierten Berichten namens eingerichtet werden:

* RTP B2B
* RTP-Interaktion

## Einrichten eines benutzerspezifischen Berichts {#setting-up-a-custom-report}

1. Melden Sie sich bei Google Analytics an.

1. Klicken Sie im oberen Menü auf **Anpassung** .

1. Klicken Sie auf **+Neuer benutzerspezifischer Bericht**.

![](assets/image2015-3-22-16-3a10-3a48.png)

## RTP B2B-Bericht {#rtp-b-b-report}

1. Nennen Sie den Bericht &quot;**RTP B2B Report&quot;**.

1. Nennen Sie die erste Registerkarte mit dem Namen &quot;**Branche**&quot;.

>[!NOTE]
>
>Sie werden **diese Registerkarte duplizieren** und weitere ähnliche hinzufügen - Schritt 5)

1. Wählen Sie den Berichtstyp **Explorer** aus.

   ![](assets/image2015-3-22-16-3a15-3a25.png)

1. Wählen Sie im Abschnitt **Metrikgruppen** die Metriken aus, die für Ihr Unternehmen relevant sind.

   a. Wir empfehlen Folgendes:

   ![](assets/image2015-3-22-16-3a16-3a40.png)

1. Duplizieren Sie diese Registerkarte viermal und benennen Sie sie:

   1. **Branche**
   1. **Gruppe**
   1. **Kategorie**
   1. **ABM**
   1. **Organisationen**

   ![](assets/image2015-3-22-16-3a17-3a41.png)

1. Legen Sie im Bereich **Dimensionen-Drilldown** die entsprechenden Dimensionen für jede Registerkarte wie folgt fest.

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

1. Legen Sie keine Filter fest und legen Sie fest, dass dieser Bericht für **Alle Website-Daten** verfügbar ist (oder ändern Sie ihn gegebenenfalls für ein bestimmtes Analytics-Konto).

1. Klicken Sie auf **Speichern**.

   ![](assets/image2015-3-22-16-3a21-3a23.png)

## RTP-Interaktionsbericht {#rtp-engagement-report}

1. Nennen Sie den Bericht &quot;**RTP-Interaktionsbericht**&quot;.

1. Setzen Sie den Namen der ersten Registerkarte auf **Alle Interaktionen**.

>[!NOTE]
>
>Sie duplizieren diese Registerkarte und erstellen weitere ähnliche - Schritt 5)

1. Wählen Sie den Berichtstyp **Explorer** aus.

   ![](assets/image2015-3-22-16-3a23-3a36.png)

1. Wählen Sie im Abschnitt Metrikgruppen die Metriken aus, die für Ihr Unternehmen relevant sind. Im Folgenden finden Sie eine Empfehlung:

   ![](assets/image2015-3-22-16-3a24-3a57.png)

1. Duplizieren Sie diese Registerkarte viermal und benennen Sie sie:

   1. **Alle Interaktionen**
   1. **Interaktion nach Branche**
   1. **Interaktion nach Gruppe**
   1. **Interaktion nach Kategorie**
   1. **Interaktion durch ABM**

   ![](assets/image2015-3-22-16-3a26-3a21.png)

1. Legen Sie im Bereich **Dimensionen-Drilldown** die entsprechenden Dimensionen für jede Registerkarte wie folgt fest:

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
   <td>Interaktion mit der Branche</td> 
   <td><img src="assets/b.png" data-linked-resource-id="7514682" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="7504218"></td> 
  </tr> 
 </tbody> 
</table>

1. Legen Sie die folgenden Filter fest:

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
   <td><p>Ereigniskategorie</p></td> 
   <td>Regulärer Ausdruck</td> 
   <td>RTP-Kampagnen|RTP-Recommendations|RTP-Segmente</td> 
   <td colspan="1">Filtert alle anderen benutzerdefinierten Ereignisse, die nicht mit RTP in Verbindung stehen</td> 
  </tr> 
  <tr> 
   <td>Ausschließen</td> 
   <td>Ereignisbezeichnung</td> 
   <td>Regulärer Ausdruck</td> 
   <td>Nr.</td> 
   <td colspan="1">Ermöglicht die Filterung aus Ihrer Berichtskampagne mithilfe des #-Zeichens im Kampagnennamen</td> 
  </tr> 
 </tbody> 
</table>

1. Legen Sie fest, dass dieser Bericht für **Alle Website-Daten** verfügbar ist (oder ändern Sie ihn gegebenenfalls).

   ![](assets/image2015-3-22-16-3a29-3a5.png)

1. Klicken Sie auf **Speichern**.

![](assets/image2015-3-22-16-3a30-3a0.png)

>[!MORELIKETHIS]
>
>[Integrieren von RTP in Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)
>
>[Benutzerdefinierte RTP-Dashboards in Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-dashboards-in-google-universal-analytics.md)
