---
description: Glossar zu Verkaufsaktivitäten - Marketo-Dokumente - Produktdokumentation
title: Glossar zur Verkaufsaktivität
exl-id: c7805642-07b6-4697-9efe-5c673ae9ca53
source-git-commit: 84a285974de3bbcdf33e24befae323d3d82ef239
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 7%

---

# Glossar zur Verkaufsaktivität {#sales-activity-glossary}

Wenn ein Verkäufer in Sales Connect: fügt einen Lead zu einem Verkaufskatalog hinzu, sendet ihm eine E-Mail oder tätigt einen Aufruf an eine Aktivität. Er wird im Verlauf der Marketo-Aktivität protokolliert. Wenn der Lead mit E-Mails interagiert, werden auch Öffnungen, Klicks und Antworten protokolliert.

Die folgenden Aktivitäten werden von Sales Connect aus bei Marketo protokolliert.

>[!NOTE]
>
>Diese Aktivitäten und Attribute können über unsere REST- und Bulk-API genutzt werden.

## Aktivitäten {#activities}

<table>
 <tr>
  <th>Verkaufsaktivität</th>
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
  <td>URL der Verkaufsvorlage</td>
 </tr>
 <tr>
  <td>Vertriebskampagnen-URL</td>
 </tr>
 <tr>
  <td>Name der Verkaufsvorlage</td>
 </tr>
 <tr>
  <td>Email Subject</td>
 </tr>
 <tr>
  <td>Name der Verkaufskampagne</td>
 </tr>
 <tr>
  <td>Marketo Sales Person ID</td>
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
  <td>URL der Verkaufsvorlage</td>
 </tr>
 <tr>
  <td>Vertriebskampagnen-URL</td>
 </tr>
 <tr>
  <td>Name der Verkaufsvorlage</td>
 </tr>
 <tr>
  <td>Email Subject</td>
 </tr>
 <tr>
  <td>Name der Verkaufskampagne</td>
 </tr>
 <tr>
  <td>Marketo Sales Person ID</td>
 </tr>
 <tr>
  <th rowspan="10">angeklickte E-Mail zum Vertrieb</th>
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
  <td>URL der Verkaufsvorlage</td>
 </tr>
 <tr>
  <td>Vertriebskampagnen-URL</td>
 </tr>
 <tr>
  <td>Name der Verkaufsvorlage</td>
 </tr>
 <tr>
  <td>Email Subject</td>
 </tr>
 <tr>
  <td>Name der Verkaufskampagne</td>
 </tr>
 <tr>
  <td>Marketo Sales Person ID</td>
 </tr>
<tr>
  <th rowspan="3">E-Mail zum empfangenen Verkauf</th>
  <td>Erhalten von</td>
 </tr>
 <tr>
  <td>Quelle</td>
 </tr>
 <tr>
  <td>Marketo Sales Person ID</td>
 </tr>
 <tr>
  <th rowspan="11">Hat Verkaufsanruf empfangen</th>
  <td>Verkaufsaufruf von</td>
 </tr>
 <tr>
  <td>Status der Verkaufsaufrufe</td>
 </tr>
 <tr>
  <td>Verkaufsgespräch</td>
 </tr>
 <tr>
  <td>Name der Verkaufskampagne</td>
 </tr>
 <tr>
  <td>Vertriebskampagnen-URL</td>
 </tr>
 <tr>
  <td>Telefonnummer des Verkäufers aufgerufen</td>
 </tr>
 <tr>
  <td>Quelle</td>
 </tr>
 <tr>
  <td>Dauer der Verkaufsaufrufe</td>
 </tr>
 <tr>
  <td>URL zur Aufzeichnung von Verkaufsaufrufen</td>
 </tr>
  <tr>
  <td>Verkaufsaufruf beantwortet von</td>
 </tr>
 <tr>
  <td>Marketo Sales Person ID</td>
 </tr>
 <tr>
  <th rowspan="6">Zur Verkaufskampagne hinzufügen</th>
  <td>Name der Verkaufskampagne</td>
 </tr>
 <tr>
  <td>Status der Verkaufsaufrufe</td>
 </tr>
 <tr>
  <td>Vertriebskampagnen-URL</td>
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
  <th rowspan="6">Aus Vertriebskampagne entfernen</th>
  <td>Name der Verkaufskampagne</td>
 </tr>
 <tr>
  <td>Status der Verkaufsaufrufe</td>
 </tr>
 <tr>
  <td>Vertriebskampagnen-URL</td>
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
   <td>Details zur Bounce-Fehlermeldung.</td> 
  </tr> 
  <tr> 
   <td><strong>E-Mail</strong></td> 
   <td>Bounce-E-Mail-Adresse.</td> 
  </tr> 
  <tr> 
   <td><strong>Link</strong></td> 
   <td>URL, auf die geklickt wurde.</td> 
  </tr> 
  <tr> 
   <td><strong>Marketo Sales Person ID</strong></td> 
   <td>Eindeutige ID für den Personendatensatz in Sales Connect.</td> 
  </tr> 
  <tr> 
   <td><strong>Erhalten von</strong></td> 
   <td>E-Mail-Adresse der Person, die die E-Mail gesendet hat.</td> 
  </tr>
  <tr> 
   <td><strong>Verkaufsaufruf beantwortet von</strong></td> 
   <td>Name der Person, die den Anruf entgegengenommen hat.</td> 
  </tr>
  <tr> 
   <td><strong>Dauer der Verkaufsaufrufe</strong></td> 
   <td>Länge des Aufrufs in Sekunden.</td> 
  </tr>
  <tr> 
   <td><strong>Verkaufsaufruf von</strong></td> 
   <td>E-Mail-Adresse der Verkaufsperson, die den Anruf getätigt hat.</td> 
  </tr>
  <tr> 
   <td><strong>URL zur Aufzeichnung von Verkaufsaufrufen</strong></td> 
   <td>URL der Aufrufaufzeichnung.</td> 
  </tr>
  <tr> 
   <td><strong>Status der Verkaufsaufrufe</strong></td> 
   <td>Speichert den endgültigen Aufrufstatus des Aufrufs, der Folgendes enthält: abgeschlossen, keine Antwort, abgebrochen, fehlgeschlagen.</td> 
  </tr>
  <tr> 
   <td><strong>Verkaufsgespräch</strong></td> 
   <td>Rufen Sie das Ergebnis auf, das von einem Vertriebsbenutzer im Dialer ausgewählt wird.</td> 
  </tr>
  <tr> 
   <td><strong>Vertriebskampagnen-ID</strong></td> 
   <td>Eindeutige ID für Sales Campaign-Assets in Sales Connect.</td> 
  </tr>
  <tr> 
   <td><strong>Name der Verkaufskampagne</strong></td> 
   <td>Name der Verkaufskampagne.</td> 
  </tr>
  <tr> 
   <td><strong>Vertriebskampagnen-URL</strong></td> 
   <td>Sales Connect-URL für die Vertriebskampagne.</td> 
  </tr>
  <tr> 
   <td><strong>Sales Email Subject</strong></td> 
   <td>Betreffzeile der E-Mail</td> 
  </tr>
  <tr> 
   <td><strong>Telefonnummer des Verkäufers aufgerufen</strong></td> 
   <td>Telefonnummer, die von Sales aufgerufen wird.</td> 
  </tr>
  <tr> 
   <td><strong>Name der Verkaufsvorlage</strong></td> 
   <td>Name der E-Mail-Vorlage in Sales Connect.</td> 
  </tr>
  <tr> 
   <td><strong>URL der Verkaufsvorlage</strong></td> 
   <td>Sales Connect-URL für E-Mail-Vorlage.</td> 
  </tr>
  <tr> 
   <td><strong>Gesendet von</strong></td>
   <td>E-Mail-Adresse der Person, die die E-Mail gesendet hat.</td> 
  </tr> 
  <tr> 
   <td><strong>Quelle</strong></td> 
   <td>Quelle der Aktivität. Wird für Sales Connect-Aktivitäten als "Tout"festgelegt.</td> 
  </tr> 
  <tr> 
   <td><strong>Vorlagen-ID</strong></td> 
   <td>Wenn die Quelle Tout ist, ist die Vorlagen-ID die Marketo Sales Connect-Vorlagen-ID. Verwenden Sie dies, um eine bestimmte Vorlage anstelle der Betreffzeile auszuwählen, die in mehreren Vorlagen vorhanden sein könnte.
</td> 
  </tr> 
 </tbody> 
</table>
