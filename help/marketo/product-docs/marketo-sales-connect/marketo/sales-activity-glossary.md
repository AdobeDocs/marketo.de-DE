---
description: Glossar zu Verkaufsaktivitäten - Marketo-Dokumente - Produktdokumentation
title: Glossar zur Verkaufsaktivität
hide: true
hidefromtoc: true
source-git-commit: 70f17106efe52ee742c8e31013e533fc36ce9835
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 15%

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
  <th rowspan="3">Verkaufs-E-Mail senden</th>
  <td>Gesendet von</td>
 </tr>
 <tr>
  <td>Quelle</td>
 </tr>
 <tr>
  <td>Vorlagen-ID</td>
 </tr>
 <tr>
  <th rowspan="3">Verkaufs-E-Mail öffnen</th>
  <td>Gesendet von</td>
 </tr>
 <tr>
  <td>Quelle</td>
 </tr>
 <tr>
  <td>Vorlagen-ID</td>
 </tr>
 <tr>
  <th rowspan="4">angeklickte E-Mail zum Vertrieb</th>
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
  <th rowspan="2">E-Mail zum empfangenen Verkauf</th>
  <td>Erhalten von</td>
 </tr>
 <tr>
  <td>Quelle</td>
 </tr>
 <tr>
  <th rowspan="4">Verkaufs-E-Mail war aufgrund eines Bounce-Ereignisses unzustellbar</th>
  <td>Details</td>
 </tr>
 <tr>
  <td>Vorlagen-ID</td>
 </tr>
 <tr>
  <td>E-Mail</td>
 </tr>
 <tr>
  <td>Gesendet von</td>
 </tr>
 <tr>
  <th rowspan="7">Hat Verkaufsanruf empfangen</th>
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
  <tr> 
   <td><strong>Erhalten von</strong></td> 
   <td>E-Mail-Adresse der Person, die die E-Mail gesendet hat.</td> 
  </tr> 
  <tr> 
   <td><strong>Details</strong></td> 
   <td>Details zur Bounce-Fehlermeldung.</td> 
  </tr> 
  <tr> 
   <td><strong>E-Mail</strong></td> 
   <td>Bounce-E-Mail-Adresse.</td> 
  </tr> 
 </tbody> 
</table>