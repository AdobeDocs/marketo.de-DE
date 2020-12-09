---
unique-page-id: 1146999
description: Tokens für interessante Momente - Marketing Docs - Produktdokumentation
title: Tokens für interessante Momente
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# Tokens für interessante Momente {#tokens-for-interesting-moments}

>[!PREREQUISITES]
>
>* Erfahren Sie, wie Sie den Schritt [zum Fluss des](../../../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md)interessanten Moments verwenden.
>* Erfahren Sie mehr über [Token](http://docs.marketo.com/display/docs/tokens).

>



## Verfügbare Tokens {#available-tokens}

Sehen Sie sich die [Tokens Übersicht](../../../../../../product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) an, um alle Token zu sehen, die Sie in einen interessanten Moment setzen können.

## Auslöser-Tokens {#trigger-tokens}

Je nach Auslöser, der in einer intelligenten Kampagne verwendet wird, stehen zusätzliche Auslösertoken zur Verfügung.

* `{{trigger.Trigger Name}}` was immer der eigentliche Auslöser ist. Beispiel: Klicken Sie in der E-Mail auf Link.
* `{{trigger.Name}}` der Name des Assets, das die Kampagne ausgelöst hat. Beispiel: Klicks Link auf der Webseite ist die URL selbst, Betreff für Salesforce-Auslöser, etc.
* Weitere Auslöser stehen aufgrund von Einschränkungen zur Verfügung, die im Folgenden aufgeführt sind:

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
  </tr> 
  <tr> 
   <td>Abonnements von E-Mail abmelden</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><br></td> 
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
   <td><br></td> 
  </tr> 
  <tr> 
   <td>E-Mail zum Vertrieb</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>Öffnet Verkaufs-E-Mail</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>E-Mail zum Vertrieb erhalten</td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(Zecken)"></td> 
  </tr> 
  <tr> 
   <td colspan="1">E-Mail-Absprung des Verkaufs</td> 
   <td colspan="1"><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td colspan="1"><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
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
   <td><p><br></p></td> 
  </tr> 
  <tr> 
   <td colspan="1">Webseite für Besuche*</td> 
   <td colspan="1"><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><img src="assets/check.svg" alt="(Zecken)"></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Wenn es keinen Häkchen ![(Häkchen)](assets/check.svg) hat, wird eine leere Zeichenfolge (nichts) im interessanten Moment zurückgegeben.

*Die Webseite **&quot;** Auslöser-Besuche&quot;enthält einige zusätzliche Token:

* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!TIP]
>
>Testen Sie immer Ihre interessanten Momente, um sicherzustellen, dass sie die von Ihnen gewünschte Art darstellen.
>
>Vergewissern Sie sich auch, dass es für den Verkäufer interessant ist, nicht nur für Sie. ![(wink)](assets/wink.svg)>

