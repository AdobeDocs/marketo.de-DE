---
description: Dialogfelder - Marketo-Dokumente - Produktdokumentation
title: Dialogfelder
exl-id: 5ec17ad0-6d56-4c06-a6ac-4c5771b2d91d
source-git-commit: 8aaa6f5225f7965228c3472c0cf6beb2259f3642
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 1%

---

# Dialogfelder {#dialogues}

Dialoge sind individuelle Chatunterhaltungen. Erfahren Sie, wie Sie sie visuell anpassen, festlegen, auf welchen Seiten sie erscheinen, und entscheiden, was gesagt wird und wer sie sieht.

## Neues Dialogfeld erstellen {#create-a-new-dialogue}

1. Klicken **Dialogfelder**.

   ![](assets/dialogues-1.png)

1. Klicken Sie auf **Neu erstellen** Schaltfläche.

   ![](assets/dialogues-2.png)

1. Geben Sie einen Namen ein (Beschreibung ist optional), legen Sie die Prioritätsstufe fest und klicken Sie auf **Speichern**.

   ![](assets/dialogues-3.png)

>[!NOTE]
>
>Die Priorität bestimmt, welches Dialogfeld einem Besucher angezeigt wird, wenn er sich für mehrere Dialogfelder gleichzeitig qualifiziert.

## Zielgruppenkriterien {#audience-criteria}

Ähnlich wie bei Smart-Lists in Marketo ermöglichen Ihnen Zielgruppenkriterien-Attribute die Definition Ihrer Zielgruppe. Sie können bekannte oder unbekannte Personen mithilfe von Inferred, Person oder Unternehmensattributen (oder einer Kombination daraus) ansprechen.

**Bekannte Personen**

Es gibt _many_ Attributkombinationen zur Auswahl. In diesem Beispiel zielen wir auf alle **bekannte Personen** in Kalifornien, die in einem Unternehmen mit mehr als 50 Beschäftigten arbeiten.

1. Grab die **Bundesland** -Attribut fest und ziehen Sie es nach rechts.

   ![](assets/dialogues-4.png)

1. _Is_ ist standardmäßig festgelegt. Geben Sie im Feld Werte auswählen eine Zertifizierungsstelle ein (Sie können auch auf die Dropdown-Liste klicken und aus der Liste auswählen).

   ![](assets/dialogues-5.png)

1. Grab die **Firmengröße** Attribut hinzufügen und an die gewünschte Position ziehen _Attribut hier ziehen und ablegen_.

   ![](assets/dialogues-6.png)

   >[!NOTE]
   >
   >Sie können auch ein Attribut auswählen, indem Sie auf dessen **+** Symbol.

1. Klicken Sie auf die Dropdown-Liste Operator und wählen Sie **Größer als**.

   ![](assets/dialogues-7.png)

1. Geben Sie 50 ein und klicken Sie auf eine andere Stelle auf dem Bildschirm, um zu speichern.

   ![](assets/dialogues-8.png)

Und das ist es!

**Anonyme Personen**

Es gibt eine einfache Möglichkeit, Personen gezielt anzusprechen, die noch nicht in Ihrer Datenbank sind. In diesem Beispiel zielen wir auf alle **Anonyme Personen** befindet sich im Gebiet von New York.

1. Grab die **Personen-E-Mail** -Attribut fest und ziehen Sie es nach rechts.

   ![](assets/dialogues-9.png)

1. Klicken Sie auf die Dropdown-Liste Operator und wählen Sie **Ist leer**.

   ![](assets/dialogues-10.png)

1. Grab die **Inferated State** Attribut hinzufügen und an die gewünschte Position ziehen _Attribut hier ziehen und ablegen_.

   ![](assets/dialogues-11.png)

   >[!NOTE]
   >
   >Wenn jemand Ihre Website besucht, [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) Cookies und setzt sie in das System. Wir suchen ihre IP-Adresse in einer speziellen Datenbank und schließen alle möglichen guten Informationen.

1. _Is_ ist standardmäßig festgelegt. Geben Sie im Feld Werte auswählen NY ein (Sie können auch auf die Dropdown-Liste klicken und aus der Liste auswählen).

   ![](assets/dialogues-12.png)

## Gruppen hinzufügen {#add-groups}

Sie haben auch die Möglichkeit, Attribute zu gruppieren, falls Sie alle Attribute zusammen mit &quot;all&quot;oder &quot;any&quot;eines anderen Attributs haben möchten. Sie können mehrere Gruppen hinzufügen.

![](assets/dialogues-13.png)

![](assets/dialogues-14.png)

## Ziel {#target}

Hier geben Sie die URL(s) ein, für die ein bestimmtes Dialogfeld angezeigt werden soll.

Zulässige Formate:

* `http://website.com`
* `https://*.website.com`
* `http://website.com/folder/*`
* `https://*.website.com/folder/*`

>[!NOTE]
>
>Die Verwendung eines Sternchens dient als Platzhalter. Also `https://*.website.com` würde das Dialogfeld auf jeder Seite der Site platzieren, einschließlich Subdomains (z. B.: `support.website.com`). und `https://website.com/folder/*` würde das Dialogfeld auf jeder HTML-Seite im folgenden Ordner platzieren (z. B.: Nehmen wir in diesem Fall an, der Ordner ist &quot;Sport&quot;, also: website.com/sports/baseball.html, website.com/sports/football.html usw.).

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
  <td>Bietet dem Besucher einen Kalender der verfügbaren Daten, um eine Weiterverfolgung zu planen. Die Verfügbarkeit eines Kalenders spiegelt <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing">der nächste Agent in Zeilen</a>.</td>
 </tr>
 <tr>
  <td><strong>Ziel</strong></td>
  <td>Dies ist die einzige Karte, die die Besucher nicht sehen werden. Es liegt an Ihnen zu bestimmen, an welchem Punkt ein Ziel innerhalb des spezifischen Chat erreicht wird (z. B.: Wenn das Sammeln der E-Mail des Besuchers Ihr Ziel ist, platzieren Sie die Zielkarte unmittelbar nach der Informationserfassung im Stream.</td>
 </tr>
</table>

**Erstellen eines Streams**

Es gibt _many_ mögliche Stream-Kombinationen. Sehen wir uns ein Beispiel an [in diesem Artikel](/help/marketo/product-docs/demand-generation/dynamic-chat/create-a-stream.md).

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
  <td><strong>Erfasste Personen</strong></td>
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

>[!MORELIKETHIS]
>
>[Erstellen eines Streams](/help/marketo/product-docs/demand-generation/dynamic-chat/create-a-stream.md)
