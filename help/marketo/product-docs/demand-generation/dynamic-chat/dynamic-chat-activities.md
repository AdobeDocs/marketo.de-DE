---
description: Dynamic Chat-Aktivitäten - Marketo-Dokumente - Produktdokumentation
title: Dynamische Chat-Aktivitäten
feature: Dynamic Chat
exl-id: ef3bb1a3-6758-4798-92eb-fef28a5ff9c7
source-git-commit: 79b439a9bb3d3cd130eb5a7b52cea13988e7b88e
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 6%

---

# Dynamische Chat-Aktivitäten {#dynamic-chat-activities}

Dynamic Chat bietet mehrere Filter und Trigger zur Verwendung in Ihren Smart Lists.

![](assets/dynamic-chat-activities-1.png)

## Definitionen {#definitions}

<table>
<thead>
<tbody>
  <tr>
    <td style="width:25%"><b>Ausgelöst</b></td>
    <td>Ein Besucherereignis tritt ein, wenn ein Trigger die Zielgruppenkriterien für einen Dialog oder einen Konversationsfluss erfüllt und das Dialogfeld angezeigt wird.
    <br>Ein Besucherereignis pro Trigger und Sitzung.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Interagiert mit einem Gesprächsfluss/-dialog</b></td>
    <td>Eine Interaktion findet statt, wenn ein Web-Besucher zum ersten Mal in einem Dialogfeld oder einem Gesprächsfluss auf eine Eingabeaufforderung klickt (Klick auf eine Multiple-Choice-Option, Senden von Informationen, Buchung eines Meetings, Öffnen eines Dokuments usw.). Wenn ein Besucher ein Dialogfeld oder einen Gesprächsfluss öffnet, aber nicht auf eine Eingabeaufforderung klickt, wird <b> Interaktion </b>. 
    <br>Ein Interaktionsereignis pro Besucher und Sitzung.</td>
  </tr>
   <tr>
    <td style="width:25%"><b>Involviert mit einem Support-Mitarbeitenden</b></td>
    <td>Tritt auf, wenn ein Besucher erfolgreich mit einem Live-Chat-Agenten verbunden ist.
    <br>Einer interagiert mit einem Agentenereignis pro Besucher und pro Sitzung.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Hat mit Dokument interagiert</b></td>
    <td>Tritt auf, wenn ein Besucher auf ein Dokument in einer Dokumentenkarte klickt.
    <br>Pro Besucher und Sitzung können mehrere Dokumenteninteraktionen stattfinden.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Ziel(e) erreicht</b></td>
    <td>Geschieht, wenn ein Besucher ein Ziel erreicht. <br>Pro Besucher und Sitzung können mehrere Ereignisse für das Erreichen des Ziels auftreten.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Geplante Besprechung</b></td>
    <td>Dies geschieht, wenn ein Besucher ein Meeting mit einem Dynamic Chat-Agenten bucht.
    <br>Pro Besucher und pro Sitzung können mehrere Veranstaltungen mit Besprechungsbuchung stattfinden.</td>
  </tr>
</tbody>
</table>

## Zu beachtende Punkte {#things-to-note}

* Bedingungen werden in Dynamic Chat-Flussschritten unterstützt
* Dynamic Chat-Aktivitäten können mit [Marketo Sales Insight synchronisiert werden](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target="_blank"}
* Einzelne Dynamic Chat-Aktivitäten können im Aktivitätsprotokoll eines Personendatensatzes angezeigt werden
