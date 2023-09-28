---
description: TS-YYYY-MM-DD-Tradeshow-Programm - Marketo Docs - Produktdokumentation
title: TS-YYYY-MM-DD-Tradeshow-Programm
feature: Programs
exl-id: 32e4d07e-e9fd-4906-acc4-5f97c09f3c44
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 21%

---

# TS-YYYY-MM-DD-Tradeshow-Programm {#ts-yyyy-mm-dd-tradeshow-program}

Dies ist ein Beispiel für ein Messeprogramm mit Einladungs- und Follow-up-E-Mails unter Verwendung eines Marketo Engage Event Program.

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
   <br/>04-besuchter Stand
   <br/>05-interagiert bei Show - Erfolg
   <br/>60-Grad-Teilnahme an Beitragsshow - Erfolg</td>
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
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Schnellstart-E-Mail-Vorlage</a></td>
   <td>01-Email-Vielen Dank</td>
  </tr>
   <tr> 
   <td>E-Mail</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Schnellstart-E-Mail-Vorlage</a></td>
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
   <td>00 - Akquiseprogramm erfassen</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>01 - Einladung senden</td>
  </tr>
   <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>02 - Folgenachrichten senden</td>
  </tr>
   <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>03 - Interagiert durch Follow-up-E-Mail (Erfolg)</td>
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

![](assets/ts-yyyy-mm-dd-tradeshow-program-1.png)

## Meine Token Enthalten {#my-tokens-included}

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
>Vergessen Sie nicht, die Kampagne &quot;03 - Interagiert mit Folgenachrichten (Programm-Erfolg)&quot; zu aktivieren, um den Erfolg zu verfolgen! Verwenden Sie dies _before_ Ihre E-Mails werden gesendet.

>[!IMPORTANT]
>
>Meine Token, die auf eine URL verweisen, können http:// oder https:// nicht enthalten. Andernfalls funktioniert der Link im Asset nicht ordnungsgemäß.
