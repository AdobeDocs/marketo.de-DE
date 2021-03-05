---
unique-page-id: 1146999
description: Tokens für interessante Momente - Marketing Docs - Produktdokumentation
title: Tokens für interessante Momente
translation-type: tm+mt
source-git-commit: 1649aae540204bb5de205e3f5b75ec7e968a7da4
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---


# Tokens für interessante Momente {#tokens-for-interesting-moments}

>[!PREREQUISITES]
>
>Hier erfahren Sie, wie Sie den Schritt [Interessanter Moment-Fluss](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md) verwenden.

## Verfügbare Tokens {#available-tokens}

Sehen Sie sich [Tokens Overview](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) an, um alle Token zu sehen, die Sie in einen interessanten Moment setzen können.

## Trigger-Tokens {#trigger-tokens}

Je nach Trigger, der in einer intelligenten Kampagne verwendet wird, stehen zusätzliche Trigger-Token zur Verfügung.

* `{{trigger.Trigger Name}}` was immer der eigentliche Trigger ist. Beispiel: Klicken Sie in der E-Mail auf Link.
* `{{trigger.Name}}` der Name des Assets, das die Kampagne ausgelöst hat. Beispiel: Klicks Link auf der Webseite ist die URL selbst, Betreff für Salesforce Trigger, etc.
* Weitere Trigger stehen aufgrund von Einschränkungen zur Verfügung, die nachfolgend aufgeführt sind.

**E-Mail-Trigger**

<table> 
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
   <td>Klicks Link in E-Mail</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
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
   <td>E-Mail-Absprünge hart</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
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
   <td>E-Mail-Absprünge weich</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
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
   <td>E-Mail wird gesendet</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
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
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
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
   <td>An Freunde weitergeleitete E-Mail erhalten</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
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
   <td>An Freunde weiterleiten</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td>
  </tr> 
  <tr> 
   <td>Abonnements von E-Mail abmelden</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

**Salesforce-Trigger**

<table> 
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
   <td>Klicks Link in Verkaufs-E-Mail</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Wird E-Mail zum Vertrieb gesendet</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Öffnet Verkaufs-E-Mail</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>E-Mail-Absprünge im Vertrieb</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
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
   <td>E-Mail zum Verkauf wird empfangen</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>Chancen werden aktualisiert</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
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
   <td>Änderungen am Inhaber</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
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
   <td>Person wird konvertiert</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
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
   <td>Person wird aus dem SFDC gelöscht</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
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
   <td>Person wird mit dem SFDC synchronisiert</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
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
   <td>Aus Gelegenheit entfernt</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
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
   <td>Aus der SFDC-Kampagne entfernt</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
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
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
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
   <td>Aktivität wurde aktualisiert</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
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
   <td>Zu Chancen hinzugefügt</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
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
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
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
   <td>Status in der SFDC-Kampagne geändert</td> 
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

**Sales Connect-Trigger**

<table> 
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
   <td>Klicks Link in Verkaufs-E-Mail</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Wird E-Mail zum Vertrieb gesendet</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Öffnet Verkaufs-E-Mail</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>E-Mail-Absprünge im Vertrieb</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
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
   <td>E-Mail zum Verkauf wird empfangen</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Wird zur Kampagne Vertrieb hinzugefügt</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
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
   <td>Änderungen am Inhaber</td> 
   <td>wird aus der Kampagne Vertrieb entfernt</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
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
   <td>Kaufaufruf erhalten</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
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

**Sonstiges**

<table> 
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
   <td>Ausfüllen des Formulars</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Besuche der Webseite</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Klicks Link auf Webseite</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Wenn es keinen Häkchen hat ![(tick)](assets/check.svg) würde es eine leere Zeichenfolge (nichts) im interessanten Moment zurückgeben.

*Der Trigger **Webseite &quot;Besuche&quot;** verfügt über einige zusätzliche Token:

* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!TIP]
>
>Testen Sie immer Ihre interessanten Momente, um sicherzustellen, dass sie die von Ihnen gewünschte Art darstellen.
>
>Vergewissern Sie sich auch, dass es für den Verkäufer interessant ist, nicht nur für Sie. ![(wink)](assets/wink.svg)>
