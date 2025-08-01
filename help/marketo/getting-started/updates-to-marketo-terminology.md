---
unique-page-id: 11387674
description: Aktualisierungen der Marketo-Terminologie - Marketo-Dokumente - Produktdokumentation
hide: true
hidefromtoc: true
title: Aktualisierungen der Terminologie von Marketo
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 2%

---

# Aktualisierungen der Terminologie von Marketo {#updates-to-marketo-terminology}

Wir nehmen einige Änderungen an unserer Plattform vor, die sich auf einige Dinge auswirken werden, die wir nennen. Wenn Sie seit März 2016 eine neue Marketo-Instanz haben oder Ihr Unternehmen nach Juli 2016 erneuert wurde, wird Ihnen die neue Terminologie möglicherweise jetzt angezeigt.

Auch wenn in der Dokumentation zu Marketo möglicherweise eine andere Terminologie verwendet wird, seien Sie versichert, dass jeder Artikel in Kürze aktualisiert wird, um diese Änderungen widerzuspiegeln. Alle Anweisungen sind gleich.

Was hat sich also geändert?

## Lead ist jetzt Person {#lead-is-now-person}

Die größte Änderung ist die Umbenennung von Lead/Leads in Person/Personen.

<table>
 <colgroup>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <td><strong>Alt</strong></td>
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

In einigen Fällen wird das Wort „Lead“ einfach entfernt.

<table>
 <colgroup>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <td><strong>Alt</strong></td>
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

Lead und Person **sind das Gleiche**.

## Token {#tokens}

Token mit dem Wort Lead in ihnen **ändern sich nicht**. Wir entschuldigen uns für jegliche Verwirrung. Wenn Sie jedoch alle Token so ändern, dass sie der neuen Terminologie entsprechen, würde dies eine ganze Reihe von Token beschädigen, die derzeit verwendet werden. So werden weiterhin Token wie &quot;`{{lead.First Name}}`&quot; angezeigt. Es gibt keine personenspezifischen Token.

>[!NOTE]
>
>Es *ein Token* dem Namen „Person Notes“, jedoch war dieses Token immer vorhanden. Sie wird in Ihrem CRM normalerweise für ein Beschreibungsfeld verwendet, falls vorhanden.

## Feldverwaltung {#field-management}

Felder, die den Begriff Lead enthalten, wurden entweder durch Person ersetzt oder das Wort Lead wurde entfernt. Eine wichtige Ausnahme bildet jedoch das Feld „Lead Owner“. Sie wird jetzt als „Sales Owner“ bezeichnet.

<table>
 <colgroup>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <td><strong>Alt</strong></td>
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
>Eine vollständige Liste der betroffenen Feldnamen finden Sie in diesem [-Artikel](https://nation.marketo.com/docs/DOC-4218#jive_content_id_Field_Names_and_Tokens){target="_blank"}.

## Real-Time Personalization (RTP) ist jetzt Web Personalization {#real-time-personalization-rtp-is-now-web-personalization}

<table>
 <colgroup>
  <col>
  <col>
 </colgroup>
 <tbody>
  <tr>
   <td><strong>Alt</strong></td>
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

| **[Web-Personalization](https://docs.marketo.com/display/DOCS/Web+Personalization+-+RTP){target="_blank"}** | Hat eine eigene Kachel auf dem Startbildschirm |
|---|---|
| **[Account-Based Web Marketing](https://docs.marketo.com/display/DOCS/Account-Based+Web+Marketing){target="_blank"}** | Zugänglich über die Kachel Web Personalization |
| **[Personalisiertes Retargeting](https://docs.marketo.com/display/DOCS/Website+Retargeting){target="_blank"}** | Zugänglich über die Kachel Web Personalization |
| **[Prädiktiver Inhalt](https://docs.marketo.com/display/DOCS/Predictive+Content){target="_blank"}** | Hat eine eigene Kachel auf dem Startbildschirm |

>[!NOTE]
>
>Die auf Ihrem Startbildschirm angezeigten Kacheln spiegeln die gekauften Module wider.

Vielen Dank für Ihre Geduld während dieses Updates.
