---
description: Online Advertising Marketo Landingpage-Programmvorlage. Verwenden Sie ihn für Paid-Kampagnen mit Marketo-Seiten.
title: 'Marketo-Landingpage mit Online-Werbung: OA-JJJJ-MM'
feature: Programs
exl-id: f7f17792-cc16-4a99-8683-68796770e42c
TQID: https://experienceleague.adobe.com/B1msn3wZ33NB3YzSKz82xTFuq-JPdjZ3nMvJTQZm1mY
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2:
  - id: ea6641cb-8461-4151-a8a9-9faaa44a928a
topic_v2:
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 508
ht-degree: 15%

---

# Marketo-Landingpage mit Online-Werbung: OA-JJJJ-MM {#oa-yyyy-mm-online-advertising-marketo-landing-page}

Dies ist ein Beispiel für ein Tracking-Programm für Online-Werbung, einschließlich einer Marketo-Landingpage mit Registrierungsformular und Verwendung eines Marketo-Standardprogramms. Der Link zum Angebot kann auf der Dankeseite angezeigt, in einer Dankesnachricht gesendet oder auf beiden Seiten angezeigt werden.

Wenden Sie sich an das Adobe-Accountteam oder besuchen Sie die Seite [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"}, um weitere Unterstützung bei der Strategie oder bei der Anpassung eines Programms zu erhalten.

## Kanal-Zusammenfassung {#channel-summary}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Kanal</th>
   <th>Mitgliedschaftsstatus</th>
   <th>Analytics Behavior</th>
   <th>Programmtyp</th>
  </tr>
  <tr>
   <td>Online-Werbung</td>
   <td>01 - Mitglied
<br/>02 - Interagiert - Erfolg</td>
   <td>Einschließlich</td>
   <td>Standard</td>
  </tr>
 </tbody>
</table>

## Programm enthält die folgenden Assets {#program-contains-the-following-assets}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Typ</th>
   <th>Vorlagenname</th>
   <th>Asset-Name</th>
  </tr>
  <tr>
   <td>Formular</td>
   <td> </td>
   <td>FM-Content-Registrierung</td>
  </tr>
  <tr>
   <td>E-Mail</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">E-Mail-Vorlage für Schnellstart</a></td>
   <td>01-email-thank you</td>
  </tr>
  <tr>
   <td>Landingpage</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">Schnellstart-LP-Vorlage</a></td>
   <td>01 - LP - Registrierung</td>
  </tr>
   <tr>
   <td>Landingpage</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-landing-page-template.md" target="_blank">Schnellstart-LP-Vorlage</a></td>
   <td>02 - LP - Danke</td>
  </tr>
   <tr>
   <td>Lokaler Bericht</td>
   <td> </td>
   <td>E-Mail-Leistung</td>
  </tr>
  <tr>
   <td>Lokaler Bericht</td>
   <td> </td>
   <td>Landing Page-Leistung</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>00 - Erfassungsprogramm</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>01 - Ausgefülltes Formular</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>02 - Interagiert (Programm erfolgreich)</td>
  </tr>
  <tr>
   <td>Ordner</td>
   <td> </td>
   <td>Assets - enthält alle Kreativ-Assets
<br/>(Unterordner für E-Mails und Landingpages)  </td>
  </tr>
  <tr>
   <td>Ordner</td>
   <td> </td>
   <td>Kampagnen - enthält alle intelligenten Kampagnen</td>
  </tr>
  <tr>
   <td>Ordner</td>
   <td> </td>
   <td>Berichte</td>
  </tr>
 </tbody>
</table>

![](assets/oa-yyyy-mm-online-advertising-marketo-landing-page-1.png)

## Meine Token enthalten {#my-tokens-included}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Token-Typ</th>
   <th>Token-Name</th>
   <th>Wert</th>
  </tr>
  <tr>
   <td>RTF</td>
   <td><code>{{my.Content-Description}}</code></td>
   <td>Für Details doppelklicken
<br/><code><--My Content Description Here--></code>
<br/>Bearbeiten Sie diese Inhaltsbeschreibung auf Programmebene auf der Registerkarte Meine Token .
<br/>Sie werden lernen:
<li>Aufzählungszeichen 1</li>
<li>Aufzählungszeichen 2</li>
<li>Aufzählungszeichen 3</li></td>
  </tr>
  <tr>
   <td>Text</td>
   <td><code>{{my.Content-Title}}</code></td>
   <td><code><--My Content Title Here--></code></td>
  </tr>
  <tr>
   <td>Text</td>
   <td><code>{{my.Content-Type}}</code></td>
   <td><code><--My Content Type Here--></code></td>
  </tr>
  <tr>
   <td>Text</td>
   <td><code>{{my.Content-URL}}</code></td>
   <td>my.ContentURL?without=http://</td>
  </tr>
  <tr>
   <td>Text</td>
   <td><code>{{my.Email-FromAddress}}</code></td>
   <td>PlaceholderFrom.email@mydomain.com</td>
  </tr>
  <tr>
   <td>Text</td>
   <td><code>{{my.Email-FromName}}</code></td>
   <td><code><--My From Name Here--></code></td>
  </tr>
  <tr>
   <td>Text</td>
   <td><code>{{my.Email-ReplyToAddress}}</code></td>
   <td>reply-to.email@mydomain.com</td>
  </tr>
  <tr>
   <td>Text</td>
   <td><code>{{my.PageURL-ThankYou}}</code></td>
   <td>My.DankePageURL?ohne die http://</td>
  </tr>
 </tbody>
</table>

SCREENSHOT DES PROGRAMMS

## Kollisionsregeln {#conflict-rules}

* **Programm-Tags**
   * Tags in diesem Abonnement erstellen - _Empfohlen_
   * Ignorieren

* **Landingpage-Vorlage mit demselben Namen**
   * Originalvorlage kopieren
   * Zielvorlage verwenden - _Empfohlen_

* **Bilder mit demselben Namen**
   * Beide Dateien beibehalten
   * Element in diesem Abonnement ersetzen - _Empfohlen_

* **E-Mail-Vorlagen mit demselben Namen**
   * Beide Vorlagen beibehalten
   * Vorhandene Vorlage ersetzen - _Empfohlen_

SCREENSHOT DER KONFLIKTREGELN

## Bewährte Methoden {#best-practices}

* Verschieben Sie das Formular nach dem Import des Inhaltsprogramms von einem lokalen Asset in ein globales Asset, das sich in Design Studio befindet.
   * Das Verringern der Anzahl von Formularen und die Verwendung von mehr globalen Assets aus dem Design Studio ermöglicht mehr Skalierbarkeit in Ihrem Programmdesign und der administrativen Governance. Außerdem bietet es Flexibilität bei regelmäßigen Compliance-Aktualisierungen für Felder, Opt-in-Sprache usw.

* Erwägen Sie, die Vorlagen in Ihrem importierten Programm zu aktualisieren, um die aktuellen Markenvorlagen zu verwenden, oder aktualisieren Sie die neu importierte Vorlage, um Ihre Marke widerzuspiegeln, indem Sie einen Ausschnitt oder Ihre entsprechenden Logo-/Fußzeileninformationen hinzufügen.

* Verwenden Sie Programm-Tags, um Berichte nach Ihren verschiedenen Quellen von Online Advertising zu filtern.

* Erwägen Sie, die Namenskonvention dieses Programmbeispiels zu aktualisieren, um sie an Ihre Namenskonvention anzupassen.

>[!NOTE]
>
>Denken Sie daran, die Werte für Mein Token in der Programmvorlage und jedes Mal, wenn Sie das Programm verwenden, nach Bedarf zu aktualisieren.

>[!TIP]
>
>Aktivieren Sie die Kampagne „02 - Interagiert (Programmerfolg)“, um den Erfolg zu verfolgen, bevor Ihr Formular live ist und E-Mails gesendet werden.

>[!IMPORTANT]
>
>Meine Token, die auf eine URL verweisen, dürfen die URL http:// oder https:// nicht enthalten. Andernfalls funktioniert der Link innerhalb des Assets nicht ordnungsgemäß.
