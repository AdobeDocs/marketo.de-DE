---
description: Glossar zur Vertriebsaktivität - Marketo-Dokumente - Produktdokumentation
title: Glossar zur Verkaufsaktivität
exl-id: c7805642-07b6-4697-9efe-5c673ae9ca53
feature: Marketo Sales Connect
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 36%

---

# Glossar zur Verkaufsaktivität {#sales-activity-glossary}

Wenn in Sales Connect ein Verkäufer: einen Lead zu einer Verkaufskadenz hinzufügt, ihm eine E-Mail sendet oder einen Aufruf zu einer Aktivität ausführt, wird dies unter dem Aktivitätsverlauf von Marketo protokolliert. Wenn der Lead mit E-Mails interagiert, werden außerdem Öffnungen, Klicks und Antworten protokolliert.

Die folgenden Aktivitäten werden von Sales Connect bei Marketo protokolliert.

>[!NOTE]
>
>Diese Aktivitäten und Attribute können über unsere REST- und Bulk-API genutzt werden.

## Aktivitäten {#activities}

<table>
 <tr>
  <th>Sales-Aktivität</th>
  <th>Attribut</th>
 </tr>
 <tr>
  <th rowspan="9">Verkaufs-E-Mail senden</th>
  <td>Gesendet von</td>
 </tr>
 <tr>
  <td>Quelle</td>
 </tr>
 <tr>
  <td>Vorlagen-ID</td>
 </tr>
 <tr>
  <td>Verkaufsvorlagen-URL</td>
 </tr>
 <tr>
  <td>Verkaufskampagne URL</td>
 </tr>
 <tr>
  <td>Name der Verkaufsvorlage</td>
 </tr>
 <tr>
  <td>E-Mail-Betreff</td>
 </tr>
 <tr>
  <td>Verkaufskampagne Name</td>
 </tr>
 <tr>
  <td>Marketo-Verkäufer-ID</td>
 </tr>
 <tr>
  <th rowspan="9">Verkaufs-E-Mail öffnen</th>
  <td>Gesendet von</td>
 </tr>
 <tr>
  <td>Quelle</td>
 </tr>
 <tr>
  <td>Vorlagen-ID</td>
 </tr>
 <tr>
  <td>Verkaufsvorlagen-URL</td>
 </tr>
 <tr>
  <td>Verkaufskampagne URL</td>
 </tr>
 <tr>
  <td>Name der Verkaufsvorlage</td>
 </tr>
 <tr>
  <td>E-Mail-Betreff</td>
 </tr>
 <tr>
  <td>Verkaufskampagne Name</td>
 </tr>
 <tr>
  <td>Marketo-Verkäufer-ID</td>
 </tr>
 <tr>
  <th rowspan="10">Verkaufs-E-Mail angeklickt</th>
  <td>Link</td>
 </tr>
 <tr>
  <td>Gesendet von</td>
 </tr>
 <tr>
  <td>Quelle</td>
 </tr>
 <tr>
  <td>Vorlagen-ID</td>
 </tr>
 <tr>
  <td>Verkaufsvorlagen-URL</td>
 </tr>
 <tr>
  <td>Verkaufskampagne URL</td>
 </tr>
 <tr>
  <td>Name der Verkaufsvorlage</td>
 </tr>
 <tr>
  <td>E-Mail-Betreff</td>
 </tr>
 <tr>
  <td>Verkaufskampagne Name</td>
 </tr>
 <tr>
  <td>Marketo-Verkäufer-ID</td>
 </tr>
<tr>
  <th rowspan="3">Hat auf Vertriebsemail geantwortet</th>
  <td>Empfangen von</td>
 </tr>
 <tr>
  <td>Quelle</td>
 </tr>
 <tr>
  <td>Marketo-Verkäufer-ID</td>
 </tr>
 <tr>
  <th rowspan="11">Hat Verkaufsanruf empfangen</th>
  <td>Verkaufsanruf getätigt von</td>
 </tr>
 <tr>
  <td>Verkaufsanruf Status</td>
 </tr>
 <tr>
  <td>Verkaufsanruf Betreff</td>
 </tr>
 <tr>
  <td>Verkaufskampagne Name</td>
 </tr>
 <tr>
  <td>Verkaufskampagne URL</td>
 </tr>
 <tr>
  <td>Angerufene Telefonnummer des Verkaufs</td>
 </tr>
 <tr>
  <td>Quelle</td>
 </tr>
 <tr>
  <td>Dauer des Verkaufsgesprächs</td>
 </tr>
 <tr>
  <td>URL für die Aufzeichnung von Verkaufsanrufen</td>
 </tr>
  <tr>
  <td>Verkaufsanruf beantwortet von</td>
 </tr>
 <tr>
  <td>Marketo-Verkäufer-ID</td>
 </tr>
 <tr>
  <th rowspan="6">Zur Verkaufskampagne hinzufügen</th>
  <td>Verkaufskampagne Name</td>
 </tr>
 <tr>
  <td>Verkaufsanruf Status</td>
 </tr>
 <tr>
  <td>Verkaufskampagne URL</td>
 </tr>
 <tr>
  <td>Gesendet von</td>
 </tr>
 <tr>
  <td>Quelle</td>
 </tr>
 <tr>
  <td>Vertriebskampagnen-ID</td>
 </tr>
 <tr>
  <th rowspan="6">Aus Verkaufskampagne entfernen</th>
  <td>Verkaufskampagne Name</td>
 </tr>
 <tr>
  <td>Verkaufsanruf Status</td>
 </tr>
 <tr>
  <td>Verkaufskampagne URL</td>
 </tr>
 <tr>
  <td>Gesendet von</td>
 </tr>
 <tr>
  <td>Quelle</td>
 </tr>
 <tr>
  <td>Vertriebskampagnen-ID</td>
 </tr>
 <tr>
  <th rowspan="5">E-Mail-Bounce für Verkauf</th>
  <td>Details</td>
 </tr>
 <tr>
  <td>E-Mail</td>
 </tr>
 <tr>
  <td>Gesendet von</td>
 </tr>
 <tr>
  <td>Marketo-Verkäufer-ID</td>
 </tr>
 <tr>
  <td>Vorlagen-ID</td>
 </tr>
</table>

## Beschreibungen {#descriptions}

<table> 
 <tr>
  <th>Attribut</th>
  <th>Beschreibung</th>
 </tr>
 <tbody> 
 <tr> 
   <td><strong>Details</strong></td> 
   <td>Details der Bounce-Fehlermeldung.</td> 
  </tr> 
  <tr> 
   <td><strong>E-Mail</strong></td> 
   <td>E-Mail-Adresse, die zurückkam.</td> 
  </tr> 
  <tr> 
   <td><strong>Link</strong></td> 
   <td>Angeklickte URL.</td> 
  </tr> 
  <tr> 
   <td><strong>Marketo-Verkäufer-ID</strong></td> 
   <td>Eindeutige ID für Personendatensatz in Sales Connect.</td> 
  </tr> 
  <tr> 
   <td><strong>Empfangen von</strong></td> 
   <td>E-Mail-Adresse des Absenders der E-Mail.</td> 
  </tr>
  <tr> 
   <td><strong>Verkaufsanruf beantwortet von</strong></td> 
   <td>Name der Person, die den Anruf entgegengenommen hat.</td> 
  </tr>
  <tr> 
   <td><strong>Dauer des Verkaufsgesprächs</strong></td> 
   <td>Länge des Aufrufs in Sekunden.</td> 
  </tr>
  <tr> 
   <td><strong>Verkaufsanruf getätigt von</strong></td> 
   <td>E-Mail-Adresse des Verkäufers, der den Anruf getätigt hat.</td> 
  </tr>
  <tr> 
   <td><strong>URL für die Aufzeichnung von Verkaufsanrufen</strong></td> 
   <td>URL der Anrufaufzeichnung.</td> 
  </tr>
  <tr> 
   <td><strong>Verkaufsanruf Status</strong></td> 
   <td>Speichert den endgültigen Anrufstatus des Anrufs, der Folgendes umfasst: Abgeschlossen, keine Antwort, Abgebrochen, Fehlgeschlagen.</td> 
  </tr>
  <tr> 
   <td><strong>Verkaufsanruf Betreff</strong></td> 
   <td>Anrufergebnis, das von einem Verkaufsbenutzer in der Wählhilfe ausgewählt wird.</td> 
  </tr>
  <tr> 
   <td><strong>Vertriebskampagnen-ID</strong></td> 
   <td>Eindeutige ID für Sales Campaign-Asset in Sales Connect.</td> 
  </tr>
  <tr> 
   <td><strong>Verkaufskampagne Name</strong></td> 
   <td>Name der Verkaufskampagne.</td> 
  </tr>
  <tr> 
   <td><strong>Verkaufskampagne URL</strong></td> 
   <td>Sales Connect-URL für die Verkaufskampagne.</td> 
  </tr>
  <tr> 
   <td><strong>E-Mail-Betreff für Verkauf</strong></td> 
   <td>Betreffzeile der E-Mail, gefolgt von einer eindeutigen ID (z. B.: Meine Betreffzeile (MSC-12345678)</td> 
  </tr>
  <tr> 
   <td><strong>Angerufene Telefonnummer des Verkaufs</strong></td> 
   <td>Telefonnummer, die vom Vertrieb angerufen wurde.</td> 
  </tr>
  <tr> 
   <td><strong>Name der Verkaufsvorlage</strong></td> 
   <td>Name der E-Mail-Vorlage in Sales Connect.</td> 
  </tr>
  <tr> 
   <td><strong>Verkaufsvorlagen-URL</strong></td> 
   <td>Sales Connect-URL für E-Mail-Vorlage.</td> 
  </tr>
  <tr> 
   <td><strong>Gesendet von</strong></td>
   <td>E-Mail-Adresse des Absenders der E-Mail.</td> 
  </tr> 
  <tr> 
   <td><strong>Quelle</strong></td> 
   <td>Source der Aktivität. Wird für Sales Connect-Aktivitäten vor der Version vom Oktober 2021 als „Tout“ festgelegt. Wird nach der Version vom Oktober 2021 „Sales App“ für Sales Connect-Aktivitäten.</td>
  </tr> 
  <tr> 
   <td><strong>Vorlagen-ID</strong></td> 
   <td>Wenn die Quelle Tout ist, ist die Vorlagen-ID die Marketo Sales Connect-Vorlagen-ID. Verwenden Sie diese Option, um eine bestimmte Vorlage anstelle der Betreffzeile auszuwählen, die in mehreren Vorlagen vorhanden sein könnte.
</td> 
  </tr> 
 </tbody> 
</table>
