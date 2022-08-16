---
description: Chatbot-Verhalten - Marketo-Dokumente - Produktdokumentation
title: Chatbot-Verhalten
hide: true
hidefromtoc: true
exl-id: e91e7981-6617-42fe-8120-a7311a99cdfb
source-git-commit: 97b1a00b8ff1dc29a92687a70c71093fc8c04267
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
        <p>D1 sollte auf V1 aufgelöst werden </p>
      </td>
      <td>Die Anzahl der Trigger für D1 sollte um 1 erhöht werden</td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>V1 besucht WP1</p>
        <p>V1 aktualisiert WP1</p>
      </td>
      <td>
        <p>D1 sollte auf V1 aufgelöst werden</p>
        <p>Nach der Aktualisierung sollte D1 erneut aufgelöst werden</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger für D1 sollte um 1 erhöht werden</p>
        <p>Nach der Aktualisierung keine Änderung am D1-Trigger oder an der Interaktionsanzahl</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1, reagiert jedoch nicht</p>
      </td>
      <td>D1 sollte auf V1 aufgelöst werden</td>
      <td>
        <p>Die Anzahl der Trigger für D1 sollte um 1 erhöht werden</p>
        <p>Keine Änderung an der Anzahl der Interaktionen in D1</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1 und liefert die erste Antwort</p>
      </td>
      <td>D1 sollte auf V1 aufgelöst werden</td>
      <td>
        <p>Die Anzahl der Trigger für D1 sollte um 1 erhöht werden</p>
        <p>Die Interaktionsanzahl für D1 sollte um 1 erhöht werden</p>
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
        <p>D1 sollte auf V1 aufgelöst werden</p>
        <p>Nach der Aktualisierung sollte D1 fortgesetzt werden</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger und Interaktionen für D1 sollte um 1 erhöht werden</p>
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
        <p>D1 sollte auf V1 aufgelöst werden</p>
        <p>Nach der Aktualisierung sollte kein Dialogfeld oder nächstes Dialogfeld für V1 aufgelöst werden.</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger, Interaktionen und Abgeschlossene Anzahl für D1 sollte um 1 erhöht werden.</p>
        <p>Nach der Aktualisierung sollte kein Dialogfeld oder nächstes Dialogfeld aufgelöst werden</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1, WP2</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1, reagiert jedoch nicht </p>
        <p>V1 besucht WP2</p>
      </td>
      <td>
        <p>Seitenbesuch WP1, D1 sollte auf V1 aufgelöst werden</p>
        <p>Seitenbesuch WP2, D1 sollte auf V2 aufgelöst werden</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger für D1 sollte um 1 erhöht werden</p>
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
        <p>Seitenbesuch WP1, D1 sollte auf V1 aufgelöst werden</p>
        <p>Seitenbesuch WP2, D1 sollte auf V1 aufgelöst werden</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger und Interaktionen für D1 sollte um 1 erhöht werden</p>
        <p>In WP2 wird keine Anzahl geändert</p>
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
        <p>D1 sollte auf WP1 aufgelöst werden</p>
        <p>D1 sollte weiterhin V1 auf WP2 verwenden</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger und Interaktionen für D1 sollte um 1 erhöht werden</p>
        <p>Keine Änderung an D2-Trigger oder Interaktionsanzahl</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>D2 nur für WP2</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1, reagiert jedoch nicht </p>
        <p>V1 besucht WP2</p>
      </td>
      <td>D1 sollte auf WP1 aufgelöst werden<br/>
      D2 sollte auf WP2 aufgelöst werden</td>
      <td>
        <p>Die Anzahl der Trigger für D1 sollte um 1 erhöht werden</p>
        <p>Die Anzahl der Trigger für D2 sollte um 1 erhöht werden</p>
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
      <td>D1 sollte bei WP1 und nach der Fertigstellung aufgelöst werden<br/>D2 sollte auf WP2 aufgelöst werden</td>
      <td>
        <p>Die Anzahl der Trigger, Interaktionen und Abgeschlossene Anzahl für D1 sollte um 1 erhöht werden.</p>
        <p>Die Anzahl der Trigger für D2 sollte um 1 erhöht werden</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>D2 nur für WP2</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1 und schließt D1 ab</p>
        <p>V1 besucht WP2</p>
        <p>V1-Klicks auf D2 liefern die erste Antwort </p>
      </td>
      <td>D1 sollte bei WP1 und nach der Fertigstellung aufgelöst werden<br/>D2 sollte auf WP2 aufgelöst werden</td>
      <td>
        <p>Die Anzahl der Trigger, Interaktionen und Abgeschlossene Anzahl für D1 sollte um 1 erhöht werden.</p>
        <p>Trigger und Interaktionsanzahl für D2 sollten um 1 erhöht werden</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1, reagiert jedoch nicht</p>
        <p>D1 ist unveröffentlicht</p>
      </td>
      <td>D1 sollte auf V1 aufgelöst werden</td>
      <td>
        <p>Die Anzahl der Trigger für D1 sollte um 1 erhöht werden</p>
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
        <p>D1 sollte zum ersten Mal in V1 aufgelöst werden</p>
        <p>Nach der Aktualisierung sollte kein Dialogfeld aufgelöst werden</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger für D1 sollte um 1 erhöht werden</p>
        <p>Keine Änderung an der Anzahl der D1-Interaktionen</p>
        <p>Nach der Aktualisierung keine Änderung am D1-Trigger oder an der Interaktionsanzahl</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 nur für WP1</p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 mit D1 </p>
        <p>D1 ist unveröffentlicht</p>
        <p>V1 aktualisiert WP1</p>
      </td>
      <td>
        <p>D1 sollte auf V1 aufgelöst werden</p>
        <p>Nach der Aktualisierung sollte D1 fortgesetzt werden</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger für D1 sollte um 1 erhöht werden</p>
        <p>Die Anzahl der Interaktionen mit D1 sollte um 1 erhöht werden.</p>
        <p>Nach der Aktualisierung wird D1 weiter verwendet und ändert sich nicht mehr in die Trigger- oder Interaktionsanzahl.</p>
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
        <p>D1 sollte zum ersten Mal in V1 aufgelöst werden</p>
        <p>Nach der Aktualisierung sollte das Dialogfeld mit neuen Änderungen aufgelöst werden</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger für D1 sollte um 1 erhöht werden</p>
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
        <p>D1 sollte zum ersten Mal in V1 aufgelöst werden</p>
        <p>Nach der Aktualisierung sollte das Dialogfeld mit alten Änderungen fortgesetzt werden</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger für D1 sollte um 1 erhöht werden</p>
        <p>Die Interaktionsanzahl für D1 sollte um 1 erhöht werden </p>
        <p>Nach der Aktualisierung wird die alte D1 angezeigt, sodass keine Änderung an der Anzahl der Trigger vorgenommen wird.</p>
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
        <p>D1 sollte zum ersten Mal in V1 aufgelöst werden</p>
        <p>Nach der Aktualisierung sollte D2 auf V1 aufgelöst werden</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger für D1 sollte um 1 erhöht werden</p>
        <p>Nach der Aktualisierung sollte die Anzahl der Trigger für D2 um 1 erhöht werden</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 für WP1 mit 1 Priorität</p>
        <p>D2 für WP1 mit 2 Priorität </p>
        <p>V1 besucht WP1 zum ersten Mal</p>
        <p>V1 klickt auf D1 und schließt D1 ab</p>
        <p>V1 aktualisiert WP1 und sieht D2<br/>V1 klickt auf D2 und schließt D2 ab</p>
        <p>Marketingexperte haben Änderungen an D1 vorgenommen und erneut veröffentlicht.</p>
        <p>V1 aktualisiert WP1</p>
      </td>
      <td>
        <p>D1 sollte zum ersten Mal in V1 aufgelöst werden</p>
        <p>Nach der Aktualisierung sollte D2 auf V1 aufgelöst werden</p>
        <p>Nach Abschluss von D1 und D2 sollte D2 unabhängig von den Änderungen oder der erneuten Veröffentlichung von D1 nicht mehr in V1 angezeigt werden.</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger, Interaktionen und Abgeschlossene Anzahl für D1 sollte um 1 erhöht werden.</p>
        <p>Nach Abschluss von D2 aktualisieren, keine Maßnahmen erforderlich</p>
      </td>
    </tr>
    <tr>
      <td>
        <p>D1 für WP1 mit dem Trigger "Besuchszeit pro Site"von 30 Sekunden</p>
        <p>V1 besucht WP1</p>
      </td>
      <td>
        <p>D1 sollte aufgelöst werden, wird jedoch nicht auf V1 ausgelöst</p>
        <p>Nach 30 Sekunden sollte D1 auf V1 angezeigt/ausgelöst werden</p>
      </td>
      <td>Die Anzahl der Trigger für D1 sollte nur nach mehr als 30 Sekunden, die auf einer Webseite verbracht wurden, um 1 erhöht werden</td>
    </tr>
    <tr>
      <td>
        <p>D1 für WP1, WP2 mit dem Trigger "Time on page"von 30 Sekunden</p>
        <p>V1 besucht WP1, WP2</p>
      </td>
      <td>
        <p>D1 sollte aufgelöst werden, wird jedoch nicht auf V1 ausgelöst</p>
        <p>Nach 30 Sekunden sollte D1 auf V1 angezeigt/ausgelöst werden</p>
      </td>
      <td>Die Anzahl der Trigger für D1 sollte nur nach mehr als 30 Sekunden, die auf einer Webseite verbracht wurden, um 1 erhöht werden</td>
    </tr>
    <tr>
      <td>
        <p>D1 für WP1 mit Trigger "Bildlaufprozentsatz"von 50</p>
        <p>V1 besucht WP1</p>
      </td>
      <td>
        <p>D1 sollte aufgelöst werden, wird jedoch nicht auf V1 ausgelöst</p>
        <p>Nach einem 50%igen Bildlauf sollte D1 auf V1 angezeigt/ausgelöst werden</p>
      </td>
      <td>Die Anzahl der Trigger für D1 sollte nur nach 50 % Bildlauf um 1 erhöht werden</td>
    </tr>
    <tr>
      <td>
        <p>D1, die für WP1 mit einer Priorität und dem Trigger "Besuchszeit pro Seite"mit 30 Sekunden bestimmt ist</p>
        <p>D2 für WP1 mit 2 Priorität und Ereignis "Seitenscrollprozentsatz"von 50</p>
        <p>V1 besucht WP1, nachdem V1 WP2 nach 10 Sekunden besucht hat, besucht V1 WP1</p>
      </td>
      <td>
        <p>Auf WP1 sollte D1 aufgelöst werden, wird jedoch nicht auf V1 ausgelöst</p>
        <p>Auf WP2 sollte D2 aufgelöst werden, wird jedoch nicht auf V1 ausgelöst</p>
        <p>Auf WP1 sollte D1 aufgelöst und nach 20 Sekunden sollte D1 auf V1 ausgelöst werden</p>
      </td>
      <td>Die Anzahl der Trigger für D1 sollte nur nach 30 Sekunden um 1 erhöht werden</td>
    </tr>
    <tr>
      <td>
        <p>D1 wurde für WP1 mit dem Trigger "Besuchszeit pro Site"von 1 Minute bestimmt</p>
        <p>V1 besucht WP1 für 1 Minute und wird D1 angezeigt, interagiert jedoch nicht</p>
        <p>V1 schließt WP1 und kehrt 2 Tage später zu WP1 zurück</p>
      </td>
      <td>
        <p>D1 sollte V1 automatisch angezeigt werden, da sie die Trigger-Kriterien bereits während der vorherigen Sitzung erfüllt haben</p>
        <p>Dieselbe Logik sollte für "Besuchszeit pro Seite"und "Seitenbildprozentsatz"gelten</p>
      </td>
      <td>
        <p>Die Anzahl der Trigger für D1 sollte um 1 erhöht werden</p>
        <p>Nach der Rückkehr keine Maßnahmen erforderlich</p>
      </td>
    </tr>
  </tbody>
</table>
