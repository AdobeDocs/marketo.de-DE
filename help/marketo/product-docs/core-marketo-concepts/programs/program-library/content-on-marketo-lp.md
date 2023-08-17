---
description: Inhalt auf Marketo LP - Marketo Docs - Produktdokumentation
title: Inhalt in Marketo LP
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 661a41eb0c5c43541a63a36c31837b35f516d827
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 13%

---

# Inhalt in Marketo LP {#content-on-marketo-lp}

Programmname: CT-YYYY-MM-Content on Marketo LP

Diese Beispielreferenz ist als Inhaltsprogramm konzipiert, das eine Marketo-Landingpage mit einem Marketo-Formular mit einem Marketo-Standardprogramm nutzt. Das Formular dient dem Zugriff auf den Inhalt/das Angebot. Der Link zum Angebot kann auf der Dankeseite angezeigt, in einer Dankesemail oder in beiden. Weitere Hilfe zur Strategie oder Hilfe bei der Anpassung eines Programms erhalten Sie vom Adobe-Account-Team oder unter [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html) Seite.

**Kanal-Zusammenfassung**

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

**Das Programm enthält die folgenden Assets:**

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
   <td>Landing Page</td> 
   <td>Schnellstart-LP-Vorlage</td>
   <td>01 - LP - Registrierung</td>
  </tr>
  <tr> 
   <td>Landing Page</td> 
   <td>Schnellstart-LP-Vorlage</td>
   <td>02 - LP - Vielen Dank</td>
  </tr>
  <tr> 
   <td>Formular</td> 
   <td> </td>
   <td>Formular zur Inhaltsregistrierung</td>
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
   <td>Assets - Host alle Kreativ-Assets 
<br/>(Unterordner für E-Mail und Landingpages)  </td>
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

SCREENSHOT - Bild des Programms

**Meine Token umfassten:**

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Token-Typ</th> 
   <th>Token-Name</th>
   <th>Wert </th>
  </tr> 
  <tr> 
   <td>RTF</td> 
   <td><code>{{my.Content-Description}}</code></td>
   <td>Doppelklicken für Details  
<br/><code><--My Content Description Here--></code> 
<br/>Bearbeiten Sie diese Inhaltsbeschreibung auf der Programmebene auf der Registerkarte My Tokens . 
<br/>Sie werden Folgendes erfahren: 
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
   <td><code>{{my. Email-ReplyToAddress}}</code></td>
   <td>reply-to.email@mydomain.com</td>
  </tr>
  <tr> 
   <td>Text</td> 
   <td><code>{{my.PageURL-ThankYou}}</code></td>
   <td>My.Vielen DankYouPageURL?ohne http://</td>
  </tr>
 </tbody> 
</table>

>[!CAUTION]
>
>Siehe Programmimportanleitungen für standardmäßige Konfliktregeln .

**Empfohlene standardmäßige Konfliktregeln für den Import:**

* Programm-Tags
   * In diesem Abonnement Tags erstellen (Standard) - Empfohlen
   * Ignorieren

* Landingpage-Vorlage mit demselben Namen
   * Originalvorlage kopieren (Standard)
   * Verwenden der Zielvorlage - Empfohlen

* Bilder mit demselben Namen
   * Beide Dateien beibehalten (Standard)
   * Element in diesem Abonnement ersetzen - Empfohlen

* E-Mail-Vorlagen mit demselben Namen
   * Beides beibehalten (Standard)
   * Vorhandene Vorlage ersetzen - Empfohlen

SCREENSHOT - Bild der standardmäßigen Konfliktregeln

**Empfohlene Best Practices:**

* Marketo Consulting Best Practices empfehlen, das Formular nach dem Import des Inhaltsprogramms von einem lokalen Asset in ein globales Asset in Design Studio von Marketo Engage zu verschieben.
   * Die Verringerung der Anzahl von Formularen und die Verwendung von mehr globalen Assets aus Design Studio ermöglichen eine größere Skalierbarkeit in der Programmentwicklung und Verwaltungsführung. Es bietet außerdem Flexibilität bei regelmäßigen Aktualisierungen der Kompatibilität für Felder, Opt-in-Sprache usw.

* Aktualisieren Sie die Vorlagen in Ihrem importierten Programm, um die derzeit verwendeten Vorlagen zu verwenden, oder aktualisieren Sie die neu importierte Vorlage entsprechend Ihrer Marke, indem Sie einen Ausschnitt oder Ihre entsprechenden Logos- und Fußzeileninformationen hinzufügen.

* Falls erforderlich, sollten Sie die Benennungskonvention für diese Programmvorlage aktualisieren, um sie an Ihre Benennungskonvention anzupassen.

* Vergessen Sie nicht, die My Token Values auf der Programmvorlage und jedes Mal, wenn Sie das Programm verwenden, nach Bedarf zu aktualisieren.

* Weitere Hilfe zur Strategie oder Hilfe bei der Anpassung eines Programms erhalten Sie von Ihrem Adobe-Account-Team oder unter [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html) Seite.

>[!TIP]
>
>Vergessen Sie nicht, die Kampagne &quot;02-engagiert&quot;zu aktivieren, um den Erfolg zu verfolgen! Führen Sie dies aus, BEVOR Ihr Formular live ist und E-Mails gesendet werden.

>[!NOTE]
>
>Meine Token, die auf eine URL verweisen, können http:// oder https:// nicht enthalten. Andernfalls funktioniert der Link im Asset nicht ordnungsgemäß.
