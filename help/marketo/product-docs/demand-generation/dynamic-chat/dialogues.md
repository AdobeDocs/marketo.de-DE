---
description: Dialogfelder - Marketo-Dokumente - Produktdokumentation
title: Dialogfelder
hide: true
hidefromtoc: true
source-git-commit: 8252a1a7cb32227eeae754e37386d975c4ed8884
workflow-type: tm+mt
source-wordcount: '752'
ht-degree: 1%

---

# Dialogfelder {#dialogues}

Dialoge sind individuelle Chatunterhaltungen. Erfahren Sie, wie Sie sie visuell anpassen, bestimmen, auf welchen Seiten sie erscheinen, und entscheiden, was gesagt wird und wer sie sieht.

## Neues Dialogfeld erstellen {#create-a-new-dialogue}

1. Klicken Sie auf **Dialogfelder**.

   ![](assets/dialogues-1.png)

1. Klicken Sie auf die Schaltfläche **Neu erstellen** .

   ![](assets/dialogues-2.png)

1. Geben Sie einen Namen ein (Beschreibung ist optional), legen Sie die Prioritätsstufe fest und klicken Sie auf **Speichern**.

   ![](assets/dialogues-3.png)

>[!NOTE]
>
>Die Prioritätsstufe bestimmt, wo das Dialogfeld in Ihrer Liste angezeigt wird (z. B.: Priorität 1 bedeutet, dass sie ganz oben steht).

## Zielgruppenkriterien {#audience-criteria}

Ähnlich wie bei Smart-Lists in Marketo ermöglichen Ihnen Zielgruppenkriterien-Attribute die Definition Ihrer Zielgruppe. Sie können bekannte oder unbekannte Leads mit abgeleiteten, Lead- oder Unternehmensattributen (oder einer Kombination daraus) als Ziel auswählen.

**Bekannte Leads**

Es gibt _viele_ Attributkombinationen, aus denen Sie auswählen können. In diesem Beispiel richten wir uns an alle **bekannten Leads** in Kalifornien, die in einem Unternehmen mit mehr als 50 Mitarbeitern arbeiten.

1. Ziehen Sie das Attribut **Lead-Status** und ziehen Sie es nach rechts.

   ![](assets/dialogues-4.png)

1. __ Die Liste wird standardmäßig festgelegt. Geben Sie im Feld Werte auswählen eine Zertifizierungsstelle ein (Sie können auch auf die Dropdown-Liste klicken und aus der Liste auswählen).

   ![](assets/dialogues-5.png)

1. Ziehen Sie das Attribut **Unternehmensgröße** und ziehen Sie es an die Stelle, an der _steht. Ziehen Sie ein Attribut hierher_.

   ![](assets/dialogues-6.png)

   >[!NOTE]
   >
   >Sie können auch ein Attribut auswählen, indem Sie auf das Symbol **+** klicken.

1. Klicken Sie auf das Dropdown-Menü für den Operator und wählen Sie **Größer als** aus.

   ![](assets/dialogues-7.png)

1. Geben Sie 50 ein und klicken Sie auf eine andere Stelle auf dem Bildschirm, um zu speichern.

   ![](assets/dialogues-8.png)

**Anonyme Leads**

Es gibt eine einfache Möglichkeit, Leads gezielt anzusprechen, die noch nicht in Ihrer Datenbank sind. In diesem Beispiel richten wir uns an alle **anonymen Leads**, die sich im Raum New York befinden.

1. Ziehen Sie das Attribut **Lead-E-Mail** und ziehen Sie es nach rechts.

   ![](assets/dialogues-9.png)

1. Klicken Sie auf das Dropdown-Menü für den Operator und wählen Sie **Ist leer** aus.

   ![](assets/dialogues-10.png)

1. Ziehen Sie das Attribut **Inferred State** und ziehen Sie es an die Stelle, an der _steht. Ziehen Sie ein Attribut hierher_.

   ![](assets/dialogues-11.png)

   >[!NOTE]
   >
   >Wenn ein Besucher Ihre Website besucht, werden diese von [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) Cookies gesetzt und in das System eingefügt. Wir schauen ihre IP in einer speziellen Datenbank nach und schließen alle möglichen guten Informationen.

1. __ Die Liste wird standardmäßig festgelegt. Geben Sie im Feld Werte auswählen NY ein (Sie können auch auf die Dropdown-Liste klicken und aus der Liste auswählen).

   ![](assets/dialogues-12.png)

## Gruppen hinzufügen {#add-groups}

Sie haben auch die Möglichkeit, Attribute zu gruppieren, falls Sie alle Attribute zusammen mit &quot;beliebig&quot;eines anderen Attributs haben möchten.

ABSCHLIESSEN

## Ziel {#target}

Hier geben Sie die URL(s) ein, für die ein bestimmtes Dialogfeld angezeigt werden soll.

Zulässige Formate:

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>Die Verwendung eines Sternchens dient als Platzhalter. `https://*.website.com` würde also den Dialog auf jeder Seite der Site platzieren, einschließlich Subdomains (z. B.: `support.website.com`). Und `https://website.com/folder/*` würde das Dialogfeld auf jede HTML-Seite im nachfolgenden Ordner platzieren (z. B.: Nehmen wir in diesem Fall an, der Ordner ist &quot;Sport&quot;, also: website.com/sports/baseball.html, website.com/sports/football.html usw.).

## Stream-Designer {#stream-designer}

Der Stream-Designer enthält verschiedene Karten, die Sie hinzufügen können, um die Chat-Konversation zu gestalten.

<table>
 <tr>
  <td><strong>Nachricht</strong></td>
  <td>Verwenden Sie diese Option, wenn Sie eine Anweisung ohne Antwort erstellen möchten (z. B.: "Hallo! Mit dem Code SAVE25" sind alle Artikel heute um 25 % billiger.
</td>
 </tr>
 <tr>
  <td><strong>Frage</strong></td>
  <td>Verwenden Sie diese Option, wenn Sie eine Multiple-Choice-Frage stellen möchten, von der Sie die verfügbaren Antworten bereitstellen (z. B.: An welcher Art von Fahrzeug interessiert Sie sich? Antworten = SUV, Compact, Truck usw.).</td>
 </tr>
 <tr>
  <td><strong>Informationserfassung</strong></td>
  <td>Verwenden Sie diese Option, wenn Sie Informationen erfassen möchten. Die drei Felder, aus denen Sie wählen können, sind E-Mail-Adresse, Telefonnummer und Text (mit denen der Besucher eine eigene Nachricht schreiben kann).</td>
 </tr>
 <tr>
  <td><strong>Zeitplan für die Ernennung</strong></td>
  <td>Bietet dem Besucher einen Kalender der verfügbaren Daten, um eine Weiterverfolgung zu planen. Die Kalenderverfügbarkeit spiegelt [den nächsten Agenten in der Zeile](/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing) wider.</td>
 </tr>
 <tr>
  <td><strong>Ziel</strong></td>
  <td>Dies ist die einzige Karte, die die Besucher nicht sehen werden. Es liegt an Ihnen zu bestimmen, an welchem Punkt ein Ziel innerhalb des spezifischen Chat erreicht wird (z. B.: Wenn das Sammeln der E-Mail des Besuchers Ihr Ziel ist, platzieren Sie die Zielkarte nach "Informationserfassung"im Stream).</td>
 </tr>
</table>

**Erstellen eines Streams**

Es müssen _viele_ Stream-Kombinationen erstellt werden. In diesem Beispiel stellen wir eine Ja- oder Nein-Frage und bereiten einige Antworten vor.

Beispiel

## Berichte {#reports}

Im Tab Berichte können Sie Daten aus den letzten 90 Tagen anzeigen. Jede Kategorie wird unten definiert.

<table>
 <tr>
  <td><strong>Ausgelöste Gesamtzahl</strong></td>
  <td>Wird jedes Mal erhöht, wenn sich ein Besucher für ein Dialogfeld qualifiziert/angezeigt wird.
</td>
 </tr>
 <tr>
  <td><strong>Eingebunden</strong></td>
  <td>Wird jedes Mal erhöht, wenn ein Besucher auf den Chatbot-Anker klickt, um das Dialogfeld zu öffnen.</td>
 </tr>
 <tr>
  <td><strong>Abgeschlossen</strong></td>
  <td>Wird jedes Mal erhöht, wenn ein Besucher das Ende einer Verzweigung in einem Dialogfeld erreicht.</td>
 </tr>
 <tr>
  <td><strong>Erfasste Leads</strong></td>
  <td>Wird jedes Mal erhöht, wenn ein Besucher eine gültige E-Mail-Adresse in einem Dialogfluss bereitstellt.</td>
 </tr>
 <tr>
  <td><strong>Eingeschlossene Sitzungen</strong></td>
  <td>Wird jedes Mal erhöht, wenn ein Besucher einen Termin erfolgreich über den Chatbot einplant.</td>
 </tr>
 <tr>
  <td><strong>Erreichte Ziele</strong></td>
  <td>Wird jedes Mal erhöht, wenn ein Besucher in einem beliebigen Dialogfluss ein Ziel erreicht.</td>
 </tr>
</table>
