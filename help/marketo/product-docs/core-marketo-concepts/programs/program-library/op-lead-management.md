---
description: OP-Lead-Management - Marketo-Dokumente - Produktdokumentation
title: OP-Lead-Management
feature: Programs
source-git-commit: 720215ea958206931413f2d273a4a058bc051579
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 19%

---

# OP-Lead-Management {#op-lead-management}

Dies ist ein Beispiel für Best Practice-Workflows für die Lead-Verwaltung, die ein Marketo Engage-Standardprogramm verwenden, um Sie bei der Verwaltung von Datensätzen in Ihrer Marketo Engage-Datenbank in Ihrem CRM-System zu unterstützen.

>[!NOTE]
>
>In Marketo Engage werden Datensätze in Ihrer Datenbank als Personen/Personen bezeichnet. Die Lead-Verwaltung in diesem Beispiel bezieht sich auf die Datensätze in Ihrem CRM-System.

Weitere Hilfe zur Strategie oder Hilfe bei der Anpassung eines Programms erhalten Sie vom Adobe-Account-Team oder unter [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html) Seite.

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
   <td>E-Mail-Benachrichtigung</td>
  </tr>
 </tbody> 
</table>

![](assets/op-lead-management-1.png)

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

* Ziehen Sie das Hinzufügen zusätzlicher intelligenter Kampagnen in Erwägung, um alle Lebenszyklusstatus-Anforderungen zu erfüllen, die Sie möglicherweise in Ihrem Unternehmen verfolgen. Jede in diesem Programm erstellte Kampagne soll ein Beispiel für den Best Practice-Build sein und nicht für alle Anwendungsfälle spezifisch sein. Denken Sie daran, die Smart-Kampagnen zu aktualisieren, um Ihren spezifischen Prozess des Lead-Lebenszyklusmanagements zu berücksichtigen.

* Erwägen Sie, die Namenskonvention für dieses Programmbeispiel zu aktualisieren und sie an Ihre anzupassen.
