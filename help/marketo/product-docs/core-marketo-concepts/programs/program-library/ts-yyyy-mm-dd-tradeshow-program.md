---
description: Messe-Programmvorlage. Verwenden Sie ihn für Veranstaltungen und Messen mit konsistenter Benennung.
title: 'Messeprogramm: TS-EV-JJJJ-MM-TT'
feature: Programs
exl-id: 39ef8d6e-392b-456e-a925-b1f6c2cb81d8
TQID: https://experienceleague.adobe.com/RRYrVLXxJpc3XM-KyoQgLMP-LNwstkjavPomdOXVo5s
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: b0bb9048-d951-48d8-8232-45cf248a7e27id: d65b4a73-87a3-4d56-b638-74e74d9939ceid: e64968b2-4ee5-47f9-8cae-0588f184b9ebid: f82558ea-6af5-44eb-a424-5b3389abb0a3
subfeature_v2: id: ea6641cb-8461-4151-a8a9-9faaa44a928a
topic_v2: id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 440
ht-degree: 18%

---

# Messeprogramm: TS-EV-JJJJ-MM-TT {#ts-yyyy-mm-dd-tradeshow-program}

Dies ist ein Beispiel für ein Messeprogramm mit Einladungen und Follow-up-E-Mails unter Verwendung eines Marketo Engage-Veranstaltungsprogramms.

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
   <td>Ereignis</td>
   <td>01-Invited
   <br/>02-waitlisted
   <br/>03-registriert
   <br/>04-Besuchter Stand
   <br/>05-Engaged auf der Messe - Erfolg
   <br/>06-Engaged auf der Post Show - Erfolg</td>
   <td>Einschließlich</td>
   <td>Ereignis</td>
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
   <td>E-Mail</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">E-Mail-Vorlage für Schnellstart</a></td>
   <td>01-email-thank you</td>
  </tr>
   <tr>
   <td>E-Mail</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">E-Mail-Vorlage für Schnellstart</a></td>
   <td>02a- E-Mail - Einladung</td>
  </tr>
  <tr>
  <tr>
   <td>Lokaler Bericht</td>
   <td> </td>
   <td>E-Mail-Leistung</td>
  </tr>
  <tr>
   <td>Lokaler Bericht</td>
   <td> </td>
   <td>Programmleistung</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>00 - Erfassungsprogramm</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>01 - Einladung senden</td>
  </tr>
   <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>02 - Senden von Folge-E-Mails</td>
  </tr>
   <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>03 - Interagiert mit Follow-up-E-Mail (Erfolg)</td>
  </tr>
  <tr>
   <td>Ordner</td>
   <td> </td>
   <td>Assets - enthält alle Kreativ-Assets
<br/>(Unterordner für E-Mail und Landingpages)</td>
  </tr>
  <tr>
   <td>Ordner</td>
   <td> </td>
   <td>Kampagnen - Alle intelligenten Kampagnen werden gespeichert</td>
  </tr>
  <tr>
   <td>Ordner</td>
   <td> </td>
   <td>Berichte</td>
  </tr>
 </tbody>
</table>

![](assets/ts-yyyy-mm-dd-tradeshow-program-1.png)

## Meine Token enthalten {#my-tokens-included}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Token-Typ</th>
   <th>Token-Name</th>
   <th>Wert</th>
  </tr>
  <tr>
   <td>Kalenderdatei</td>
   <td><code>{{my.AddToCalendar}}</code></td>
   <td>Für Details doppelklicken</td>
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
   <td><code>{{my.Event-Date}}</code></td>
   <td><code><--My Event Date--></code></td>
  </tr>
   <tr>
   <td>RTF</td>
   <td><code>{{my.Event-Booth#}}</code></td>
   <td><code><--My Booth Number--></code></td>
  </tr>
   <tr>
   <td>Text</td>
   <td><code>{{my.Event-City}}</code></td>
   <td><code><--My Event City Here--></code></td>
  </tr>
  <tr>
   <td>Text</td>
   <td><code>{{my.Event-Date}}</code></td>
   <td><code><--My Event Date--></code></td>
  </tr>
  <tr>
   <td>Text</td>
   <td><code>{{my.Event-Time}}</code></td>
   <td><code><--My Event Time + TimeZone--></code></td>
  </tr>
  <tr>
   <td>Text</td>
   <td><code>{{my.Event-Title}}</code></td>
   <td><code><--My Event Title Here--></code></td>
  </tr>
  <tr>
   <td>Text</td>
   <td><code>{{my.Event-Type}}</code></td>
   <td>Fachmesse</td>
  </tr>
 </tbody>
</table>

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

## Bewährte Methoden {#best-practices}

* Verschieben Sie das Formular nach dem Import des Webinar-Programms von einem lokalen Asset in ein globales Asset im Design Studio.
   * Das Verringern der Anzahl von Formularen und die Verwendung von mehr globalen Assets aus dem Design Studio ermöglicht mehr Skalierbarkeit in Ihrem Programmdesign und der administrativen Governance. Außerdem bietet es Flexibilität bei regelmäßigen Compliance-Aktualisierungen für Felder, Opt-in-Sprache usw.

* Erwägen Sie, die Vorlagen in Ihrem importierten Programm zu aktualisieren, um die aktuellen Markenvorlagen zu verwenden, oder aktualisieren Sie die neu importierte Vorlage, um Ihre Marke widerzuspiegeln, indem Sie einen Ausschnitt oder Ihre entsprechenden Logo-/Fußzeileninformationen hinzufügen.

* Erwägen Sie, die Namenskonvention dieses Programmbeispiels zu aktualisieren, um sie an Ihre Namenskonvention anzupassen.

>[!NOTE]
>
>Denken Sie daran, die Werte für Mein Token in der Programmvorlage und jedes Mal, wenn Sie das Programm verwenden, nach Bedarf zu aktualisieren.

>[!TIP]
>
>Aktivieren Sie die Kampagne „03 - Interagiert mit Follow-up-E-Mail (Programm-Erfolg)“, um den Erfolg vor dem Versand Ihrer E-Mails zu verfolgen.

>[!IMPORTANT]
>
>Meine Token, die auf eine URL verweisen, dürfen die URL http:// oder https:// nicht enthalten. Andernfalls funktioniert der Link innerhalb des Assets nicht ordnungsgemäß.
