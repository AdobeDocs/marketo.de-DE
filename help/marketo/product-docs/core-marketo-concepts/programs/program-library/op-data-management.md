---
description: OP-Data Management - Marketo-Dokumente - Produktdokumentation
title: OP-Data Management
feature: Programs
exl-id: ac4a522b-37a7-4080-83d6-fbc2203a568b
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '319'
ht-degree: 26%

---

# OP-Data Management {#op-data-management}

Dies ist ein Beispiel für einen einfachen Workflow mit Best Practices für das Betriebsdatenmanagement, der ein Standardprogramm verwendet, um Ihnen bei der Verwaltung der Datenkonsistenz für Datensätze in Ihrer Marketo Engage-Datenbank zu helfen.

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
   <td>Land normalisieren - USA</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Normalize Country - United Kingdom</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Auf die Blockierungsliste gesetzt auf True setzen</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Ist Partner auf "True"setzen</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Listenimport</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Live-Veranstaltung</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Online-Werbung</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Messe</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Web-Inhalt</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Web-Anforderung</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Webinar</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Neue Person aus Listenimport</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Neue Person aus Live-Ereignis</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Neue Person aus Online Advertising</td>
  </tr>
  <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Neue Person aus der Fachmesse</td>
  </tr>
   <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Neue Person aus Web-Inhalten</td>
  </tr>
   <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Neue Person aus Web-Anforderung</td>
  </tr>
   <tr> 
   <td>Intelligente Kampagne</td> 
   <td> </td>
   <td>Neue Person aus Webinar</td>
  </tr>
  <tr> 
   <td>Ordner</td> 
   <td> </td>
   <td>Person Source Nightly Batch (für Instanzen mit hohem Traffic)</td>
  </tr>
  <tr> 
   <td>Ordner</td> 
   <td> </td>
   <td>Person Source ausgelöst (für Instanzen mit geringem Traffic)</td>
  </tr>
  <tr> 
   <td>Ordner</td> 
   <td> </td>
   <td>Person Source erfassen</td>
  </tr>
  <tr> 
   <td>Ordner</td> 
   <td> </td>
   <td>Normalisierung</td>
  </tr>
  <tr> 
   <td>Ordner</td> 
   <td> </td>
   <td>Datensatzverwaltung</td>
  </tr>
  <tr> 
   <td>Ordner</td> 
   <td> </td>
   <td>Sperrliste</td>
  </tr>
 </tbody> 
</table>

![](assets/op-data-management-1.png)

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
