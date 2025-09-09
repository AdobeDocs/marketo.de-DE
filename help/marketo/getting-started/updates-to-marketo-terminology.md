---
unique-page-id: 11387674
description: Aktualisierungen der Terminologie von Marketo – Marketo-Dokumente – Produktdokumentation
hide: true
hidefromtoc: true
title: Aktualisierungen der Terminologie von Marketo
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: ht
source-wordcount: '328'
ht-degree: 100%

---

# Aktualisierungen der Terminologie von Marketo {#updates-to-marketo-terminology}

Wir nehmen einige Änderungen an unserer Plattform vor, die sich auf die Bezeichnungen mancher Elemente auswirken werden. Wenn Sie seit März 2016 eine neue Marketo-Instanz haben oder Ihr Unternehmen sie nach Juli 2016 erneuert hat, wird Ihnen möglicherweise jetzt die neue Terminologie angezeigt.

Auch wenn in der Marketo-Dokumentation möglicherweise eine andere Terminologie verwendet wird, seien Sie versichert, dass alle Artikel in Kürze aktualisiert werden, um diese Änderungen widerzuspiegeln. Alle Anweisungen bleiben gleich.

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

Token mit dem Wort „Lead“ im Namen **ändern sich nicht**. Wir entschuldigen uns für jegliches Durcheinander. Wenn Sie jedoch alle Token so ändern, dass sie der neuen Terminologie entsprechen, würde dies eine ganze Reihe von Token, die derzeit in Verwendung sind, beschädigen. Darum werden weiterhin Token wie „`{{lead.First Name}}`“ angezeigt. Es gibt keine personenspezifischen Token.

>[!NOTE]
>
>Es *gibt* ein Token mit dem Namen „Person Notes“. Dieses gab es jedoch schon immer. Es wird in Ihrem CRM normalerweise für ein Beschreibungsfeld verwendet, wenn überhaupt.

## Feldverwaltung {#field-management}

Bei Feldern, die den Begriff „Lead“ enthielten, wurde dieser entweder durch „Person“ ersetzt oder ganz entfernt. Eine wichtige Ausnahme bildet jedoch das Feld „Lead-Eigentümer“. Dieses Feld heißt jetzt „Verkaufsinhaberin bzw. Verkaufsinhaber“.

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
>Eine vollständige Liste der betroffenen Feldnamen finden Sie in diesem [Support-Artikel](https://nation.marketo.com/docs/DOC-4218#jive_content_id_Field_Names_and_Tokens){target="_blank"}.

## Real-Time Personalization (RTP) ist jetzt Web-Personalisierung {#real-time-personalization-rtp-is-now-web-personalization}

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

| **[Web-Personalisierung](https://docs.marketo.com/display/DOCS/Web+Personalization+-+RTP){target="_blank"}** | Hat eine eigene Kachel auf dem Startbildschirm |
|---|---|
| **[Kontenbasiertes Web Marketing](https://docs.marketo.com/display/DOCS/Account-Based+Web+Marketing){target="_blank"}** | Zugänglich über die Kachel „Web-Personalisierung“ |
| **[Personalisiertes Retargeting](https://docs.marketo.com/display/DOCS/Website+Retargeting){target="_blank"}** | Zugänglich über die Kachel „Web-Personalisierung“ |
| **[Prädiktive Inhalte](https://docs.marketo.com/display/DOCS/Predictive+Content){target="_blank"}** | Hat eine eigene Kachel auf dem Startbildschirm |

>[!NOTE]
>
>Die auf Ihrem Startbildschirm angezeigten Kacheln spiegeln die erworbenen Module wider.

Vielen Dank für Ihre Geduld während dieses Updates.
