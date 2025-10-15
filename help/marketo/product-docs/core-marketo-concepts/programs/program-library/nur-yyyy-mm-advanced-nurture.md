---
description: NUR-YYYY-MM-Advanced Nurture - Marketo-Dokumentation
title: 'Erweitertes Nurturing: NUR-JJJJ-MM'
feature: Programs
exl-id: bd9c6605-a13f-4c73-aaa8-eca43cfcc950
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 16%

---

# Erweitertes Nurturing: NUR-JJJJ-MM {#nur-yyyy-mm-advanced-nurture}

Dies ist ein Beispiel für erweiterte Nurture-Programme, die das Marketo Engage Engagement Program verwenden. Verschachtelte E-Mail-Programme verhindern, dass Personen Inhalte erhalten, die sie bereits konsumiert haben, oder steuern den Typ des Inhalts, den sie in jedem Stream konsumieren sollen. Attributionsberichte können für jedes einzelne verschachtelte E-Mail-Programm ausgeführt werden. Kanäle: „Pflegen“ und ein dedizierter Kanal „Pflege-E-Mail“ für die verschachtelten E-Mail-Programme senden eine Newsletter-E-Mail mit einem Marketo Engage-E-Mail-Programm. Die E-Mail kann einen A/B-Test enthalten oder nicht.

Wenden Sie sich an das Adobe-Accountteam oder besuchen Sie die Seite [Adobe Professional Services](https://business.adobe.com/de/customers/consulting-services/main.html){target="_blank"}, um weitere Unterstützung bei der Strategie oder bei der Anpassung eines Programms zu erhalten.

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
  <tr>
   <td>E-Mail-Nurturing</td>
   <td>01 - Überspringen
<br/>02 - gesendet
<br/>03 - Interagiert - Erfolg</td>
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
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">E-Mail-Vorlage für Schnellstart</a></td>
   <td>01 - E-Mail (Live in verschachtelten Programmen)</td>
  </tr>
   <tr>
   <td>E-Mail</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">E-Mail-Vorlage für Schnellstart</a></td>
   <td>02 - E-Mail (Live in verschachtelten Programmen)</td>
  </tr>
   <tr>
   <td>E-Mail</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">E-Mail-Vorlage für Schnellstart</a></td>
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
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>00 - E-Mail überspringen (in jedem verschachtelten Programm)</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>01 - E-Mail senden (in jedem verschachtelten Programm)</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>02 - Engaged-Success (in jedem verschachtelten Programm)</td>
  </tr>
  <tr>
   <td>Ordner</td>
   <td> </td>
   <td>Assets (enthält verschachtelte Programme und Asset-Ordner, die auch in verschachtelten Programmen vorhanden sind, um E-Mails zu enthalten)</td>
  </tr>
  <tr>
   <td>Ordner</td>
   <td> </td>
   <td>Verschachtelte Programme (in Assets verfügbar)</td>
  </tr>
  <tr>
   <td>Ordner</td>
   <td> </td>
   <td>Kampagnen - Alle Smart-Kampagnen im übergeordneten Nurture-Programm werden gespeichert, und die Kampagnenordner befinden sich ebenfalls in jedem verschachtelten Programm.</td>
  </tr>
  <tr>
   <td>Ordner</td>
   <td> </td>
   <td>Berichte</td>
  </tr>
 </tbody>
</table>

![](assets/nur-yyyy-mm-advanced-nurture-1.png)

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
