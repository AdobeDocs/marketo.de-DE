---
description: Vorlage für das operationelle Programm „Daten-Management“. Verwenden Sie diese Option, um Ihre Datenbank sauber und auf dem neuesten Stand zu halten.
title: OP-Daten-Management
feature: Programs
exl-id: ac4a522b-37a7-4080-83d6-fbc2203a568b
TQID: https://experienceleague.adobe.com/EGzqLIOGFIpRAB2OoDhRBTheiHBtitfI29T8TvZQNp0
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: c5f60233-d5ea-4453-a799-0ad258b4d399id: e64968b2-4ee5-47f9-8cae-0588f184b9ebid: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2: id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 335
ht-degree: 27%

---

# OP-Daten-Management {#op-data-management}

Dies ist ein Beispiel für einfache Best Practice-Workflows für das Betriebsdaten-Management unter Verwendung eines Standardprogramms, das Sie bei der Verwaltung der Datenkonsistenz für Datensätze in Ihrer Marketo Engage-Datenbank unterstützt.

Wenden Sie sich an das Adobe-Accountteam oder besuchen Sie die Seite [Adobe Professional Services](https://business.adobe.com/de/customers/consulting-services/main.html){target="_blank"}, um weitere Unterstützung bei der Strategie oder bei der Anpassung eines Programms zu erhalten.

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
   <td>Land normalisieren - Vereinigte Staaten</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>Normalisierungsland - Vereinigtes Königreich</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>Auf „True“ festlegen</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>Ist Partner auf „true“ gesetzt</td>
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
   <td>Neue Person vom Live-Ereignis</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>Neue Person von Online Advertising</td>
  </tr>
  <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>Neue Person von der Messe</td>
  </tr>
   <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>Neue Person aus Webinhalten</td>
  </tr>
   <tr>
   <td>Intelligente Kampagne</td>
   <td> </td>
   <td>Neue Person aus Web-Anfrage</td>
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
   <td>Ausgelöste Personen-Source (für Instanzen mit geringem Traffic)</td>
  </tr>
  <tr>
   <td>Ordner</td>
   <td> </td>
   <td>Person-Source erfassen</td>
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

* Jede erstellte Kampagne ist als Beispiel für den Best-Practice-Build gedacht und nicht spezifisch für Ihre Anwendungsfälle. Denken Sie daran, die Smart Campaign zu aktualisieren, um Ihre spezifischen Probleme und Herausforderungen bezüglich der Daten zu bewältigen.

* Erwägen Sie, die Namenskonvention dieses Programmbeispiels zu aktualisieren, um sie an Ihre Namenskonvention anzupassen.
