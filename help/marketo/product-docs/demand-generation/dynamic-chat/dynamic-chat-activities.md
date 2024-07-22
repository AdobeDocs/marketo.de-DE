---
description: Dynamic Chat-Aktivitäten - Marketo Docs - Produktdokumentation
title: Dynamische Chat-Aktivitäten
feature: Dynamic Chat
exl-id: ef3bb1a3-6758-4798-92eb-fef28a5ff9c7
source-git-commit: 79b439a9bb3d3cd130eb5a7b52cea13988e7b88e
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 6%

---

# Dynamische Chat-Aktivitäten {#dynamic-chat-activities}

Dynamic Chat bietet mehrere Filter und Trigger zur Verwendung in Ihren Smart-Listen.

![](assets/dynamic-chat-activities-1.png)

## Definitionen {#definitions}

<table>
<thead>
<tbody>
  <tr>
    <td style="width:25%"><b>Ausgelöst</b></td>
    <td>Ein Trigger-Ereignis tritt auf, wenn ein Besucher die Targeting-Kriterien für ein Dialogfeld oder einen Konversationsfluss erfüllt und das Dialogfeld angezeigt wird.
    <br>Ein Besucherereignis pro Trigger und Sitzung.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Eingebunden in einen Konversationsfluss/-dialog</b></td>
    <td>Eine Interaktion tritt auf, wenn ein Webbesucher zum ersten Mal in einem Dialogfeld oder einem Konversationsfluss auf eine Eingabeaufforderung klickt (Klicken auf eine Multiple-Choice-Option, Senden von Informationen, Buchung eines Meetings, Öffnen eines Dokuments usw.). Wenn ein Besucher ein Dialogfeld oder einen Konversionsfluss öffnet, aber nicht auf eine Eingabeaufforderung klickt, wird die Interaktion <b>nicht</b> protokolliert. 
    <br>Ein Interaktionsereignis pro Besucher und Sitzung.</td>
  </tr>
   <tr>
    <td style="width:25%"><b>Involviert mit einem Support-Mitarbeitenden</b></td>
    <td>Tritt auf, wenn ein Besucher erfolgreich mit einem Live-Chat-Agenten verbunden ist.
    <br>Pro Besucher und Sitzung mit dem Agentenereignis interagiert.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Hat mit Dokument interagiert</b></td>
    <td>Wird ausgelöst, wenn ein Besucher auf ein Dokument in einer Dokumentkarte klickt.
    <br>Es kann mehrere Dokumentinteraktionen pro Besucher und Sitzung geben.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Erreichte Ziele</b></td>
    <td>Tritt auf, wenn ein Besucher ein Ziel erreicht. <br>Es kann mehrere zielerreichte Ereignisse pro Besucher und Sitzung geben.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Geplante Besprechung</b></td>
    <td>Tritt auf, wenn ein Besucher ein Treffen mit einem Dynamic Chat-Agenten bucht.
    <br>Pro Besucher und Sitzung kann es mehrere durch Besprechungen gebuchte Ereignisse geben.</td>
  </tr>
</tbody>
</table>

## Zu beachten {#things-to-note}

* Bedingungen werden in Dynamic Chat-Flussschritten unterstützt
* Dynamic Chat-Aktivitäten können mit [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target="_blank"} synchronisiert werden.
* Sie können einzelne Dynamic Chat-Aktivitäten im Aktivitätsprotokoll eines Personendatensatzes anzeigen
