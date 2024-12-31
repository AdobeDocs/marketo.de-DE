---
description: Chatbot-Verhalten - Marketo-Dokumente - Produktdokumentation
title: Chatbot-Verhalten
feature: Dynamic Chat
exl-id: e91e7981-6617-42fe-8120-a7311a99cdfb
source-git-commit: d88406c1f9d72c57a6d4f09934cbf685499ed198
workflow-type: tm+mt
source-wordcount: '1680'
ht-degree: 0%

---

# Chatbot-Verhalten {#chatbot-behavior}

Im Folgenden finden Sie verschiedene mögliche Szenarien, in denen das erwartete Verhalten des Chatbots für den Besucher in jedem Szenario dargestellt wird.

<table>
  <tbody>
    <tr>
      <th>Abkürzung</th>
      <th>Details</th>
    </tr>
    <tr>
      <td>D1, D2, D3 usw.</td>
      <td>Stellt mehrere Dialogfelder dar, wobei D1 Dialogfeld eins ist</td>
    </tr>
    <tr>
      <td>P1, P2, P3 usw.</td>
      <td>Stellt Dialogprioritäten dar, bei denen P1 die höchste Priorität ist</td>
    </tr>
    <tr>
      <td>WP1, WP2, WP3 usw.</td>
      <td>Stellt mehrere Web-Seiten dar, wobei WP1 die erste Web-Seite ist</td>
    </tr>
    <tr>
      <td>V1, V2, V3 usw.</td>
      <td>Stellt mehrere Web-Seitenbesucher dar, wobei V1 ein Besucher ist</td>
    </tr>
   </tbody>
</table>

## Szenarios {#scenarios}

<table>
  <tr>
      <th>Szenario</th>
      <th>Erwartetes Chatbot-Verhalten</th>
      <th>Backend-Aktion</th>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>V1-Besuche WP1</p>
      </td>
      <td>
        <p>D1 wird in V1 aufgelöst.</p>
      </td>
      <td>Die Anzahl der Trigger für D1 wird um 1 erhöht</td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>V1-Besuche WP1</p>
        <p>V1 aktualisiert WP1</p>
      </td>
      <td>
        <p>D1 wird in V1 aufgelöst.</p>
        <p>Nach der Aktualisierung wird D1 erneut aufgelöst.</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger für D1 wird um 1 erhöht</p>
        <p>Nach der Aktualisierung ändert sich weder der D1-Trigger noch die Interaktionsanzahl.</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1, hat jedoch nicht reagiert</p>
      </td>
      <td>D1 wird in V1 aufgelöst.</td>
      <td>
        <p>Die Anzahl der Trigger für D1 wird um 1 erhöht</p>
        <p>Keine Änderung der D1-Interaktionsanzahl</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1 und gibt die erste Antwort</p>
      </td>
      <td>D1 wird in V1 aufgelöst.</td>
      <td>
        <p>Die Anzahl der Trigger für D1 wird um 1 erhöht</p>
        <p>Die Interaktionsanzahl für D1 wird um 1 erhöht</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1 und gibt die erste Antwort</p>
        <p>V1 aktualisiert WP1</p>
      </td>
      <td>
        <p>D1 wird in V1 aufgelöst.</p>
        <p>Nach der Aktualisierung wird D1 fortgesetzt</p>
      </td>
      <td>
        <p>Anzahl der Trigger und Interaktionsanzahl für D1 werden um 1 erhöht</p>
        <p>Nach der Aktualisierung bleibt die Anzahl unverändert</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1, interagiert mit dem Chatbot und schließt D1 ab</p>
        <p>V1 aktualisiert WP1</p>
      </td>
      <td>
        <p>D1 wird in V1 aufgelöst.</p>
        <p>Nach der Aktualisierung wird kein Dialogfeld und kein nächstes Dialogfeld für V1 aufgelöst.</p>
      </td>
      <td>
        <p>Anzahl der Trigger, Interaktionsanzahl und abgeschlossene Anzahl für D1 werden um 1 erhöht</p>
        <p>Nach der Aktualisierung werden kein Dialogfeld und kein nächstes Dialogfeld aufgelöst.</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1, WP2</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1, hat jedoch nicht reagiert</p>
        <p>V1-Besuche WP2</p>
      </td>
      <td>
        <p>Seitenbesuch WP1, D1 wird zu V1 aufgelöst.</p>
        <p>Seitenbesuch WP2, D1 wird zu V2 aufgelöst.</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger für D1 wird um 1 erhöht</p>
        <p>In WP2, keine Änderung der D1 Trigger Anzahl</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1, WP2</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1 und ist eingeschaltet</p>
        <p>V1-Besuche WP2</p>
      </td>
      <td>
        <p>Seitenbesuch WP1, D1 wird zu V1 aufgelöst.</p>
        <p>Seitenbesuch WP2, D1 wird zu V1 aufgelöst.</p>
      </td>
      <td>
        <p>Anzahl der Trigger und Interaktionsanzahl für D1 werden um 1 erhöht</p>
        <p>In WP2 keine Änderung an einer Zählung</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>D2 nur für WP2</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1 und gibt die erste Antwort</p>
        <p>V1-Besuche WP2</p>
      </td>
      <td>
        <p>D1 wird auf WP1 aufgelöst</p>
        <p>D1 wird weiterhin V1 auf WP2</p>
      </td>
      <td>
        <p>Anzahl der Trigger und Interaktionsanzahl für D1 werden um 1 erhöht</p>
        <p>Keine Änderung an der Anzahl der D2-Trigger oder Interaktionen</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>D2 nur für WP2</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1, hat jedoch nicht reagiert</p>
        <p>V1-Besuche WP2</p>
      </td>
      <td>D1 wird auf WP1 aufgelöst<br/>
      D2 wird auf WP2 aufgelöst</td>
      <td>
        <p>Die Anzahl der Trigger für D1 wird um 1 erhöht</p>
        <p>Die Anzahl der Trigger für D2 wird um 1 erhöht</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>D2 nur für WP2</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1 und schließt D1 ab</p>
        <p>V1-Besuche WP2</p>
      </td>
      <td>D1 wird auf WP1 aufgelöst und bei <br/> Abschluss D2 wird auf WP2 aufgelöst</td>
      <td>
        <p>Anzahl der Trigger, Interaktionsanzahl und abgeschlossene Anzahl für D1 werden um 1 erhöht</p>
        <p>Die Anzahl der Trigger für D2 wird um 1 erhöht</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>D2 nur für WP2</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1 und schließt D1 ab</p>
        <p>V1-Besuche WP2</p>
        <p>Klicks von V1 auf D2 liefern die erste Antwort</p>
      </td>
      <td>D1 wird auf WP1 aufgelöst und bei <br/> Abschluss D2 wird auf WP2 aufgelöst</td>
      <td>
        <p>Anzahl der Trigger, Interaktionsanzahl und abgeschlossene Anzahl für D1 werden um 1 erhöht</p>
        <p>Die Anzahl der Trigger und Interaktionen für D2 wird um 1 erhöht</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1, hat jedoch nicht reagiert</p>
        <p>Veröffentlichung von D1 aufgehoben</p>
      </td>
      <td>D1 wird in V1 aufgelöst.</td>
      <td>
        <p>Die Anzahl der Trigger für D1 wird um 1 erhöht</p>
        <p>Keine Änderung der D1-Interaktionsanzahl</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1, hat jedoch nicht reagiert</p>
        <p>Veröffentlichung von D1 aufgehoben</p>
        <p>V1 aktualisiert WP1</p>
      </td>
      <td>
        <p>D1 wird erstmals in V1 aufgelöst.</p>
        <p>Nach der Aktualisierung wird kein Dialogfeld aufgelöst.</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger für D1 wird um 1 erhöht</p>
        <p>Keine Änderung der D1-Interaktionsanzahl</p>
        <p>Nach der Aktualisierung ändert sich weder der D1-Trigger noch die Interaktionsanzahl.</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 mit D1 in Eingriff</p>
        <p>Veröffentlichung von D1 aufgehoben</p>
        <p>V1 aktualisiert WP1</p>
      </td>
      <td>
        <p>D1 wird in V1 aufgelöst.</p>
        <p>Nach der Aktualisierung wird D1 fortgesetzt</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger für D1 wird um 1 erhöht</p>
        <p>D1-Interaktionsanzahl wird um 1 erhöht</p>
        <p>Nach der Aktualisierung wird D1 nicht mehr geändert, um die Trigger- oder Interaktionsanzahl zu ändern</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1, hat jedoch nicht reagiert</p>
        <p>D1 wird mit neuen Änderungen veröffentlicht</p>
        <p>V1 aktualisiert WP1</p>
      </td>
      <td>
        <p>D1 wird erstmals in V1 aufgelöst.</p>
        <p>Nach der Aktualisierung wird das Dialogfeld mit den neuen Änderungen aufgelöst.</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger für D1 wird um 1 erhöht</p>
        <p>Nach der Aktualisierung als D1 mit neuen Änderungen, aber keiner weiteren Änderung der Trigger-Anzahl</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>Klicks von V1 auf D1 liefern die erste Antwort</p>
        <p>D1 wird mit neuen Änderungen veröffentlicht</p>
        <p>V1 aktualisiert WP1</p>
      </td>
      <td>
        <p>D1 wird erstmals in V1 aufgelöst.</p>
        <p>Nach der Aktualisierung wird das Dialogfeld mit den alten Änderungen fortgesetzt</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger für D1 wird um 1 erhöht</p>
        <p>Die Interaktionsanzahl für D1 wird um 1 erhöht</p>
        <p>Nach dem Aktualisieren, da die alte D1 angezeigt wird, sodass keine Änderung an der Anzahl der Trigger</p>
      </td>
    </tr>
    <tr>
     <td>
        <p>D1 für WP1 mit 1 Priorität</p>
        <p>D2 für WP1 mit zwei Prioritäten</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1, hat jedoch nicht reagiert</p>
        <p>Veröffentlichung von D1 aufgehoben</p>
        <p>V1 aktualisiert WP1</p>
      </td>
      <td>
        <p>D1 wird erstmals in V1 aufgelöst.</p>
        <p>Nach der Aktualisierung wird D2 in V1 aufgelöst.</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger für D1 wird um 1 erhöht</p>
        <p>Nach der Aktualisierung wird die Trigger-Anzahl für D2 um 1 erhöht</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 für WP1 mit 1 Priorität</p>
        <p>D2 für WP1 mit zwei Prioritäten</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1 und schließt D1 ab</p>
        <p>V1 aktualisiert WP1 und zeigt D2<br/>V1 Klicks auf D2 und schließt D2 ab</p>
        <p>Marketer hat Änderungen an D1 vorgenommen und erneut veröffentlicht</p>
        <p>V1 aktualisiert WP1</p>
      </td>
      <td>
        <p>D1 wird erstmals in V1 aufgelöst.</p>
        <p>Nach der Aktualisierung wird D2 in V1 aufgelöst.</p>
        <p>Nach Abschluss von D1 und D2 wird D2 unabhängig von den Änderungen oder der erneuten Veröffentlichung von D1 nicht mehr in V1 angezeigt</p>
      </td>
      <td>
        <p>Anzahl der Trigger, Interaktionsanzahl und abgeschlossene Anzahl für D1 werden um 1 erhöht</p>
        <p>Nach Abschluss von D2 aktualisieren, keine Aktion erforderlich</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 für WP1 mit „Zeit vor Ort“-Trigger von 30 Sekunden</p>
        <p>V1-Besuche WP1</p>
      </td>
      <td>
        <p>D1 wird aufgelöst, aber nicht auf V1 ausgelöst</p>
        <p>Nach 30 Sekunden wird D1 angezeigt/ausgelöst, um V1</p>
      </td>
      <td>Die Anzahl der Trigger für D1 wird erst nach über 30 Sekunden auf der Web-Seite um 1 erhöht</td>
    </tr>
    <tr>
      <td>
        <p>D1 für WP1, WP2 mit „Zeit auf Seite“-Trigger von 30 Sekunden</p>
        <p>V1 Besuche WP1, WP2</p>
      </td>
      <td>
        <p>D1 wird aufgelöst, aber nicht auf V1 ausgelöst</p>
        <p>Nach 30 Sekunden wird D1 angezeigt/ausgelöst, um V1</p>
      </td>
      <td>Die Anzahl der Trigger für D1 wird erst nach über 30 Sekunden auf der Web-Seite um 1 erhöht</td>
    </tr>
    <tr>
      <td>
        <p>D1 für WP1 mit einem „Bildlaufprozentsatz“-Trigger von 50</p>
        <p>V1-Besuche WP1</p>
      </td>
      <td>
        <p>D1 wird aufgelöst, aber nicht auf V1 ausgelöst</p>
        <p>Nach 50 % Bildlauf wird D1 angezeigt/ausgelöst, um V1</p>
      </td>
      <td>Die Anzahl der Trigger für D1 wird erst nach dem Scrollen um 50 % erhöht</td>
    </tr>
    <tr>
      <td>
        <p>D1 für WP1 mit 1 Priorität und Ereignis „Zeit auf Seite“ Trigger von 30 Sekunden</p>
        <p>D2 ist für WP1 mit 2 Priorität und Ereignis „Seitenscroll-Prozentsatz“ von 50 vorgesehen</p>
        <p>V1 Besuche WP1, nach 10 Sekunden V1 Besuche WP2, V1 Besuche WP1</p>
      </td>
      <td>
        <p>Auf WP1 wird D1 aufgelöst, aber nicht auf V1 ausgelöst</p>
        <p>Auf WP2 wird D2 aufgelöst, aber nicht auf V1 ausgelöst</p>
        <p>Auf WP1 wird D1 aufgelöst und nach 20 Sekunden wird D1 auf V1 ausgelöst</p>
      </td>
      <td>Die Anzahl der Trigger für D1 wird erst nach 30 Sekunden um 1 erhöht</td>
    </tr>
    <tr>
      <td>
        <p>D1 für WP1 vorgesehen mit „Zeit vor Ort“-Trigger von 1 Minute</p>
        <p>V1 besucht WP1 für 1 Minute und wird als D1 angezeigt, greift aber nicht ein</p>
        <p>V1 schließt WP1 und kehrt 2 Tage später zu WP1 zurück</p>
      </td>
      <td>
        <p>D1 wird automatisch V1 angezeigt, da sie die Sitzungskriterien in der vorherigen Trigger bereits erfüllt haben</p>
        <p>Dieselbe Logik gilt für „Zeit auf Seite“ und „Seitenscrollprozentsatz“</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger für D1 wird um 1 erhöht</p>
        <p>Nach der Rückkehr sind keine Maßnahmen zu ergreifen</p>
      </td>
    </tr>
  </tbody>
</table>

## Echtzeit-Lead-Auflösung {#real-time-lead-resolution}

Während eines Gesprächs mit einem anonymen Lead und einer E-Mail-ID klären wir, ob ein bekannter Lead-Datensatz mit dieser E-Mail-ID vorhanden ist, und verwenden diesen Datensatz für die Personalisierung in Echtzeit. Wenn wir mehrere Datensätze finden, führen wir sie in Echtzeit zusammen. Dieses Verhalten ist sowohl für Dialogfelder als auch für Konversationsflüsse implementiert.
