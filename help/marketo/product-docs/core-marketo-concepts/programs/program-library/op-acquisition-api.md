---
description: OP-Acquisition-API - Marketo-Dokumente - Produktdokumentation
title: OP-Akquise-API
feature: Programs
exl-id: abf7c4a0-c363-4e92-9a1f-197c3953c515
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 19%

---

# OP-Akquise-API {#op-acquisition-api}

Dieses Beispielprogramm ist für operative Prozesse vorgesehen, um die Erfassung von Datensätzen aus API-Quellen mithilfe eines Marketo Engage-Standardprogramms zu verfolgen.

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
   <td>Set-Akquise - Batch</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>Set Acquisition - Trigger</td>
  </tr>
  <tr>
   <td>Ordner</td>
   <td> </td>
   <td>Kampagnen (enthält alle Smart-Kampagnen)</td>
  </tr>
 </tbody>
</table>

![](assets/op-acquisition-api-1.png)

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

* Führen Sie zuerst die Batch-Kampagne aus, wenn Sie in Ihrem Daten-Management Nachholbedarf haben.

* Erwägen Sie die Verwendung ähnlicher Programme, um sicherzustellen, dass diese über alle Eingabequellen hinweg an Best Practices ausgerichtet sind, um Ihre CRM- oder Datenintegrationen einzuschließen.

* Achten Sie darauf, bei Bedarf im Rahmen kanalspezifischer Marketing-Initiativen Akquise zu erfassen.
