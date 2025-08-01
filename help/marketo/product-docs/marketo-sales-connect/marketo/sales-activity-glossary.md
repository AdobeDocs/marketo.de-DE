---
description: Glossar zur Vertriebsaktivität - Marketo-Dokumente - Produktdokumentation
title: Glossar zur Verkaufsaktivität
exl-id: c7805642-07b6-4697-9efe-5c673ae9ca53
feature: Marketo Sales Connect
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 7%

---

# Glossar zur Verkaufsaktivität {#sales-activity-glossary}

Wenn in Sales Connect ein Verkäufer: einen Lead zu einer Verkaufskadenz hinzufügt, ihm eine E-Mail sendet oder einen Aufruf zu einer Aktivität ausführt, wird dies unter dem Aktivitätsverlauf von Marketo protokolliert. Wenn der Lead mit E-Mails interagiert, werden außerdem Öffnungen, Klicks und Antworten protokolliert.

Die folgenden Aktivitäten werden von [!DNL Sales Connect] an Marketo protokolliert.

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
  <td>[!UICONTROL gesendet von]</td>
 </tr>
 <tr>
  <td>Quelle</td>
 </tr>
 <tr>
  <td>[!UICONTROL Vorlagenkennung]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Verkaufsvorlage] URL</td>
 </tr>
 <tr>
  <td>[!UICONTROL Verkaufskampagne] URL</td>
 </tr>
 <tr>
  <td>Name der [!UICONTROL -Verkaufsvorlage]</td>
 </tr>
 <tr>
  <td>[!UICONTROL E-Mail-Betreff]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Name der Verkaufskampagne]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Vertriebspersonen-ID]</td>
 </tr>
 <tr>
  <th rowspan="9"> Verkaufs-E-Mail öffnen</th>
  <td>[!UICONTROL gesendet von]</td>
 </tr>
 <tr>
  <td>Quelle</td>
 </tr>
 <tr>
  <td>[!UICONTROL Vorlagenkennung]</td>
 </tr>
 <tr>
  <td>[!UICONTROL URL der Verkaufsvorlage]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Verkaufskampagnen-URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Name der Verkaufsvorlage]</td>
 </tr>
 <tr>
  <td>[!UICONTROL E-Mail-Betreff]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Name der Verkaufskampagne]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Vertriebspersonen-ID]</td>
 </tr>
 <tr>
  <th rowspan="10">Verkaufs-E-Mail angeklickt</th>
  <td>[!UICONTROL Link]</td>
 </tr>
 <tr>
  <td>[!UICONTROL gesendet von]</td>
 </tr>
 <tr>
  <td>Quelle</td>
 </tr>
 <tr>
  <td>[!UICONTROL Vorlagenkennung]</td>
 </tr>
 <tr>
  <td>[!UICONTROL URL der Verkaufsvorlage]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Verkaufskampagnen-URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Name der Verkaufsvorlage]</td>
 </tr>
 <tr>
  <td>[!UICONTROL E-Mail-Betreff]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Name der Verkaufskampagne]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Vertriebspersonen-ID]</td>
 </tr>
<tr>
  <th rowspan="3">Hat auf Vertriebsemail geantwortet</th>
  <td>[!UICONTROL empfangen von]</td>
 </tr>
 <tr>
  <td>Quelle</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Vertriebspersonen-ID]</td>
 </tr>
 <tr>
  <th rowspan="11">Hat Verkaufsanruf empfangen</th>
  <td>[!UICONTROL Verkaufsaufruf von]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Verkaufsanrufstatus]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Verkaufs-Anrufbetreff]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Name der Verkaufskampagne]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Verkaufskampagnen-URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Telefonnummer des Verkaufs aufgerufen]</td>
 </tr>
 <tr>
  <td>Quelle</td>
 </tr>
 <tr>
  <td>[!UICONTROL Dauer der Verkaufsanrufe]</td>
 </tr>
 <tr>
  <td>[!UICONTROL URL zur Aufzeichnung von Verkaufsanrufen]</td>
 </tr>
  <tr>
  <td>[!UICONTROL Verkaufsanruf beantwortet von]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Vertriebspersonen-ID]</td>
 </tr>
 <tr>
  <th rowspan="6">Zur Verkaufskampagne hinzufügen</th>
  <td>[!UICONTROL Name der Verkaufskampagne]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Verkaufsanrufstatus]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Verkaufskampagnen-URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL gesendet von]</td>
 </tr>
 <tr>
  <td>Quelle</td>
 </tr>
 <tr>
  <td>[!UICONTROL Vertriebskampagnen-ID]</td>
 </tr>
 <tr>
  <th rowspan="6">Aus Verkaufskampagne entfernen</th>
  <td>[!UICONTROL Name der Verkaufskampagne]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Verkaufsanrufstatus]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Verkaufskampagnen-URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL gesendet von]</td>
 </tr>
 <tr>
  <td>Quelle</td>
 </tr>
 <tr>
  <td>[!UICONTROL Vertriebskampagnen-ID]</td>
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
   <td><strong>[!UICONTROL Details]</strong></td>
   <td>Details der Bounce-Fehlermeldung.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL E-Mail]</strong></td>
   <td>E-Mail-Adresse, die zurückkam.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Link]</strong></td>
   <td>Angeklickte URL.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Marketo Vertriebspersonen-ID]</strong></td>
   <td>Eindeutige ID für Personendatensatz in [!DNL Sales Connect].</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL empfangen von]</strong></td>
   <td>E-Mail-Adresse des Absenders der E-Mail.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Verkaufsanruf beantwortet von]</strong></td>
   <td>Name der Person, die den Anruf entgegengenommen hat.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Dauer der Verkaufsanrufe]</strong></td>
   <td>Länge des Aufrufs in Sekunden.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Verkaufsaufruf von]</strong></td>
   <td>E-Mail-Adresse des Verkäufers, der den Anruf getätigt hat.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL URL zur Aufzeichnung von Verkaufsanrufen]</strong></td>
   <td>URL der Anrufaufzeichnung.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Verkaufsanrufstatus]</strong></td>
   <td>Speichert den endgültigen Anrufstatus des Anrufs, der Folgendes umfasst: Abgeschlossen, keine Antwort, Abgebrochen, Fehlgeschlagen.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Verkaufs-Anrufbetreff]</strong></td>
   <td>Anrufergebnis, das von einem Verkaufsbenutzer in der Wählhilfe ausgewählt wird.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Vertriebskampagnen-ID]</strong></td>
   <td>Eindeutige ID für Verkaufskampagnen-Asset in [!DNL Sales Connect].</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Name der Verkaufskampagne]</strong></td>
   <td>Name der Verkaufskampagne.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Verkaufskampagnen-URL]</strong></td>
   <td>[!DNL Sales Connect] URL für die Verkaufskampagne.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL E-Mail-Betreff für Verkauf]</strong></td>
   <td>Betreffzeile der E-Mail, gefolgt von einer eindeutigen ID (z. B.: Meine Betreffzeile (MSC-12345678)</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Telefonnummer des Verkaufs aufgerufen]</strong></td>
   <td>Telefonnummer, die vom Vertrieb angerufen wurde.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Name der Verkaufsvorlage]</strong></td>
   <td>Name der E-Mail-Vorlage in [!DNL Sales Connect].</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL URL der Verkaufsvorlage]</strong></td>
   <td>[!DNL Sales Connect] URL für E-Mail-Vorlage.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL gesendet von]</strong></td>
   <td>E-Mail-Adresse des Absenders der E-Mail.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Source]</strong></td>
   <td>Source der Aktivität. Wird für [!DNL Sales Connect] Aktivitäten vor der Version vom Oktober 2021 als „Tout“ festgelegt. Wird nach der Version vom Oktober 2021 die „Sales App“ für [!DNL Sales Connect] Aktivitäten sein.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Vorlagenkennung]</strong></td>
   <td>Wenn die Quelle Tout ist, ist die Vorlagen-ID die [!DNL Marketo Sales Connect] Vorlagen-ID. Verwenden Sie diese Option, um eine bestimmte Vorlage anstelle der Betreffzeile auszuwählen, die in mehreren Vorlagen vorhanden sein könnte.
</td>
  </tr>
 </tbody>
</table>
