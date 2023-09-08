---
description: Chatbot-Verhalten - Marketo-Dokumente - Produktdokumentation
title: Chatbot-Verhalten
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: ea9e02d9ad52991757f137c7c2b549b98f139ba5
workflow-type: tm+mt
source-wordcount: '1569'
ht-degree: 0%

---

# Chatbot-Verhalten {#chatbot-behavior}

Im Folgenden finden Sie verschiedene mögliche Szenarien, in denen das erwartete Verhalten des Chatbot für den Besucher in jedem Fall dargestellt wird.

<table>
  <tbody>
    <tr>
      <th>Abkürzung</th>
      <th>Details</th>
    </tr>
    <tr>
      <td>D1, D2, D3 usw.</td>
      <td>Stellt mehrere Dialogfelder dar, in denen D1 Dialogfeldname eins ist</td>
    </tr>
    <tr>
      <td>P1, P2, P3 usw.</td>
      <td>Stellt Dialogprioritäten dar, bei denen P1 die höchste Priorität hat</td>
    </tr>
    <tr>
      <td>WP1, WP2, WP3 usw.</td>
      <td>Stellt mehrere Webseiten dar, bei denen WP1 die erste Webseite ist</td>
    </tr>
    <tr>
      <td>V1, V2, V3 usw.</td>
      <td>Stellt mehrere Webseitenbesucher dar, bei denen V1 Besucher ist.</td>
    </tr>
   </tbody>
</table>

## Szenarien {#scenarios}

<table>
  <tr>
      <th>Szenario</th>
      <th>Erwartetes Chatbot-Verhalten</th>
      <th>Backend-Aktion</th>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>V1 besucht WP1</p>
      </td>
      <td>
        <p>D1 wird in V1 aufgelöst</p>
      </td>
      <td>Die Anzahl der Trigger für D1 wird um 1 erhöht</td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>V1 besucht WP1</p>
        <p>V1 aktualisiert WP1</p>
      </td>
      <td>
        <p>D1 wird in V1 aufgelöst</p>
        <p>Nach der Aktualisierung wird D1 erneut aufgelöst</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger für D1 wird um 1 erhöht</p>
        <p>Nach der Aktualisierung keine Änderung am D1-Trigger oder an der Interaktionsanzahl</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1, reagiert jedoch nicht</p>
      </td>
      <td>D1 wird in V1 aufgelöst</td>
      <td>
        <p>Die Anzahl der Trigger für D1 wird um 1 erhöht</p>
        <p>Keine Änderung an der Anzahl der Interaktionen in D1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1 und liefert die erste Antwort</p>
      </td>
      <td>D1 wird in V1 aufgelöst</td>
      <td>
        <p>Die Anzahl der Trigger für D1 wird um 1 erhöht</p>
        <p>Die Interaktionsanzahl für D1 wird um 1 erhöht</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1 und liefert die erste Antwort</p>
        <p>V1 aktualisiert WP1</p>
      </td>
      <td>
        <p>D1 wird in V1 aufgelöst</p>
        <p>Nach der Aktualisierung wird D1 fortgesetzt</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger und Interaktionen für D1 werden um 1 erhöht</p>
        <p>Nach der Aktualisierung wird keine Anzahl geändert</p>
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
        <p>D1 wird in V1 aufgelöst</p>
        <p>Nach der Aktualisierung wird kein Dialogfeld oder nächstes Dialogfeld für V1 aufgelöst</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger, der Interaktion und der Abgeschlossene Anzahl für D1 werden um 1 erhöht</p>
        <p>Nach der Aktualisierung wird kein Dialogfeld oder nächstes Dialogfeld aufgelöst</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1, WP2</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1, reagiert jedoch nicht</p>
        <p>V1 besucht WP2</p>
      </td>
      <td>
        <p>Seitenbesuch WP1, D1 wird in V1 aufgelöst</p>
        <p>Seitenbesuch WP2, D1 wird auf V2 aufgelöst</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger für D1 wird um 1 erhöht</p>
        <p>In WP2 keine Änderung an der Anzahl der D1-Trigger</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1, WP2</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1 und interagiert</p>
        <p>V1 besucht WP2</p>
      </td>
      <td>
        <p>Seitenbesuch WP1, D1 wird in V1 aufgelöst</p>
        <p>Seitenbesuch WP2, D1 wird in V1 aufgelöst</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger und Interaktionen für D1 werden um 1 erhöht</p>
        <p>In WP2 keine Änderung an der Anzahl</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>D2 nur für WP2</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1 und liefert die erste Antwort</p>
        <p>V1 besucht WP2</p>
      </td>
      <td>
        <p>D1 wird auf WP1 aufgelöst</p>
        <p>D1 wird weiterhin V1 auf WP2</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger und Interaktionen für D1 werden um 1 erhöht</p>
        <p>Keine Änderung an D2-Trigger oder Interaktionsanzahl</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>D2 nur für WP2</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1, reagiert jedoch nicht</p>
        <p>V1 besucht WP2</p>
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
        <p>V1 besucht WP2</p>
      </td>
      <td>D1 wird auf WP1 und nach Abschluss aufgelöst<br/>D2 wird auf WP2 aufgelöst</td>
      <td>
        <p>Die Anzahl der Trigger, der Interaktion und der Abgeschlossene Anzahl für D1 werden um 1 erhöht</p>
        <p>Die Anzahl der Trigger für D2 wird um 1 erhöht</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>D2 nur für WP2</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1 und schließt D1 ab</p>
        <p>V1 besucht WP2</p>
        <p>V1-Klicks auf D2 liefern die erste Antwort</p>
      </td>
      <td>D1 wird auf WP1 und nach Abschluss aufgelöst<br/>D2 wird auf WP2 aufgelöst</td>
      <td>
        <p>Die Anzahl der Trigger, der Interaktion und der Abgeschlossene Anzahl für D1 werden um 1 erhöht</p>
        <p>Trigger und Interaktionsanzahl für D2 werden um 1 erhöht</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1, reagiert jedoch nicht</p>
        <p>D1 ist unveröffentlicht</p>
      </td>
      <td>D1 wird in V1 aufgelöst</td>
      <td>
        <p>Die Anzahl der Trigger für D1 wird um 1 erhöht</p>
        <p>Keine Änderung an der Anzahl der D1-Interaktionen</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1, reagiert jedoch nicht</p>
        <p>D1 ist unveröffentlicht</p>
        <p>V1 aktualisiert WP1</p>
      </td>
      <td>
        <p>D1 wird zum ersten Mal in V1 aufgelöst</p>
        <p>Nach der Aktualisierung wird kein Dialogfeld aufgelöst</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger für D1 wird um 1 erhöht</p>
        <p>Keine Änderung an der Anzahl der D1-Interaktionen</p>
        <p>Nach der Aktualisierung keine Änderung am D1-Trigger oder an der Interaktionsanzahl</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 mit D1</p>
        <p>D1 ist unveröffentlicht</p>
        <p>V1 aktualisiert WP1</p>
      </td>
      <td>
        <p>D1 wird in V1 aufgelöst</p>
        <p>Nach der Aktualisierung wird D1 fortgesetzt</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger für D1 wird um 1 erhöht</p>
        <p>Die Anzahl der Interaktionen mit D1 wird um 1 erhöht</p>
        <p>Nach der Aktualisierung wird D1 weiterhin unverändert an der Trigger- oder Interaktionsanzahl angepasst.</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1, reagiert jedoch nicht</p>
        <p>D1 wird mit neuen Änderungen veröffentlicht</p>
        <p>V1 aktualisiert WP1</p>
      </td>
      <td>
        <p>D1 wird zum ersten Mal in V1 aufgelöst</p>
        <p>Nach der Aktualisierung wird das Dialogfeld mit neuen Änderungen aufgelöst</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger für D1 wird um 1 erhöht</p>
        <p>Nach der Aktualisierung, da D1 neue Änderungen enthält, aber keine weitere Änderung an der Anzahl der Trigger</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1-Klicks auf D1 liefern die erste Antwort</p>
        <p>D1 wird mit neuen Änderungen veröffentlicht</p>
        <p>V1 aktualisiert WP1</p>
      </td>
      <td>
        <p>D1 wird zum ersten Mal in V1 aufgelöst</p>
        <p>Nach der Aktualisierung wird das Dialogfeld mit alten Änderungen fortgesetzt</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger für D1 wird um 1 erhöht</p>
        <p>Die Interaktionsanzahl für D1 wird um 1 erhöht</p>
        <p>Nach der Aktualisierung wird die alte D1 angezeigt, sodass keine Änderung an der Anzahl der Trigger erfolgt</p>
      </td>
    </tr>
    <tr>
     <td>
        <p>D1 für WP1 mit 1 Priorität</p>
        <p>D2 für WP1 mit 2 Priorität</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1, reagiert jedoch nicht</p>
        <p>D1 ist unveröffentlicht</p>
        <p>V1 aktualisiert WP1</p>
      </td>
      <td>
        <p>D1 wird zum ersten Mal in V1 aufgelöst</p>
        <p>Nach der Aktualisierung wird D2 in V1 aufgelöst</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger für D1 wird um 1 erhöht</p>
        <p>Nach der Aktualisierung wird die Anzahl der Trigger für D2 um 1 erhöht</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 für WP1 mit 1 Priorität</p>
        <p>D2 für WP1 mit 2 Priorität</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1 und schließt D1 ab</p>
        <p>V1 aktualisiert WP1 und sieht D2<br/>V1 klickt auf D2 und schließt D2 ab</p>
        <p>Marketingexperte haben Änderungen an D1 vorgenommen und erneut veröffentlicht.</p>
        <p>V1 aktualisiert WP1</p>
      </td>
      <td>
        <p>D1 wird zum ersten Mal in V1 aufgelöst</p>
        <p>Nach der Aktualisierung wird D2 in V1 aufgelöst</p>
        <p>Nach Abschluss von D1 und D2 wird D2 unabhängig von den Änderungen oder der erneuten Veröffentlichung von D1 nicht mehr in V1 angezeigt.</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger, der Interaktion und der Abgeschlossene Anzahl für D1 werden um 1 erhöht</p>
        <p>Nach Abschluss von D2 aktualisieren, keine Maßnahmen erforderlich</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 für WP1 mit dem Trigger "Besuchszeit pro Site"von 30 Sekunden</p>
        <p>V1 besucht WP1</p>
      </td>
      <td>
        <p>D1 wird zwar aufgelöst, aber nicht auf V1 ausgelöst</p>
        <p>Nach 30 Sekunden wird D1 angezeigt/auf V1 ausgelöst</p>
      </td>
      <td>Die Anzahl der Trigger für D1 wird nur nach mehr als 30 Sekunden, die auf einer Webseite verbracht werden, um 1 erhöht</td>
    </tr>
    <tr>
      <td>
        <p>D1 für WP1, WP2 mit dem Trigger "Time on page"von 30 Sekunden</p>
        <p>V1 besucht WP1, WP2</p>
      </td>
      <td>
        <p>D1 wird zwar aufgelöst, aber nicht auf V1 ausgelöst</p>
        <p>Nach 30 Sekunden wird D1 angezeigt/auf V1 ausgelöst</p>
      </td>
      <td>Die Anzahl der Trigger für D1 wird nur nach mehr als 30 Sekunden, die auf einer Webseite verbracht werden, um 1 erhöht</td>
    </tr>
    <tr>
      <td>
        <p>D1 für WP1 mit Trigger "Bildlaufprozentsatz"von 50</p>
        <p>V1 besucht WP1</p>
      </td>
      <td>
        <p>D1 wird zwar aufgelöst, aber nicht auf V1 ausgelöst</p>
        <p>Nach 50 % Bildlauf wird D1 angezeigt/ausgelöst auf V1</p>
      </td>
      <td>Die Anzahl der Trigger für D1 wird erst nach 50 % Bildlauf um 1 erhöht</td>
    </tr>
    <tr>
      <td>
        <p>D1, die für WP1 mit einer Priorität und dem Trigger "Besuchszeit pro Seite"mit 30 Sekunden bestimmt ist</p>
        <p>D2 für WP1 mit 2 Priorität und Ereignis "Seitenbildprozentsatz"von 50</p>
        <p>V1 besucht WP1, nachdem V1 WP2 nach 10 Sekunden besucht hat, besucht V1 WP1</p>
      </td>
      <td>
        <p>Auf WP1 wird D1 zwar aufgelöst, aber nicht auf V1 ausgelöst</p>
        <p>Auf WP2 wird D2 zwar aufgelöst, aber nicht auf V1 ausgelöst</p>
        <p>Auf WP1 wird D1 aufgelöst und nach 20 Sekunden wird D1 auf V1 ausgelöst</p>
      </td>
      <td>Die Anzahl der Trigger für D1 wird erst nach 30 Sekunden um 1 erhöht</td>
    </tr>
    <tr>
      <td>
        <p>D1 wurde für WP1 mit dem Trigger "Besuchszeit pro Site"von 1 Minute bestimmt</p>
        <p>V1 besucht WP1 für 1 Minute und wird D1 angezeigt, interagiert jedoch nicht</p>
        <p>V1 schließt WP1 und kehrt 2 Tage später zu WP1 zurück</p>
      </td>
      <td>
        <p>D1 wird V1 automatisch angezeigt, da sie die Trigger-Kriterien während der vorherigen Sitzung bereits erfüllt haben</p>
        <p>Dasselbe gilt für "Besuchszeit pro Seite"und "Prozentsatz für Seitenbildvorgänge"</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger für D1 wird um 1 erhöht</p>
        <p>Nach der Rückkehr keine Maßnahmen zu ergreifen</p>
      </td>
    </tr>
  </tbody>
</table>

