---
description: EV-JJJJ-MM-TT-Event-Programm - Marketo Docs - Produktdokumentation
title: EV-JJJJ-MM-TT-Veranstaltungsprogramm
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: ddc9242bdf1b3ec34bb2672821b6b054647d94b5
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 19%

---

# EV-JJJJ-MM-TT-Veranstaltungsprogramm {#ev-yyyy-mm-dd-event-program}

Dies ist ein Beispiel für ein Veranstaltungsprogramm mit einer Registrierungsseite, drei Einladungs-E-Mails und Follow-up-E-Mails, die ein Marketo Engage Event Program verwenden. Geeignet für alle Veranstaltungen, bei denen Sie sich registrieren lassen müssen, einschließlich Roadshows, Mittagessen, Abendessen oder Präsentationen bei Messen. Verwenden Sie die Marketo Engage Events App zum Einchecken und zur Verfolgung von Besuchern in Ihrer iPad.

Weitere Hilfe zur Strategie oder Hilfe bei der Anpassung eines Programms erhalten Sie vom Adobe-Account-Team oder unter [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"} Seite.

## Kanal-Zusammenfassung {#channel-summary}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Kanal</th> 
   <th>Status der Mitgliedschaft</th>
   <th>Analyseverhalten</th>
   <th>Programmtyp</th>
  </tr> 
  <tr> 
   <td>Veranstaltung</td> 
   <td>01 - Eingeladen 
<br/>02-Waitlisted
<br/>03-Registered
<br/>04-Keine Sendung
<br/>05-Teilnehmer-Erfolg</td>
   <td>Inklusiv</td>
   <td>Veranstaltung</td>
  </tr>
 </tbody> 
</table>

## Das Programm enthält die folgenden Assets {#program-contains-the-following-assets}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Typ</th> 
   <th>Vorlagenname</th>
   <th>Asset-Name</th>
  </tr> 
  <tr> 
   <td>E-Mail</td> 
   <td>Schnellstart-E-Mail-Vorlage</td>
   <td>01-Email-Vielen Dank</td>
  </tr>
   <tr> 
   <td>E-Mail</td> 
   <td>Schnellstart-E-Mail-Vorlage</td>
   <td>02a- E-Mail - Einladung</td>
  </tr>
  <tr> 
   <td>E-Mail</td> 
   <td>Schnellstart-E-Mail-Vorlage</td>
   <td>02b - E-Mail - Erinnerung an Einladung</td>
  </tr>
  <tr> 
   <td>E-Mail</td> 
   <td>Schnellstart-E-Mail-Vorlage</td>
   <td>02c- E-Mail - Einladungs-Erinnerung letzte Chance</td>
  </tr>
  <tr> 
   <td>E-Mail</td> 
   <td>Schnellstart-E-Mail-Vorlage</td>
   <td>03 - E-Mail - An Erinnerung teilnehmen</td>
  </tr>
  <tr> 
   <td>E-Mail</td> 
   <td>Schnellstart-E-Mail-Vorlage</td>
   <td>04a - E-Mail - Follow-up - teilgenommen</td>
  </tr>
  <tr> 
   <td>E-Mail</td> 
   <td>Schnellstart-E-Mail-Vorlage</td>
   <td>04b - E-Mail - Follow-up - NoShow</td>
  </tr>
  <tr> 
   <td>Landing Page</td> 
   <td>Schnellstart-LP-Vorlage</td>
   <td>01a - LP - Registrierung</td>
  </tr>
  <tr> 
   <td>Landing Page</td> 
   <td>Schnellstart-LP-Vorlage</td>
   <td>01b - LP - Vielen Dank</td>
  </tr>
  <tr> 
   <td>Formular</td> 
   <td> </td>
   <td>FM-Ereignisregistrierung</td>
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
   <td>00 - Akquiseprogramm erfassen</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>01 - Prozessregistrierung</td>
  </tr>
   <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>02a - Einladung senden</td>
  </tr>
   <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>02b - Erinnerung senden</td>
  </tr>
   <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>02c - Einladung letzten Zufall senden</td>
  </tr>
   <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>03 - Erinnerung zum Senden senden</td>
  </tr>
   <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>04 - Eingestiegen (Programmerfolg)</td>
  </tr>
   <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>05 - Folgenachrichten senden</td>
  </tr>
  <tr> 
   <td>Ordner</td> 
   <td> </td>
   <td>Assets - Host alle Kreativ-Assets 
<br/>(Unterordner für E-Mail und Landingpages)</td>
  </tr>
  <tr> 
   <td>Ordner</td> 
   <td> </td>
   <td>Kampagnen - Houses all Smart Campaigns</td>
  </tr>
  <tr> 
   <td>Ordner</td> 
   <td> </td>
   <td>Berichte</td>
  </tr>
 </tbody> 
</table>

## Meine Token Enthalten {#my-tokens-included}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Token-Typ</th> 
   <th>Token-Name</th>
   <th>Wert </th>
  </tr>
  <tr> 
   <td>Kalenderdatei</td> 
   <td><code>{{my.AddToCalendar}}</code></td>
   <td>Doppelklicken Sie auf Details</td>
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
   <td><code>{{my.Content-Description}}</code></td>
   <td>Doppelklicken für Details  
<br/><code><--My Content Description Here--></code> 
<br/>Bearbeiten Sie diese Inhaltsbeschreibung auf Programmebene auf der Registerkarte My Tokens . 
<br/>Sie werden Folgendes erfahren: 
<li>Aufzählungszeichen 1</li>
<li>Aufzählungszeichen 2</li>
<li>Aufzählungszeichen 3</li></td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.Event-Location-Line1}}</code></td>
   <td><code><--XYZ Hotel--></code></td>
  </tr>
   <tr> 
   <td>Text</td> 
   <td><code>{{my.Event-Location-Line2}}</code></td>
   <td><code><--ABC Room--></code></td>
  </tr>
   <tr> 
   <td>Text</td> 
   <td><code>{{my.Event-Location-Line3}}</code></td>
   <td><code><--1234 Anystreet--></code></td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.Event-Location-Line4}}</code></td>
   <td><code><--Anytown, ZZ 99999--></code></td>
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
   <td>Live-Veranstaltung</td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.PageURL-Download}}</code></td>
   <td>my.DownloadURL?without=http://</td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.PageURL-Registration}}</code></td>
   <td>my.RegistrationPageURL?without=http://</td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.PageURL-ThankYou}}</code></td>
   <td>my.ThankYouPageURL?without=http://</td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.Speaker1-Name}}</code></td>
   <td><code><--Speaker Name Here--></code></td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.Speaker1-Title}}</code></td>
   <td><code><--Speaker Title Here--></code></td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.Speaker2-Name}}</code></td>
   <td><code><--Speaker Name Here--></code></td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.Speaker2-Title}}</code></td>
   <td><code><--Speaker Title Here--></code></td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.Speaker3-Name}}</code></td>
   <td><code><--Speaker Name Here--></code></td>
  </tr>
 <tr> 
   <td>Text</td> 
   <td><code>{{my.Speaker3-Title}}</code></td>
   <td><code><--Speaker Title Here--></code></td>
  </tr>
 </tbody> 
</table>

BILDSCHIRM DES PROGRAMMS

## Konfliktregeln {#conflict-rules}

* **Programm-Tags**
   * Erstellen von Tags in diesem Abonnement - _Empfohlen_
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

ÜBERSICHT ÜBER KONFLIKTREGELN

## Bewährte Methoden {#best-practices}

* Verschieben Sie das Formular nach dem Import des Webinarprogramms von einem lokalen Asset in ein globales Asset in Design Studio.
   * Die Verringerung der Anzahl von Formularen und die Verwendung von mehr globalen Assets aus Design Studio ermöglichen eine größere Skalierbarkeit in der Programmentwicklung und Verwaltungsführung. Es bietet außerdem Flexibilität bei regelmäßigen Aktualisierungen der Kompatibilität für Felder, Opt-in-Sprache usw.

* Aktualisieren Sie die Vorlagen in Ihrem importierten Programm, um die derzeit verwendeten Vorlagen zu verwenden, oder aktualisieren Sie die neu importierte Vorlage entsprechend Ihrer Marke, indem Sie einen Ausschnitt oder Ihre entsprechenden Logos-/Fußzeileninformationen hinzufügen.

* Erwägen Sie, die Benennungsregel dieses Programmbeispiels zu aktualisieren, um sie an Ihre Benennungsregel anzupassen.

>[!NOTE]
>
>Denken Sie daran, die &quot;My Token Values&quot;-Werte in der Programmvorlage und jedes Mal, wenn Sie das Programm verwenden, nach Bedarf zu aktualisieren.

>[!TIP]
>
>Vergessen Sie nicht, die Kampagne &quot;06-Teilnehmer (Programmerfolg)&quot; zu aktivieren, um den Erfolg zu verfolgen! Verwenden Sie dies _before_ Ihr Formular ist live und E-Mails werden gesendet.

>[!IMPORTANT]
>
>Meine Token, die auf eine URL verweisen, können http:// oder https:// nicht enthalten. Andernfalls funktioniert der Link im Asset nicht ordnungsgemäß.

>[!NOTE]
>
>Laden Sie vor dem Ereignis die Registrierungsinformationen in Ihre iPad herunter. Überprüfen Sie dann die Besucher und synchronisieren Sie die Anwesenheitsinformationen wieder mit Marketo Engage. Wenn du kein Tablet hast, kannst du [Importbeteiligte](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-members-from-a-spreadsheet-into-a-program.md){target="_blank"} im Tab &quot;Mitglieder&quot; des Programms, bevor Sie Ihre Folgenachrichten senden.
