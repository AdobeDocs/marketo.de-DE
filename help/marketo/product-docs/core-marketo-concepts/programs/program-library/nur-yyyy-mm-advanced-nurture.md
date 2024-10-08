---
description: NUR-YYYY-MM-Erweiterte Krankenversicherung - Marketo Docs - Produktdokumentation
title: NUR-YYYY-MM-Advanced Nurture
feature: Programs
exl-id: bd9c6605-a13f-4c73-aaa8-eca43cfcc950
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 13%

---

# NUR-YYYY-MM-Advanced Nurture {#nur-yyyy-mm-advanced-nurture}

Dies ist ein Beispiel für fortschrittliche Nurture-Programme, die das Marketo Engage Engagement-Programm nutzen. Verschachtelte E-Mail-Programme verhindern, dass Benutzer bereits konsumierte Inhalte empfangen, oder steuern, welche Art von Inhalt sie in den einzelnen Streams verwenden sollten. Attributionsberichte können für jedes einzelne verschachtelte E-Mail-Programm ausgeführt werden. Kanäle: &quot;Krankenpflege&quot; und ein spezieller Kanal &quot;E-Mail-Pflege&quot; für die verschachtelten E-Mail-Programme senden eine Newsletter-E-Mail mit einem Marketo Engage-E-Mail-Programm. Die E-Mail kann einen A/B-Test enthalten oder nicht.

Wenden Sie sich für weitere Strategiehilfen oder Hilfe beim Anpassen eines Programms an das Adobe-Account-Team oder besuchen Sie die Seite [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"} .

## Kanal-Zusammenfassung {#channel-summary}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Kanal</th> 
   <th>Status der Mitgliedschaft</th>
   <th>Analytics Behavior</th>
   <th>Programmtyp</th>
  </tr> 
  <tr> 
   <td>Nurture-Kampagne</td> 
   <td>01 - Mitglied 
<br/>02 - Interagiert - Erfolg</td>
   <td>Einschließlich</td>
   <td>Interaktion</td>
  </tr>
  <tr> 
   <td>E-Mail-Nurturing</td> 
   <td>01 - Überspringen 
<br/>02 - Gesendet
<br/>03 - Interagiert - Erfolg</td>
   <td>Einschließlich</td>
   <td>Standard</td>
  </tr>
 </tbody> 
</table>

## Das Programm enthält die folgende Assets {#program-contains-the-following-assets}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Typ</th> 
   <th>Vorlagenname</th>
   <th>Asset-Name</th>
  </tr> 
   <tr> 
   <td>Verschachteltes Programm</td> 
   <td> </td>
   <td>01 - Thema X</td>
  </tr>
  <tr> 
   <td>Verschachteltes Programm</td> 
   <td> </td>
   <td>02 - Thema Y</td>
  </tr>
  <tr> 
   <td>Verschachteltes Programm</td> 
   <td> </td>
   <td>03 - Thema Z</td>
  </tr>
  <tr> 
   <td>E-Mail</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Schnellstart-E-Mail-Vorlage</a></td>
   <td>01 - E-Mail (Live in verschachtelten Programmen)</td>
  </tr>
   <tr> 
   <td>E-Mail</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Schnellstart-E-Mail-Vorlage</a></td>
   <td>02 - E-Mail (Live in verschachtelten Programmen)</td>
  </tr>
   <tr> 
   <td>E-Mail</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Schnellstart-E-Mail-Vorlage</a></td>
   <td>03 - E-Mail (Live in verschachtelten Programmen)</td>
  </tr>
  <tr> 
   <td>Lokaler Bericht</td> 
   <td> </td>
   <td>E-Mail-Leistung</td>
  </tr>
  <tr> 
   <td>Lokaler Bericht</td> 
   <td> </td>
   <td>E-Mail-Link-Leistung</td>
  </tr>
  <tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>01 - Zu Krankenpflege hinzufügen</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>02 - Anhalten</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>03 - Wiederaufnahme der Fortpflanzung</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>04 - Interagiert (Programmerfolg)</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>00 - E-Mail überspringen (in jedem verschachtelten Programm lokalisiert)</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>01 - E-Mail senden (in jedem verschachtelten Programm lokalisiert)</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>02 - Engaged-Success (in jedem verschachtelten Programm lokalisiert)</td>
  </tr>
  <tr> 
   <td>Ordner</td> 
   <td> </td>
   <td>Assets (enthält verschachtelte Programme und Asset-Ordner, die auch in verschachtelten Programmen gespeichert sind, um E-Mails zu enthalten)</td>
  </tr>
  <tr> 
   <td>Ordner</td> 
   <td> </td>
   <td>Verschachtelte Programme (Lives under Assets Folder)</td>
  </tr>
  <tr> 
   <td>Ordner</td> 
   <td> </td>
   <td>Kampagnen - Houses all Smart Campaigns in parent Nurture program and campaign folders are ebenfalls in each Nested Program</td>
  </tr>
  <tr> 
   <td>Ordner</td> 
   <td> </td>
   <td>Berichte</td>
  </tr>
 </tbody> 
</table>

![](assets/nur-yyyy-mm-advanced-nurture-1.png)

## My Tokens Include {#my-tokens-included}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Token-Typ</th> 
   <th>Token-Name</th>
   <th>Wert</th>
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
 </tbody> 
</table>

## Konfliktregeln {#conflict-rules}

* **Programm-Tags**
   * Erstellen von Tags in diesem Abonnement - _Empfohlen_
   * Ignorieren

* **Vorlage für Einstiegsseiten mit demselben Namen**
   * Originalvorlage kopieren
   * Verwenden Sie die Zielvorlage - _Empfohlen_

* **Bilder mit demselben Namen**
   * Beide Dateien beibehalten
   * Ersetzen des Elements in diesem Abonnement - _Empfohlen_

* **E-Mail-Vorlagen mit demselben Namen**
   * Beide Vorlagen beibehalten
   * Vorhandene Vorlage ersetzen - _Empfohlen_

## Bewährte Methoden {#best-practices}

* Aktualisieren Sie die Vorlagen in Ihrem importierten Programm, um die derzeit verwendeten Vorlagen zu verwenden, oder aktualisieren Sie die neu importierte Vorlage entsprechend Ihrer Marke, indem Sie einen Ausschnitt oder Ihre entsprechenden Logos-/Fußzeileninformationen hinzufügen.

* Erwägen Sie, die Benennungsregel dieses Programmbeispiels zu aktualisieren, um sie an Ihre Benennungsregel anzupassen.

* Stellen Sie sicher, dass Sie Regeln eingerichtet haben, um Ihre Pflegekadenz anzuhalten und wieder aufzunehmen. Diese Smart-Kampagnen sollten aktiviert oder geplant werden, bevor das Interaktionsprogramm aktiviert wird.

>[!NOTE]
>
>Denken Sie daran, die &quot;My Token Values&quot;-Werte in der Programmvorlage und jedes Mal, wenn Sie das Programm verwenden, nach Bedarf zu aktualisieren.

>[!TIP]
>
>Vergessen Sie nicht, die Kampagne &quot;04 - Interagiert (Programmerfolg)&quot; zu aktivieren, um den Erfolg zu verfolgen! Führen Sie dies _vor_ aus, wenn Ihre E-Mails gesendet werden.
