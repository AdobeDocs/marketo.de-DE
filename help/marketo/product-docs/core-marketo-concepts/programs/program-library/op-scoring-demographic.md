---
description: Bewertung der Vorlage für das operationelle Programm „Demografische Bewertung“. Verwenden Sie ihn für die demografisch basierte Lead-Bewertung.
title: OP-Scoring-Demografie
feature: Programs
exl-id: ed11616e-b587-4d03-b293-9cc9fa3c1699
TQID: https://experienceleague.adobe.com/AQLLsHWsrvSN0lyexi4HjCBc1L-Zh7-q-jc8R60O7RI
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 326
ht-degree: 34%

---

# OP-Scoring-Demografie {#op-scoring-demographic}

Dies ist ein Beispiel für ein erweitertes (mit Token versehenes) operationelles Programm, das ein Marketo Engage-Standardprogramm für die demografische Bewertung verwendet. Zeigen Sie die Scoring-Werte auf der Registerkarte „Meine Token“ des Programms an und bearbeiten Sie sie. Erfordert ein benutzerdefiniertes Bewertungsfeld namens „Demografische Bewertung“.

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
   <td>Betrieblich</td>
   <td>01 - Mitglied</td>
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
   <td>Ergebnis</td>
   <td>Demografische Bewertung</td>
   <td>Demografische Bewertung</td>
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
   <td>Allgemeine E-Mail-Domain</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>Ungültiger Vorname</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>Ungültiger Vorname aktualisiert</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>Ungültiger Nachname</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>Ungültiger Nachname aktualisiert</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>Jahresumsatz</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>Branche</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>Jobtitel</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>Anzahl der Mitarbeiter</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>Quelle</td>
  </tr>
  <tr>
   <td>Ordner</td>
   <td> </td>
   <td>Allgemeine E-Mail-Domain</td>
  </tr>
  <tr>
   <td>Ordner</td>
   <td> </td>
   <td>Ungültiger Vorname</td>
  </tr>
  <tr>
   <td>Ordner</td>
   <td> </td>
   <td>Ungültiger Nachname</td>
  </tr>
 </tbody>
</table>

![](assets/op-scoring-demographic-1.png)

## Meine Token enthalten {#my-tokens-included}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Token-Typ</th>
   <th>Token-Name</th>
   <th>Wert</th>
  </tr>
  <tr>
   <td>Ergebnis</td>
   <td><code>{{my.Annual Revenue - High}}</code></td>
   <td>+15</td>
  </tr>
  <tr>
   <td>Ergebnis</td>
   <td><code>{{my.Annual Revenue - Low}}</code></td>
   <td>+5</td>
  </tr>
  <tr>
   <td>Ergebnis</td>
   <td><code>{{my.Annual Revenue - Mid}}</code></td>
   <td>+10</td>
  </tr>
   <tr>
   <td>Ergebnis</td>
   <td><code>{{my.Generic Email Domain}}</code></td>
   <td>-2</td>
  </tr>
  <tr>
   <td>Ergebnis</td>
   <td><code>{{my.Industry - High}}</code></td>
   <td>+10</td>
  </tr>
  <tr>
   <td>Ergebnis</td>
   <td><code>{{my.Industry - Low}}</code></td>
   <td>+6</td>
  </tr>
   <tr>
   <td>Ergebnis</td>
   <td><code>{{my.Industry - Mid}}</code></td>
   <td>+8</td>
  </tr>
  <tr>
   <td>Ergebnis</td>
   <td><code>{{my.Invalid First Name}}</code></td>
   <td>-5</td>
  </tr>
   <tr>
   <td>Ergebnis</td>
   <td><code>{{my.Invalid First Name Updated}}</code></td>
   <td>+5</td>
  </tr>
  <tr>
   <td>Ergebnis</td>
   <td><code>{{my.Invalid Last Name}}</code></td>
   <td>-5</td>
  </tr>
  <tr>
   <td>Ergebnis</td>
   <td><code>{{my.Invalid Last Name Updated}}</code></td>
   <td>+5</td>
  </tr>
  <tr>
   <td>Ergebnis</td>
   <td><code>{{my.Job Title - High}}</code></td>
   <td>+15</td>
  </tr>
   <tr>
   <td>Ergebnis</td>
   <td><code>{{my.Job Title - Low}}</code></td>
   <td>+5</td>
  </tr>
  <tr>
   <td>Ergebnis</td>
   <td><code>{{my.Job Title - Mid}}</code></td>
   <td>+10</td>
  </tr>
  <tr>
   <td>Ergebnis</td>
   <td><code>{{my.Lead Source - High}}</code></td>
   <td>+20</td>
  </tr>
  <tr>
   <td>Ergebnis</td>
   <td><code>{{my.Lead Source - Low}}</code></td>
   <td>+8</td>
  </tr>
  <tr>
   <td>Ergebnis</td>
   <td><code>{{my.Lead Source - Mid}}</code></td>
   <td>+10</td>
  </tr>
  <tr>
   <td>Ergebnis</td>
   <td><code>{{my.Number of Employees}}</code></td>
   <td>+5</td>
  </tr>
 </tbody>
</table>

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

* Jede erstellte Kampagne ist als Beispiel für den Build von Best Practices gedacht und nicht spezifisch für Ihre Anwendungsfälle. Denken Sie daran, die Smart Campaign zu aktualisieren, um Ihre spezifischen Probleme und Herausforderungen bezüglich der Daten zu bewältigen.

* Erwägen Sie, die Namenskonvention dieses Programmbeispiels zu aktualisieren, um sie an Ihre Namenskonvention anzupassen.
