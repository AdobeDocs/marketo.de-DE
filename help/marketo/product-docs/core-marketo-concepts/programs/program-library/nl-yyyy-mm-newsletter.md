---
description: NL-YYYY-MM-Newsletter - Marketo Docs - Produktdokumentation
title: NL-YYYY-MM-Newsletter
feature: Programs
exl-id: bce05e0f-e288-4614-9d05-c14844615454
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 16%

---

# NL-YYYY-MM-Newsletter {#nl-yyyy-mm-newsletter}

In diesem Beispiel wird eine Newsletter-E-Mail mit einem Marketo Engage-E-Mail-Programm gesendet. Die E-Mail kann einen A/B-Test enthalten oder nicht.

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
   <td>Newsletter</td>
   <td>01-Mitglied
<br/>02-ENGAGED-SUCCESS</td>
   <td>Einschließlich</td>
   <td>E-Mail</td>
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
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Schnellstart-E-Mail-Vorlage</a></td>
   <td>01 - E-Mail</td>
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
   <td>01 - Interagiert (Programm erfolgreich)</td>
  </tr>
  <tr>
   <td>Ordner</td>
   <td> </td>
   <td>Assets - enthält alle Kreativ-Assets
<br/>(Unterordner für E-Mails)  </td>
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

![](assets/nl-yyyy-mm-newsletter-1.png)

## Meine Token enthalten {#my-tokens-included}

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

* Erwägen Sie, die Vorlagen in Ihrem importierten Programm zu aktualisieren, um die aktuellen Markenvorlagen zu verwenden, oder aktualisieren Sie die neu importierte Vorlage, um Ihre Marke widerzuspiegeln, indem Sie einen Ausschnitt oder Ihre entsprechenden Logo-/Fußzeileninformationen hinzufügen.

* Erwägen Sie, die Namenskonvention dieses Programmbeispiels zu aktualisieren, um sie an Ihre Namenskonvention anzupassen.

>[!NOTE]
>
>Denken Sie daran, die Werte für Mein Token in der Programmvorlage und jedes Mal, wenn Sie das Programm verwenden, nach Bedarf zu aktualisieren.

>[!TIP]
>
>Vergessen Sie nicht, die Kampagne „01-Engaged“ zu aktivieren, um den Erfolg zu verfolgen! Tun Sie dies _vor_ wenn Ihr Formular live ist und E-Mails gesendet werden.
