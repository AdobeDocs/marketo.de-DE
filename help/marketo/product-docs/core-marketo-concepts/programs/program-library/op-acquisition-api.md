---
description: Vorlage für das operationelle Programm der Akquise-API. Verwendet, um Leads über API zu erfassen.
title: OP-Akquise-API
feature: Programs
exl-id: abf7c4a0-c363-4e92-9a1f-197c3953c515
TQID: https://experienceleague.adobe.com/a-4w7mJg44cvotVtX2qwx1e4p8SKIbQU1jPWyQ0BzUA
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2:
  - id: df401a2a-327d-468c-a5e4-b7b7ccd071a0
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 182
ht-degree: 21%

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

* Stellen Sie innerhalb kanalspezifischer Marketing-Initiativen sicher, dass bei Bedarf Akquise erfasst wird.
