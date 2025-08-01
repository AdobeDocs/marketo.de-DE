---
description: NUR-YYYY-MM-Simple Nurture - Marketo-Dokumentation - Produktdokumentation
title: NUR-YYYY-MM-Simple Nurture
feature: Programs
exl-id: aed11d75-3190-46ea-8b0b-c1494645901d
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 15%

---

# NUR-YYYY-MM-Simple Nurture {#nur-yyyy-mm-simple-nurture}

Dies ist ein Beispiel für Simple Nurture-Programme, bei denen das Marketo Engage Engagement-Programm verwendet wird. Dabei werden Inhalte im Zeitverlauf in die Datenbank übertragen, während Streams verwendet werden, um Datensätze anhand des Verhaltens durch die Journey zu leiten.

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
   <td>Nurture-Kampagne</td>
   <td>01 - Mitglied
<br/>02 - Interagiert - Erfolg</td>
   <td>Einschließlich</td>
   <td>Interaktion</td>
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
   <td>E-Mail</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Schnellstart-E-Mail-Vorlage</a></td>
   <td>02 - E-Mail</td>
  </tr>
   <tr>
   <td>E-Mail</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Schnellstart-E-Mail-Vorlage</a></td>
   <td>03 - E-Mail</td>
  </tr>
  <tr>
   <td>Lokaler Bericht</td>
   <td> </td>
   <td>E-Mail-Leistung</td>
  </tr>
  <tr>
   <td>Lokaler Bericht</td>
   <td> </td>
   <td>Engagement-Stream Performance</td>
  </tr>
  <tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>01 - Zu Nurture hinzufügen</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>02 - Pause Nurture</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>03 - Resume Nurture</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>04 - Interagiert (Programm erfolgreich)</td>
  </tr>
  <tr>
   <td>Ordner</td>
   <td> </td>
   <td>Assets - enthält alle Kreativ-Assets
   <br/>(Unterordner für E-Mails)</td>
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

![](assets/nur-yyyy-mm-simple-nurture-1.png)

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

* Stellen Sie sicher, dass Sie über Regeln verfügen, um Ihre Kadenz für das Pflegen auszusetzen und wieder aufzunehmen. Diese intelligenten Kampagnen sollten aktiviert oder geplant werden, bevor das Interaktionsprogramm aktiviert wird.

>[!NOTE]
>
>Denken Sie daran, die Werte für Mein Token in der Programmvorlage und jedes Mal, wenn Sie das Programm verwenden, nach Bedarf zu aktualisieren.

>[!TIP]
>
>Vergessen Sie nicht, die Kampagne „04 - Interagiert (Programmerfolg)“ zu aktivieren, um den Erfolg zu verfolgen! Tun Sie dies _vor_ wenn Ihre E-Mails gesendet werden.
