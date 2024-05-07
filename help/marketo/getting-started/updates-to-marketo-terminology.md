---
unique-page-id: 11387674
description: Aktualisierungen der Marketo-Terminologie - Marketo-Dokumente - Produktdokumentation
hide: true
hidefromtoc: true
title: Aktualisierungen der Marketo-Terminologie
source-git-commit: 14583b7fa148aa2b03c8cf6316b9a106c11717b7
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 2%

---

# Aktualisierungen der Marketo-Terminologie {#updates-to-marketo-terminology}

Wir nehmen einige Änderungen an unserer Plattform vor, die sich auf das auswirken werden, was einige Dinge heißen. Wenn Sie seit März 2016 eine neue Marketo-Instanz haben oder Ihr Unternehmen nach Juli 2016 erneuert wurde, wird Ihnen die neue Terminologie möglicherweise jetzt angezeigt.

Auch wenn Sie in der Marketo-Dokumentation möglicherweise unterschiedliche Terminologie sehen, können Sie sicher sein, dass alle Artikel bald aktualisiert werden, um diese Änderungen widerzuspiegeln. Alle Anweisungen sind identisch.

Was hat sich also geändert?

## Lead ist jetzt Person {#lead-is-now-person}

Die größte Änderung ist die Umbenennung von Lead/Leads zu Person/Personen.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Old</strong></td> 
   <td><strong>Neu</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img width="295" src="assets/leads.png" data-linked-resource-id="11387678" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <img width="295" src="assets/people.png" data-linked-resource-id="11387679" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

In einigen Fällen wird das Wort &quot;Lead&quot;einfach entfernt.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Old</strong></td> 
   <td><strong>Neu</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img src="assets/lead-database.png" data-linked-resource-id="11387676" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <p><img src="assets/database.png" data-linked-resource-id="11387677" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"></p> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

Lead und Person **das gleiche**.

## Token {#tokens}

Token mit dem Wort &quot;Lead&quot; **sich nicht ändern**. Wir entschuldigen uns für jede Verwirrung. Eine Änderung aller Token an die neue Terminologie würde jedoch viele der derzeit verwendeten Token beschädigen. Daher werden weiterhin Token wie &quot;`{{lead.First Name}}`.&quot; Es gibt keine personenspezifischen Token.

>[!NOTE]
>
>Dort *is* Ein Token namens &quot;Personnotes&quot;, aber dieses Token war immer vorhanden. Sie wird normalerweise für ein Beschreibungsfeld in Ihrem CRM-System verwendet, wenn überhaupt.

## Feldverwaltung {#field-management}

Felder, die den Begriff &quot;Lead&quot;enthielten, wurden entweder durch &quot;Person&quot;ersetzt oder das Wort &quot;Lead&quot;wurde entfernt. Eine wichtige Ausnahme bildet jedoch das Feld &quot;Lead Owner&quot;. Es wird jetzt als &quot;Vertriebsmitarbeiter&quot;bezeichnet.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Old</strong></td> 
   <td><strong>Neu</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img src="assets/lead-owner.png" data-linked-resource-id="11387757" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <img src="assets/sales-owner.png" data-linked-resource-id="11387758" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Eine vollständige Liste der betroffenen Feldnamen finden Sie in diesem [Support-Artikel](https://nation.marketo.com/docs/DOC-4218#jive_content_id_Field_Names_and_Tokens){target="_blank"}.

## Echtzeit-Personalisierung (RTP) ist jetzt Web-Personalisierung {#real-time-personalization-rtp-is-now-web-personalization}

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td><strong>Old</strong></td> 
   <td><strong>Neu</strong></td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <img src="assets/rtp.png" data-linked-resource-id="11387692" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
   <td> 
    <div> 
     <img src="assets/web.png" data-linked-resource-id="11387693" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="11387674"> 
    </div></td> 
  </tr> 
 </tbody> 
</table>

Zusätzlich zur Namensänderung besteht sie jetzt aus vier separaten Apps:

| **[Web-Personalisierung](https://docs.marketo.com/display/DOCS/Web+Personalization+-+RTP){target="_blank"}** | Hat eine eigene Kachel auf dem Startbildschirm |
|---|---|
| **[Kontobasiertes Webmarketing](https://docs.marketo.com/display/DOCS/Account-Based+Web+Marketing){target="_blank"}** | Zugriff über die Kachel Web-Personalisierung |
| **[Personalisiertes Retargeting](https://docs.marketo.com/display/DOCS/Website+Retargeting){target="_blank"}** | Zugriff über die Kachel Web-Personalisierung |
| **[Prädiktive Inhalte](https://docs.marketo.com/display/DOCS/Predictive+Content){target="_blank"}** | Hat eine eigene Kachel auf dem Startbildschirm |

>[!NOTE]
>
>Die auf Ihrem Startbildschirm sichtbaren Kacheln spiegeln die gekauften Module wider.

Vielen Dank für Ihre Geduld während dieser Aktualisierung.
