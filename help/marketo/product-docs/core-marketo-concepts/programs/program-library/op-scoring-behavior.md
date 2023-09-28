---
description: OP-Scoring-Verhalten - Marketo-Dokumente - Produktdokumentation
title: OP-Scoring-Verhalten
feature: Programs
exl-id: 7822c362-c134-4471-b9a5-4d4f06e989ed
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 33%

---

# OP-Scoring-Verhalten {#op-scoring-behavior}

Bei diesem Beispiel handelt es sich um ein erweitertes (tokenisiertes) operationelles Programm für die Verhaltensbewertung mithilfe eines Marketo Engage-Standardprogramms. Zeigen Sie die Scoring-Werte auf der Registerkarte &quot;My Tokens&quot;des Programms an und bearbeiten Sie sie. Erfordert ein benutzerdefiniertes Punktfeld namens &quot;Verhaltensbewertung&quot;.

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
   <td>Bewertung</td> 
   <td>Verhaltensbewertung</td>
   <td>BehaviorScore</td>
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
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>E-Mail - Klicks auf Link in E-Mail</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Formular - Ausfüllen des Kontaktformulars</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Formular - Ausfüllen des Inhaltsformulars</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Formular - Ausfüllen des Standardformulars</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Formular - Ausfüllen des Ereignisformulars</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Web - lädt alle PDF herunter</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Web - PPC-Scoring</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Web - Besuche wichtiger Webseiten</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Web - Besuche mehrerer Webseiten innerhalb eines Tages</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Live-Ereignis - teilgenommen</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Tradeshow - Beeinflusst</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Messen - Besuchter Stand</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Webinar - Teilnehmer</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Score reduzieren - keine Aktivität</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Score reduzieren - Besuche unerwünschte Webseiten</td>
  </tr>
  <tr> 
   <td>Ordner</td> 
   <td> </td>
   <td>Interaktionen</td>
  </tr>
  <tr> 
   <td>Ordner</td> 
   <td> </td>
   <td>Änderungen des Programmstatus</td>
  </tr>
  <tr> 
   <td>Ordner</td> 
   <td> </td>
   <td>Score-Niedergang</td>
  </tr>
 </tbody> 
</table>

![](assets/op-scoring-behavior-1.png)

## My Tokens Include {#my-tokens-included}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Token-Typ</th> 
   <th>Token-Name</th>
   <th>Wert</th>
  </tr>
  <tr> 
   <td>Bewertung</td> 
   <td><code>{{my.Decrease Score - No Activity}}</code></td>
   <td>-10</td>
  </tr>
  <tr> 
   <td>Bewertung</td> 
   <td><code>{{my.Decrease Score - Visits Undesirable Web Pages}}</code></td>
   <td>-5</td>
  </tr>
  <tr> 
   <td>Bewertung</td> 
   <td><code>{{my.Email - Clicks Link}}</code></td>
   <td>+2</td>
  </tr>
   <tr> 
   <td>Bewertung</td> 
   <td><code>{{my.Form - Fills Out Contact Form}}</code></td>
   <td>+30</td>
  </tr>
  <tr> 
   <td>Bewertung</td> 
   <td><code>{{my.Form - Fills Out Content Form}}</code></td>
   <td>+15</td>
  </tr>
  <tr> 
   <td>Bewertung</td> 
   <td><code>{{my.Form - Fills Out Default Form}}</code></td>
   <td>+10</td>
  </tr>
   <tr> 
   <td>Bewertung</td> 
   <td><code>{{my.Form - Fills-out Event Form}}</code></td>
   <td>+15</td>
  </tr>
  <tr> 
   <td>Bewertung</td> 
   <td><code>{{my.Live Event - Attended}}</code></td>
   <td>+30</td>
  </tr>
   <tr> 
   <td>Bewertung</td> 
   <td><code>{{my.Tradeshow - Influenced}}</code></td>
   <td>+20</td>
  </tr>
  <tr> 
   <td>Bewertung</td> 
   <td><code>{{my.Tradeshow - Visited Booth}}</code></td>
   <td>+5</td>
  </tr>
  <tr> 
   <td>Bewertung</td> 
   <td><code>{{my.Web - Downloaded Any PDF}}</code></td>
   <td>+5</td>
  </tr>
  <tr> 
   <td>Bewertung</td> 
   <td><code>{{my.Web - PPC Scoring}}</code></td>
   <td>+15</td>
  </tr>
   <tr> 
   <td>Bewertung</td> 
   <td><code>{{my.Web - Visits Key Web Pages}}</code></td>
   <td>+5</td>
  </tr>
  <tr> 
   <td>Bewertung</td> 
   <td><code>{{my.Web - Visits Multiple Web Pages in 1 Day}}</code></td>
   <td>+5</td>
  </tr>
  <tr> 
   <td>Bewertung</td> 
   <td><code>{{my.Webinar - Attended}}</code></td>
   <td>+20</td>
  </tr>
 </tbody> 
</table>

## Konfliktregeln {#conflict-rules}

* **Programm-Tags**
   * Erstellen von Tags in diesem Abonnement - _Empfohlen_
   * Ignorieren

* **Landingpage-Vorlage mit demselben Namen**
   * Originalvorlage kopieren - _Empfohlen_
   * Zielvorlage verwenden

* **Bilder mit demselben Namen**
   * Beides beibehalten - _Empfohlen_
   * Element in diesem Abonnement ersetzen

* **E-Mail-Vorlagen mit demselben Namen**
   * Beides beibehalten - _Empfohlen_
   * Vorhandene Vorlage ersetzen

## Bewährte Methoden {#best-practices}

* Jede erstellte Kampagne soll ein Beispiel für den Best Practice-Build sein und nicht speziell für Ihre Anwendungsfälle. Denken Sie daran, die Smart-Kampagnen zu aktualisieren, um Ihre spezifischen Schmerzpunkte und Datenherausforderungen zu beheben.

* Erwägen Sie, die Benennungsregel dieses Programmbeispiels zu aktualisieren, um sie an Ihre Benennungsregel anzupassen.
