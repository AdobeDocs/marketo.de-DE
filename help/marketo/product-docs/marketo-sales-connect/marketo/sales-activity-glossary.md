---
description: Glossar zur Verkaufsförderung - Marketo Docs - Produktdokumentation
title: Glossar zur Aktivität des Verkaufs
exl-id: c7805642-07b6-4697-9efe-5c673ae9ca53
source-git-commit: 42ddb44100a041a09ff4a68c02ccf6aabb2d953e
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 7%

---

# Glossar zur Aktivität des Verkaufs {#sales-activity-glossary}

In Sales Connect, wenn ein Verkäufer: fügt einen Lead zu einem Vertrieb Cadence, schickt ihnen eine E-Mail, oder macht einen Anruf eine Aktivität, wird es unter dem Marketo Aktivität Verlauf protokolliert. Wenn der Lead mit E-Mails interagiert, werden außerdem Klicks und Antworten protokolliert.

Die folgenden Aktivitäten werden von Sales Connect aus bei Marketo protokolliert.

>[!NOTE]
>
>Diese Aktivitäten und Attribute können über unsere REST- und Massen-API genutzt werden.

## Aktivitäten {#activities}

<table>
 <tr>
  <th>Aktivität des Verkaufs</th>
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
  <td>Verkaufs-Kampagne-URL</td>
 </tr>
 <tr>
  <td>Name der Verkaufsvorlage</td>
 </tr>
 <tr>
  <td>E-Mail-Betreff</td>
 </tr>
 <tr>
  <td>Name der Kampagne</td>
 </tr>
 <tr>
  <td>Marketo-Vertriebskennung</td>
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
  <td>Verkaufs-Kampagne-URL</td>
 </tr>
 <tr>
  <td>Name der Verkaufsvorlage</td>
 </tr>
 <tr>
  <td>E-Mail-Betreff</td>
 </tr>
 <tr>
  <td>Name der Kampagne</td>
 </tr>
 <tr>
  <td>Marketo-Vertriebskennung</td>
 </tr>
 <tr>
  <th rowspan="10">E-Mail mit angeklicktem Vertrieb</th>
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
  <td>Verkaufs-Kampagne-URL</td>
 </tr>
 <tr>
  <td>Name der Verkaufsvorlage</td>
 </tr>
 <tr>
  <td>E-Mail-Betreff</td>
 </tr>
 <tr>
  <td>Name der Kampagne</td>
 </tr>
 <tr>
  <td>Marketo-Vertriebskennung</td>
 </tr>
<tr>
  <th rowspan="3">E-Mail für Verkäufe beantwortet</th>
  <td>Erhalten von</td>
 </tr>
 <tr>
  <td>Quelle</td>
 </tr>
 <tr>
  <td>Marketo-Vertriebskennung</td>
 </tr>
 <tr>
  <th rowspan="11">Hat Verkaufsanruf empfangen</th>
  <td>Verkaufsaufruf erstellt von</td>
 </tr>
 <tr>
  <td>Status des Verkaufsaufrufs</td>
 </tr>
 <tr>
  <td>Verkaufsanruf-Betreff</td>
 </tr>
 <tr>
  <td>Name der Kampagne</td>
 </tr>
 <tr>
  <td>Verkaufs-Kampagne-URL</td>
 </tr>
 <tr>
  <td>Telefonnummer des Verkäufers aufgerufen</td>
 </tr>
 <tr>
  <td>Quelle</td>
 </tr>
 <tr>
  <td>Dauer des Verkaufsaufrufs</td>
 </tr>
 <tr>
  <td>URL zur Aufzeichnung von Verkaufsaufrufen</td>
 </tr>
  <tr>
  <td>Kaufanruf beantwortet von</td>
 </tr>
 <tr>
  <td>Marketo-Vertriebskennung</td>
 </tr>
 <tr>
  <th rowspan="6">Zur Verkaufskampagne hinzufügen</th>
  <td>Name der Kampagne</td>
 </tr>
 <tr>
  <td>Status des Verkaufsaufrufs</td>
 </tr>
 <tr>
  <td>Verkaufs-Kampagne-URL</td>
 </tr>
 <tr>
  <td>Gesendet von</td>
 </tr>
 <tr>
  <td>Quelle</td>
 </tr>
 <tr>
  <td>Vertriebs-Kampagne-ID</td>
 </tr>
 <tr>
  <th rowspan="6">Aus Kampagne des Verkaufs entfernen</th>
  <td>Name der Kampagne</td>
 </tr>
 <tr>
  <td>Status des Verkaufsaufrufs</td>
 </tr>
 <tr>
  <td>Verkaufs-Kampagne-URL</td>
 </tr>
 <tr>
  <td>Gesendet von</td>
 </tr>
 <tr>
  <td>Quelle</td>
 </tr>
 <tr>
  <td>Vertriebs-Kampagne-ID</td>
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
   <td>E-Mail-Adresse, die geknackt wurde.</td> 
  </tr> 
  <tr> 
   <td><strong>Link</strong></td> 
   <td>URL, auf die geklickt wurde.</td> 
  </tr> 
  <tr> 
   <td><strong>Marketo-Vertriebskennung</strong></td> 
   <td>Eindeutige ID für Personendatensätze in Sales Connect.</td> 
  </tr> 
  <tr> 
   <td><strong>Erhalten von</strong></td> 
   <td>E-Mail-Adresse der Person, die die E-Mail gesendet hat.</td> 
  </tr>
  <tr> 
   <td><strong>Kaufanruf beantwortet von</strong></td> 
   <td>Name der Person, die den Anruf beantwortet hat.</td> 
  </tr>
  <tr> 
   <td><strong>Dauer des Verkaufsaufrufs</strong></td> 
   <td>Dauer des Anrufs in Sekunden.</td> 
  </tr>
  <tr> 
   <td><strong>Verkaufsaufruf erstellt von</strong></td> 
   <td>E-Mail-Adresse des Verkäufers, der den Anruf getätigt hat.</td> 
  </tr>
  <tr> 
   <td><strong>URL zur Aufzeichnung von Verkaufsaufrufen</strong></td> 
   <td>URL der Telefonaufzeichnung.</td> 
  </tr>
  <tr> 
   <td><strong>Status des Verkaufsaufrufs</strong></td> 
   <td>speichert den endgültigen Anrufstatus des Anrufs, der Folgendes enthält: abgeschlossen, keine Antwort, abgebrochen, fehlgeschlagen.</td> 
  </tr>
  <tr> 
   <td><strong>Verkaufsanruf-Betreff</strong></td> 
   <td>Ergebnis anrufen, das von einem Vertriebsbenutzer im Dialer ausgewählt wird.</td> 
  </tr>
  <tr> 
   <td><strong>Vertriebs-Kampagne-ID</strong></td> 
   <td>Eindeutige ID für Sales Kampagne-Asset in Sales Connect.</td> 
  </tr>
  <tr> 
   <td><strong>Name der Kampagne</strong></td> 
   <td>Name der Kampagne.</td> 
  </tr>
  <tr> 
   <td><strong>Verkaufs-Kampagne-URL</strong></td> 
   <td>Sales Connect-URL für die Kampagne des Verkaufs.</td> 
  </tr>
  <tr> 
   <td><strong>E-Mail-Betreff für Verkäufe</strong></td> 
   <td>Betreffzeile der E-Mail.</td> 
  </tr>
  <tr> 
   <td><strong>Telefonnummer des Verkäufers aufgerufen</strong></td> 
   <td>Telefonnummer, die vom Vertrieb aufgerufen wird.</td> 
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
   <td>Wenn die Quelle Tout ist, ist die Vorlagen-ID die Marketo Sales Connect-Vorlagen-ID. Verwenden Sie diese Option, um eine bestimmte Vorlage anstelle einer Betreffzeile Zielgruppe, die in mehreren Vorlagen vorhanden sein könnte.
</td> 
  </tr> 
 </tbody> 
</table>
