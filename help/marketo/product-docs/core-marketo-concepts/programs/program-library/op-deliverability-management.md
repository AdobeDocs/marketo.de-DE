---
description: Verwaltung der OP-Zustellbarkeit - Marketo-Dokumente - Produktdokumentation
title: Verwaltung der OP-Zustellbarkeit
feature: Programs
exl-id: 7b9bc9ee-65f4-4938-8598-6f8543042159
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 18%

---

# Verwaltung der OP-Zustellbarkeit {#op-deliverability-management}

Dies ist ein Beispiel für Best Practice-Workflows bei der Zustellbarkeitsverwaltung, die ein Marketo Engage-Standardprogramm verwenden, um Ihren aktuellen Status der E-Mail-Zustellbarkeit zu überprüfen und chronische Bounces und Nicht-Responder zu verwalten.

>[!NOTE]
>
>Erfordert den Import des benutzerdefinierten Zeichenfolgenfelds &quot;Marketing Suspended Reason&quot;. [Weitere Infos](https://nation.marketo.com/community/product_and_support/support_solutions/blog/2016/04/18/how-to-monitor-deliverability-using-marketo){target="_blank"}.

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
   <td>Zeichenfolge</td> 
   <td>Ausgesetzte Marketing-Begründung</td>
   <td>MarketingSuspendedReason</td>
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
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Chronische Non-Respondern auf das Inverkehrbringen</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Marketingaussetzen chronisch abgeschnittener E-Mails</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Zurücksetzen von "E-Mail ungültig"nach E-Mail-Update</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Zurücksetzen von "Marketing ausgesetzt" nach E-Mail-Update</td>
  </tr>
  <tr> 
   <td>Ordner</td> 
   <td> </td>
   <td>Verwalten</td>
  </tr>
  <tr> 
   <td>Ordner</td> 
   <td> </td>
   <td>Überprüfen
</td>
  </tr>
 </tbody> 
</table>

![](assets/op-deliverability-management-1.png)

## Konfliktregeln {#conflict-rules}

* **Programm-Tags**
   * Erstellen von Tags in diesem Abonnement - _Empfohlen_
   * Ignorieren

* **Vorlage für Einstiegsseiten mit demselben Namen**
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
