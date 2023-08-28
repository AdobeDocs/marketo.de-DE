---
description: OP-Akquise-API - Marketo-Dokumente - Produktdokumentation
title: OP-Akquise-API
hide: true
hidefromtoc: true
feature: Programs
source-git-commit: 0f71600b18315feb3ef32e95dfb108b09c4cb79f
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 26%

---

# OP-Akquise-API {#op-acquisition-api}

Dieses Beispielprogramm dient zur Verfolgung der Akquise von Datensätzen aus API-Quellen mithilfe eines Marketo Engage-Standardprogramms.

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
   <td>Akquise festlegen - Batch</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Akquise festlegen - Trigger</td>
  </tr>
  <tr> 
   <td>Ordner</td> 
   <td> </td>
   <td>Kampagnen (enthält alle Smart-Kampagnen)</td>
  </tr>
 </tbody> 
</table>

BILDSCHIRM DES PROGRAMMS

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

ÜBERSICHT ÜBER KONFLIKTREGELN

## Bewährte Methoden {#best-practices}

* Führen Sie zuerst die Batch-Kampagne aus, wenn Sie in Ihrer Datenverwaltung aufholen müssen.

* Erwägen Sie die Verwendung ähnlicher Programme, um die Abstimmung an Best Practices für alle Eingabequellen sicherzustellen, damit Ihre CRM- oder Datenintegrationen einbezogen werden.

* Erfassen Sie bei kanalspezifischen Marketinginitiativen bei Bedarf die Akquise.
