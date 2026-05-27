---
description: Vorlage für das operationelle Zustellbarkeits-Management. Verwenden Sie sie, um die Zustellbarkeit von E-Mails zu gewährleisten.
title: OP-Verwaltung der Zustellbarkeit
feature: Programs
exl-id: 7b9bc9ee-65f4-4938-8598-6f8543042159
TQID: https://experienceleague.adobe.com/cJTv2uEq6YUEDphACUTypZOrkoLxTU0GRaPo43Igzjw
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: e64968b2-4ee5-47f9-8cae-0588f184b9ebid: f82558ea-6af5-44eb-a424-5b3389abb0a3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 277
ht-degree: 19%

---

# OP-Verwaltung der Zustellbarkeit {#op-deliverability-management}

Dies ist ein Beispiel für Best Practice-Workflows zur Zustellbarkeitsverwaltung, die ein Marketo Engage-Standardprogramm verwenden, um Ihren aktuellen Zustand der E-Mail-Zustellbarkeit zu überprüfen und chronische Bounces und Non-Responder zu verwalten.

>[!NOTE]
>
>Erfordert das benutzerdefinierte Zeichenfolgenfeld „Grund für ausgesetztes Marketing“ zum Importieren. [Weitere Informationen](https://nation.marketo.com/community/product_and_support/support_solutions/blog/2016/04/18/how-to-monitor-deliverability-using-marketo){target="_blank"}.

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
   <td>Betrieblich</td>
   <td>01-Mitglied</td>
   <td>Betrieblich</td>
   <td>Standard</td>
  </tr>
 </tbody>
</table>

## Vorausgesetzte Felder {#prerequisite-fields}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Typ</th>
   <th>Anzeigename</th>
   <th>API-Name</th>
  </tr>
  <tr>
   <td>String</td>
   <td>Grund für ausgesetztes Marketing</td>
   <td>MarketingSuspendedReason</td>
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
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>Marketing-Suspendierung chronischer Non-Responder</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>Marketing-Aussetzen für chronisch unzustellbare E-Mails</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>„E-Mail ungültig“ nach E-Mail-Aktualisierung zurücksetzen</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>„Marketing ausgesetzt“ nach E-Mail-Aktualisierung zurücksetzen</td>
  </tr>
  <tr>
   <td>Ordner</td>
   <td> </td>
   <td>Verwalten</td>
  </tr>
  <tr>
   <td>Ordner</td>
   <td> </td>
   <td>Überprüfung</td>
  </tr>
 </tbody>
</table>

![](assets/op-deliverability-management-1.png)

## Kollisionsregeln {#conflict-rules}

* **Programm-Tags**
   * Tags in diesem Abonnement erstellen - _Empfohlen_
   * Ignorieren

* **Landingpage-Vorlage mit demselben Namen**
   * Originalvorlage kopieren - _Empfohlen_
   * Zielvorlage verwenden

* **Bilder mit demselben Namen**
   * Beide Dateien beibehalten - _Empfohlen_
   * Element in diesem Abonnement ersetzen

* **E-Mail-Vorlagen mit demselben Namen**
   * Beide Vorlagen beibehalten - _Empfohlen_
   * Vorhandene Vorlage ersetzen

## Bewährte Methoden {#best-practices}

* Jede erstellte Kampagne ist als Beispiel für den Best-Practice-Build gedacht und nicht spezifisch für Ihre Anwendungsfälle. Denken Sie daran, die Smart Campaign zu aktualisieren, um Ihre spezifischen Probleme und Herausforderungen bezüglich der Daten zu bewältigen.

* Erwägen Sie, die Namenskonvention dieses Programmbeispiels zu aktualisieren, um sie an Ihre Namenskonvention anzupassen.
