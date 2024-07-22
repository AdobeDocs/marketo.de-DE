---
description: OP-Lead-Management - Marketo-Dokumente - Produktdokumentation
title: OP-Lead-Management
feature: Programs
exl-id: bde644fe-d40b-4c9c-925d-a0f522e6de01
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 13%

---

# OP-Lead-Management {#op-lead-management}

Dies ist ein Beispiel für Best Practice-Workflows für die Lead-Verwaltung, die ein Marketo Engage-Standardprogramm verwenden, um Sie bei der Verwaltung von Datensätzen in Ihrer Marketo Engage-Datenbank in Ihrem CRM-System zu unterstützen.

>[!NOTE]
>
>In Marketo Engage werden Datensätze in Ihrer Datenbank als Personen/Personen bezeichnet. Die Lead-Verwaltung in diesem Beispiel bezieht sich auf die Datensätze in Ihrem CRM-System.

Wenden Sie sich für weitere Strategiehilfen oder Hilfe beim Anpassen eines Programms an das Adobe-Account-Team oder besuchen Sie die Seite [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html) .

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
   <td>01 - Synchronisieren neuer Personen mit CRM</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>02 - Marketing qualifiziert</td>
  </tr>
  <tr> 
   <td>E-Mail</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Schnellstart-E-Mail-Vorlage</a></td>
   <td>01 - E-Mail - WARNUNG - MQL</td>
  </tr>
  <tr> 
   <td>Ordner</td> 
   <td> </td>
   <td>Kampagnen</td>
  </tr>
  <tr> 
   <td>Ordner</td> 
   <td> </td>
   <td>Email Alert</td>
  </tr>
 </tbody> 
</table>

![](assets/op-lead-management-1.png)

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

* Ziehen Sie das Hinzufügen zusätzlicher intelligenter Kampagnen in Erwägung, um alle Lebenszyklusstatus-Anforderungen zu erfüllen, die Sie möglicherweise in Ihrem Unternehmen verfolgen. Jede in diesem Programm erstellte Kampagne soll ein Beispiel für den Best Practice-Build sein und nicht für alle Anwendungsfälle spezifisch sein. Denken Sie daran, die Smart-Kampagnen zu aktualisieren, um Ihren spezifischen Prozess des Lead-Lebenszyklusmanagements zu berücksichtigen.

* Erwägen Sie, die Namenskonvention für dieses Programmbeispiel zu aktualisieren und sie an Ihre anzupassen.
