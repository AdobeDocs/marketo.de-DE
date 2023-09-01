---
description: Landingpage CT-YYY-MM-Content non-Marketo - Marketo Docs - Produktdokumentation
title: Einstiegsseite für CT-YYY-MM-Content (Nicht-Marketo-Inhalt)
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 17b86ff816a447315dda5e1cbac67536472e777d
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 18%

---

# Einstiegsseite für CT-YYY-MM-Content (Nicht-Marketo-Inhalt) {#ct-yyyy-mm-content-non-marketo-landing-page}

Dies ist ein Beispiel für ein Inhaltsprogramm mit einem Marketo Engage-Formular zum Herunterladen von Inhalten auf einer nicht-Marketo Engage-Landingpage, das ein Marketo Engage-Standardprogramm verwendet. Dieses Programm ist für die Arbeit mit einem auf Ihrer Website eingebetteten Marketo Engage-Formular vorgesehen. Der Link zum Angebot/Inhalt kann in einer Dankesemail gesendet werden.

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
   <td>Webinhalt</td> 
   <td>01-Mitglied 
<br/>02-Engaged-Success</td>
   <td>Inklusiv</td>
   <td>Standard</td>
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
   <td>Formular</td> 
   <td> </td>
   <td>Formular zur FM-Inhaltsregistrierung (globales Asset in Design Studio)</td>
  </tr>
  <tr> 
   <td>Lokaler Bericht</td> 
   <td> </td>
   <td>E-Mail-Leistung</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>00-Capture Acquisition Program</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>01 Ausgefülltes Formular</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>02-Engagiert (Programmerfolg)</td>
  </tr>
  <tr> 
   <td>Ordner</td> 
   <td> </td>
   <td>Assets - Häusert alle Kreativ-Assets 
<br/>(Unterordner für E-Mails und Landingpages)  </td>
  </tr>
  <tr> 
   <td>Ordner</td> 
   <td> </td>
   <td>Kampagnen - Alle Smart-Kampagnen werden beherbergt</td>
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

* Verschieben Sie das Formular nach dem Import des Inhaltsprogramms von einem lokalen Asset in ein globales Asset in Design Studio.
   * Die Verringerung der Anzahl von Formularen und die Verwendung von mehr globalen Assets aus Design Studio ermöglichen eine größere Skalierbarkeit in der Programmentwicklung und Verwaltungsführung. Es bietet außerdem Flexibilität für regelmäßige Aktualisierungen der Kompatibilität für Felder, Opt-in-Sprache usw.

* Aktualisieren Sie die Vorlagen in Ihrem importierten Programm, um die derzeit verwendeten Vorlagen zu verwenden, oder aktualisieren Sie die neu importierte Vorlage entsprechend Ihrer Marke, indem Sie einen Ausschnitt oder Ihre entsprechenden Logos-/Fußzeileninformationen hinzufügen.

* Erwägen Sie, die Benennungsregel dieses Programmbeispiels zu aktualisieren, um sie an Ihre Benennungskonvention anzupassen.

>[!NOTE]
>
>Denken Sie daran, die &quot;My Token Values&quot;-Werte in der Programmvorlage und jedes Mal, wenn Sie das Programm verwenden, nach Bedarf zu aktualisieren.

>[!TIP]
>
>Vergessen Sie nicht, die Kampagne &quot;02-engagiert&quot;zu aktivieren, um den Erfolg zu verfolgen! Verwenden Sie dies _before_ Ihr Formular ist live und E-Mails werden gesendet.
