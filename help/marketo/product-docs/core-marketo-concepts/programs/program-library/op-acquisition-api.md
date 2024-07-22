---
description: OP-Akquise-API - Marketo-Dokumente - Produktdokumentation
title: OP-Akquise-API
feature: Programs
exl-id: abf7c4a0-c363-4e92-9a1f-197c3953c515
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 19%

---

# OP-Akquise-API {#op-acquisition-api}

Dieses Beispielprogramm dient zur Verfolgung der Akquise von Datensätzen aus API-Quellen mithilfe eines Marketo Engage-Standardprogramms.

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

![](assets/op-acquisition-api-1.png)

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

* Führen Sie zuerst die Batch-Kampagne aus, wenn Sie in Ihrer Datenverwaltung aufholen müssen.

* Erwägen Sie die Verwendung ähnlicher Programme, um die Abstimmung an Best Practices für alle Eingabequellen sicherzustellen, damit Ihre CRM- oder Datenintegrationen einbezogen werden.

* Erfassen Sie bei kanalspezifischen Marketinginitiativen bei Bedarf die Akquise.
