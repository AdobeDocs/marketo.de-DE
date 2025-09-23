---
unique-page-id: 7504218
description: Benutzerdefinierte RTP-Berichte in Google Universal Analytics - Marketo-Dokumente - Produktdokumentation
title: Benutzerdefinierte RTP-Berichte in Google Universal Analytics
exl-id: c8b1e653-03b8-48bc-b80d-3e6cdf3485c3
feature: Web Personalization
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 8%

---

# Benutzerdefinierte RTP-Berichte in Google Universal Analytics {#custom-rtp-reports-in-google-universal-analytics}

>[!PREREQUISITES]
>
>[Integrieren von RTP mit Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)

In diesem Artikel wird erläutert, wie Sie benutzerdefinierte RTP-Berichte für Google Universal Analytics (GUA) einrichten.  Die Daten, die von RTP an GUA gesendet werden, können als zwei separate benutzerdefinierte Berichte eingerichtet werden:

* RTP B2B
* RTP-Interaktion

## Einrichten eines [!UICONTROL benutzerdefinierten Berichts] {#setting-up-a-custom-report}

1. Melden Sie sich bei Google Analytics an.

1. Klicken Sie **[!UICONTROL oberen Menü auf]** Anpassung“.

1. Klicken Sie **[!UICONTROL Neuer benutzerdefinierter Bericht]**.

![](assets/image2015-3-22-16-3a10-3a48.png)

## RTP B2B-Bericht {#rtp-b-b-report}

1. Benennen Sie den Bericht **RTP B2B-**.

1. Benennen Sie die erste Registerkarte **[!UICONTROL Industry]**.

>[!NOTE]
>
>Sie werden **diese Registerkarte duplizieren** und zusätzliche ähnliche erstellen - Schritt 5)

1. Wählen Sie **[!UICONTROL Berichtstyp]** Explorer“.

   ![](assets/image2015-3-22-16-3a15-3a25.png)

1. Wählen Sie **[!UICONTROL Abschnitt]** die Metriken aus, die für Ihr Unternehmen relevant sind.

   a. Wir empfehlen Folgendes:

   ![](assets/image2015-3-22-16-3a16-3a40.png)

1. Duplizieren Sie diese Registerkarte 4-mal und benennen Sie sie:

   1. **Branche**
   1. **Gruppe**
   1. **Kategorie**
   1. **ABM**
   1. **Organisationen**

   ![](assets/image2015-3-22-16-3a17-3a41.png)

1. Legen Sie im Abschnitt **Dimension-Drill** Downs die relevanten Dimensionen für jede Registerkarte wie folgt fest.

<table>
 <thead>
  <tr>
   <th>
    <div>
      Name der Registerkarte
    </div></th>
   <th>
    <div>
      Dimension-Drill-down
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

1. Legen Sie keine Filter fest und legen Sie fest, dass dieser Bericht für &quot;**[!UICONTROL Website-Daten“ verfügbar]** (oder ändern Sie ihn, falls für ein bestimmtes Analytics-Konto relevant).

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2015-3-22-16-3a21-3a23.png)

## RTP-Interaktionsbericht {#rtp-engagement-report}

1. Benennen Sie den Bericht **RTP-Interaktionsbericht**.

1. Legen Sie den Namen der ersten Registerkarte auf &quot;**[!UICONTROL Interaktion“]**.

>[!NOTE]
>
>Sie duplizieren diese Registerkarte und erstellen weitere ähnliche Registerkarten - Schritt 5)

1. Wählen Sie **[!UICONTROL Berichtstyp]** Explorer“.

   ![](assets/image2015-3-22-16-3a23-3a36.png)

1. Wählen Sie [!UICONTROL  Abschnitt ] die Metriken aus, die für Ihr Unternehmen relevant sind. Im Folgenden finden Sie eine Empfehlung:

   ![](assets/image2015-3-22-16-3a24-3a57.png)

1. Duplizieren Sie diese Registerkarte 4-mal und benennen Sie sie:

   1. **Alle Interaktionen**
   1. **Interaktion der Branche**
   1. **Interaktion nach Gruppe**
   1. **Interaktion nach Kategorie**
   1. **Engagement von ABM**

   ![](assets/image2015-3-22-16-3a26-3a21.png)

1. Legen Sie im Abschnitt **Dimension-Drill** Downs die relevanten Dimensionen für jede Registerkarte wie folgt fest:

<table>
 <thead>
  <tr>
   <th>
    <div>
      Name der Registerkarte
    </div></th>
   <th>
    <div>
      Dimension-Drill-down
    </div></th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td>Gesamte Interaktion</td>
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
   <td>Engagement der Industrie</td>
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
      erh/exc
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
   <td><p><span class="uicontrol">Ereigniskategorie</span></p></td>
   <td>Regex</td>
   <td>RTP-Kampagnen|RTP-Recommendations|RTP-Segmente</td>
   <td colspan="1">Filtert alle anderen benutzerspezifischen Ereignisse, die nicht mit RTP in Verbindung stehen.</td>
  </tr>
  <tr>
   <td>Ausschließen</td>
   <td><span class="uicontrol">Ereignistitel</span></td>
   <td>Regex</td>
   <td>#</td>
   <td colspan="1">Ermöglicht das Filtern von Kampagnenberichten mithilfe der Ziffer # im Kampagnennamen</td>
  </tr>
 </tbody>
</table>

1. Legen Sie fest, dass dieser Bericht für &quot;**[!UICONTROL Website-Daten“ verfügbar]** (oder ändern Sie ihn bei Bedarf).

   ![](assets/image2015-3-22-16-3a29-3a5.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

![](assets/image2015-3-22-16-3a30-3a0.png)

>[!MORELIKETHIS]
>
>[Integrieren von RTP mit Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/integrate-rtp-with-google-universal-analytics.md)
>
>[Benutzerdefinierte RTP-Dashboards in Google Universal Analytics](/help/marketo/product-docs/web-personalization/reporting-for-web-personalization/web-analytics-integrations/custom-rtp-dashboards-in-google-universal-analytics.md)
