---
description: EM-JJJJ-MM-TT-Einzelversand einer E-Mail - Marketo-Dokumente - Produktdokumentation
title: EM-JJJJ-MM-TT-Einzelner E-Mail-Versand
feature: Programs
exl-id: 58782d4c-658b-42cd-9ca3-fa53c7476e48
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 16%

---

# EM-JJJJ-MM-TT-Einzelner E-Mail-Versand {#em-yyyy-mm-dd-single-email-send}

In diesem Beispiel wird eine E-Mail mit einem Marketo Engage-E-Mail-Programm gesendet. Die E-Mail kann einen A/B-Test enthalten oder nicht.

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
   <td>E-Mail</td> 
   <td>01-Mitglied 
<br/>02-Engaged-Success</td>
   <td>Einschließlich</td>
   <td>E-Mail</td>
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
   <td>E-Mail</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Schnellstart-E-Mail-Vorlage</a></td>
   <td>01-Email-Vielen Dank</td>
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
   <td>01-Engagiert (Programmerfolg)</td>
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

![](assets/em-yyyy-mm-dd-single-email-send-1.png)

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

>[!NOTE]
>
>Denken Sie daran, die &quot;My Token Values&quot;-Werte in der Programmvorlage und jedes Mal, wenn Sie das Programm verwenden, nach Bedarf zu aktualisieren.

>[!TIP]
>
>Vergessen Sie nicht, die Kampagne &quot;01-engagiert&quot;zu aktivieren, um den Erfolg zu verfolgen! Führen Sie diesen Schritt _vor_ aus, wenn Ihr Formular live ist und E-Mails gesendet werden.
