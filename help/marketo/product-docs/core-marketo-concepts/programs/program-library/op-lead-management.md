---
description: Vorlage für das operationelle Programm für Lead-Management. Verwalten Sie damit den Lead-Lebenszyklus und die Bewertung.
title: OP-Lead-Management
feature: Programs
exl-id: bde644fe-d40b-4c9c-925d-a0f522e6de01
TQID: https://experienceleague.adobe.com/KJvZjFZ9OsjIXXZTfbnscxf8puUxu-IxFXnNaj9JJFs
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: c5f60233-d5ea-4453-a799-0ad258b4d399id: e64968b2-4ee5-47f9-8cae-0588f184b9ebid: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2: id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 279
ht-degree: 16%

---

# OP-Lead-Management {#op-lead-management}

Dies ist ein Beispiel für Best Practice-Workflows für das Lead-Management, die ein Marketo Engage-Standardprogramm verwenden, um Sie bei der Verwaltung von Datensätzen in Ihrer Marketo Engage-Datenbank für Ihr CRM-System zu unterstützen.

>[!NOTE]
>
>In Marketo Engage werden Datensätze in Ihrer Datenbank als Personen/Personen bezeichnet. Die Lead-Verwaltung in diesem Beispiel bezieht sich auf die Datensätze in Ihrem CRM.

Wenden Sie sich für weitere Strategieunterstützung oder Hilfe bei der Anpassung eines Programms an das Adobe-Accountteam oder besuchen Sie die Seite [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html).

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
   <td>01 - Neue Personen mit CRM synchronisieren</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>02 - Marketing qualifiziert</td>
  </tr>
  <tr>
   <td>E-Mail</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">E-Mail-Vorlage für Schnellstart</a></td>
   <td>01 - E-MAIL - WARNHINWEIS - MQL</td>
  </tr>
  <tr>
   <td>Ordner</td>
   <td> </td>
   <td>Kampagnen</td>
  </tr>
  <tr>
   <td>Ordner</td>
   <td> </td>
   <td>E-Mail-Warnung</td>
  </tr>
 </tbody>
</table>

![](assets/op-lead-management-1.png)

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

* Erwägen Sie das Hinzufügen zusätzlicher intelligenter Kampagnen, um alle Lebenszyklusstatus-Anforderungen zu erfüllen, die Sie in Ihrer Organisation möglicherweise verfolgen. Jede in diesem Programm erstellte Kampagne ist als Beispiel für die Erstellung von Best Practices gedacht und ist nicht für alle Anwendungsfälle spezifisch. Denken Sie daran, die Smart-Kampagnen entsprechend Ihrem spezifischen Lead-Lebenszyklus-Management-Prozess zu aktualisieren.

* Erwägen Sie, die Namenskonvention dieses Programmbeispiels zu aktualisieren, damit sie mit Ihrer übereinstimmt.
