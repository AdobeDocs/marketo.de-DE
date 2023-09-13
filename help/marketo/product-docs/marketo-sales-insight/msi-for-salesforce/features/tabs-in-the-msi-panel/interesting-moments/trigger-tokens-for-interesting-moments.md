---
unique-page-id: 1146999
description: Trigger-Token für interessante Momente - Marketo-Dokumente - Produktdokumentation
title: Trigger-Token für interessante Momente
exl-id: 666a6eed-c432-4088-b4f1-54c996eca64c
feature: Marketo Sales Insights
source-git-commit: f0a38ddec7e42a52f31f22aa114a3f6f0c20baae
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 23%

---

# Trigger-Token für interessante Momente {#trigger-tokens-for-interesting-moments}

>[!PREREQUISITES]
>
>Erfahren Sie, wie Sie die [Interessanter Moment Flow-Schritt](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md).

## Verfügbare Token {#available-tokens}

Checkout [Token-Übersicht](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) um alle Token zu sehen, die Sie in einen interessanten Moment setzen können.

## Trigger-Token {#trigger-tokens}

Basierend auf dem in einer Smart-Kampagne verwendeten Trigger werden zusätzliche Trigger-Token bereitgestellt.

* `{{trigger.Trigger Name}}` ist immer der eigentliche Trigger selbst. Beispiel: Klicks auf Link in E-Mail.
* `{{trigger.Name}}` ist der Name des Assets, das die Kampagne ausgelöst hat. Beispiel: Klicks Link auf der Webseite ist die URL selbst, Betreff für Salesforce-Trigger usw.
* Zusätzliche Trigger sind basierend auf Einschränkungen verfügbar, die unten aufgeführt sind.

### Email Trigger {#email-triggers}

<table style="table-layout:auto"> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col>
  <col>
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th><br></th> 
   <th><code>{{trigger.Trigger Name}}</code></th> 
   <th><code>{{trigger.Name}}</code></th> 
   <th><code>{{trigger.Link}}</code></th> 
   <th><code>{{trigger.Subject}}</code></th> 
   <th><code>{{trigger.Category}}</code></th> 
   <th><code>{{trigger.Details}}</code></th> 
   <th><code>{{trigger.Web Page}}</code></th> 
   <th><code>{{trigger.Client IP Address}}</code></th> 
   <th><code>{{trigger.Sent By}}</code></th> 
   <th><code>{{trigger.Received By}}</code></th> 
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr> 
  <tr> 
   <td>Link in E-Mail angeklickt</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Hard-E-Mail-Bounces</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>E-Mail nicht zugestellt (Soft Bounce)</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>E-Mail wird bereitgestellt</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Öffnet E-Mail</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>Weiterleitung an E-Mail-Adresse eines Freundes wurde empfangen</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>Weiterleitung an E-Mail-Adresse eines Freundes wurde gesendet</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td>
  </tr> 
  <tr> 
   <td>Bestellt E-Mail ab</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

### Salesforce-Trigger {#salesforce-triggers}

<table style="table-layout:auto"> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col>
  <col>
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th><br></th> 
   <th><code>{{trigger.Trigger Name}}</code></th> 
   <th><code>{{trigger.Name}}</code></th> 
   <th><code>{{trigger.Link}}</code></th> 
   <th><code>{{trigger.Subject}}</code></th> 
   <th><code>{{trigger.Category}}</code></th> 
   <th><code>{{trigger.Details}}</code></th> 
   <th><code>{{trigger.Web Page}}</code></th> 
   <th><code>{{trigger.Client IP Address}}</code></th> 
   <th><code>{{trigger.Sent By}}</code></th> 
   <th><code>{{trigger.Received By}}</code></th> 
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr> 
  <tr> 
   <td>Link in Verkaufs-E-Mail angeklickt</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Ist gesendete Verkaufs-E-Mail</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Öffnet Verkaufs-E-Mail</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Verkaufs-E-Mail wird aufgrund eines Bounce-Ereignisses nicht zugestellt</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Verkaufs-E-Mail wird empfangen</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>Opportunity wird aktualisiert</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>Eigentümer wird geändert</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Person ist konvertiert</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Person wird aus SFDC gelöscht</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Person wird mit SFDC synchronisiert</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Aus Opportunity entfernt</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Aus SFDC-Kampagne entfernt</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Aktivität wird protokolliert</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Aktivität wird aktualisiert</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Zu Opportunity hinzugefügt</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Zu SFDC-Kampagne hinzugefügt</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Status wird in SFDC-Kampagne geändert</td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

### Sales Connect-Trigger {#sales-connect-triggers}

<table style="table-layout:auto"> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col>
  <col>
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th><br></th> 
   <th><code>{{trigger.Trigger Name}}</code></th> 
   <th><code>{{trigger.Name}}</code></th> 
   <th><code>{{trigger.Link}}</code></th> 
   <th><code>{{trigger.Subject}}</code></th> 
   <th><code>{{trigger.Category}}</code></th> 
   <th><code>{{trigger.Details}}</code></th> 
   <th><code>{{trigger.Web Page}}</code></th> 
   <th><code>{{trigger.Client IP Address}}</code></th> 
   <th><code>{{trigger.Sent By}}</code></th> 
   <th><code>{{trigger.Received By}}</code></th> 
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr> 
  <tr> 
   <td>Link in Verkaufs-E-Mail angeklickt</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Ist gesendete Verkaufs-E-Mail</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Öffnet Verkaufs-E-Mail</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Verkaufs-E-Mail wird aufgrund eines Bounce-Ereignisses nicht zugestellt</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Verkaufs-E-Mail wird empfangen</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Ist zur Verkaufskampagne hinzugefügt</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr>
   <td>Eigentümer wird geändert</td> 
   <td>Ist aus Verkaufskampagne entfernt</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Hat Verkaufsanruf empfangen</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

### Dynamic Chat Trigger-Token {#dynamic-chat-trigger-tokens}

<table>
<thead>
  <tr>
    <th> </th>
    <th><code>{{trigger.Agent Email}}</code></th>
    <th><code>{{trigger.Agent Name}}</code></th>
    <th><code>{{trigger.Conversation Status}}</code></th>
    <th><code>{{trigger.Conversation Summary}}</code></th>
    <th><code>{{trigger.Conversation Transcript}}</code></th>
    <th><code>{{trigger.Document Downloaded}}</code></th>
    <th><code>{{trigger.Document Name}}</code></th>
    <th><code>{{trigger.Document Opened}}</code></th>
    <th><code>{{trigger.Document URL}}</code></th>
    <th><code>{{trigger.Goal name}}</code></th>
    <th><code>{{trigger.meeting status}}</code></th>
    <th><code>{{trigger.Name}}</code></th>
    <th><code>{{trigger.Page URL}}</code></th>
    <th><code>{{trigger.routing queue name}}</code></th>
    <th><code>{{trigger.Scheduled For}}</code></th>
    <th><code>{{trigger.source name}}</code></th>
    <th><code>{{trigger.source type}}</code></th>
    <th><code>{{trigger.Trigger Name}}</code></th>
    <th><code>{{trigger.ui type}}</code></th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Mit einem Dialogfeld interagieren</td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Mit einem Konversationsformular interagieren</td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
  </tr>
  <tr>
    <td>Interagiert mit einem Agenten im Dialogfeld</td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Kontakt mit einem Agenten im Konversationsformular</td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Geplantes Meeting im Dialogfeld</td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Geplantes Treffen in Form von Gesprächen</td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Dialogfeld-Ziel erreicht</td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Erreichtes Konversationsformziel</td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Interagiert mit Dokument im Dialogfeld</td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr>
    <td>Interagiert mit Dokument im Konversationsformular</td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td><img src="assets/check.png" alt="check"></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
</tbody>
</table>

### Verschiedenes {#miscellaneous}

<table style="table-layout:auto"> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col>
  <col>
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th><br></th> 
   <th><code>{{trigger.Trigger Name}}</code></th> 
   <th><code>{{trigger.Name}}</code></th> 
   <th><code>{{trigger.Link}}</code></th> 
   <th><code>{{trigger.Subject}}</code></th> 
   <th><code>{{trigger.Category}}</code></th> 
   <th><code>{{trigger.Details}}</code></th> 
   <th><code>{{trigger.Web Page}}</code></th> 
   <th><code>{{trigger.Client IP Address}}</code></th> 
   <th><code>{{trigger.Sent By}}</code></th> 
   <th><code>{{trigger.Received By}}</code></th> 
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr> 
  <tr> 
   <td>Füllt Formular aus</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Besucht Webseite</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Klickt Link auf Webseite an</td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="check"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Wenn keine Prüfung vorhanden ist ![(Häkchen)](assets/check.png) dann würde es eine leere Zeichenfolge (nichts) im interessanten Moment zurückgeben.

&#42;Der Trigger **Besuche-Webseite** verfügt über einige zusätzliche Token:

* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!TIP]
>
>Testen Sie immer Ihre interessanten Momente, um sicherzustellen, dass sie wie gewünscht rendern.
>
>Stellen Sie außerdem sicher, dass es für den Vertriebsmitarbeiter interessant ist, nicht nur für Sie!
