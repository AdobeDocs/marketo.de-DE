---
description: Dialogfelder - Marketo-Dokumente - Produktdokumentation
title: Dialogfelder
hide: true
hidefromtoc: true
source-git-commit: c6713c972603ab9528a66e908e47e4c187b86c0c
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 0%

---

# Dialogfelder {#dialogues}

Dialogfelder sind die spezifischen Chatunterhaltungen, die Sie einrichten. Sie können angepasst werden, indem Sie sehen, was gesagt wird und wer es sieht.

## Neues Dialogfeld erstellen {#create-a-new-dialogue}

1. Klicken Sie auf **Dialogfelder**.

PICC

1. Klicken Sie auf die Schaltfläche **Neu erstellen** .

PICC

1. Geben Sie einen Namen ein (Beschreibung ist optional), legen Sie die Prioritätsstufe fest und klicken Sie auf **Speichern**.

PICC

>[!NOTE]
>
>PRIORITÄTSEBENE ERKLÄREN

## Zielgruppenkriterien {#audience-criteria}

Ähnlich wie bei Smart-Lists in Marketo ermöglichen Ihnen Zielgruppenkriterien-Attribute die Definition Ihrer Zielgruppe.

Es gibt mehrere Attribute zur Auswahl. In diesem Beispiel richten wir uns an alle bekannten Leads in Kalifornien, die in einem Unternehmen mit mehr als 50 Mitarbeitern arbeiten.

1. Ziehen Sie das Attribut Lead-Status nach rechts.

PICC

1. __ Die Liste wird standardmäßig festgelegt. Geben Sie im Feld Werte auswählen eine Zertifizierungsstelle ein (Sie können auch auf die Dropdown-Liste klicken und aus der Liste auswählen).

PICC

1. Ziehen Sie das Attribut Unternehmensgröße nach rechts.

PICC

1. Klicken Sie auf das Dropdown-Menü für den Operator und wählen Sie Größer als aus.

PICC

1. Geben Sie 50 ein und klicken Sie auf eine andere Stelle auf dem Bildschirm, um zu speichern.

PICC

ERFASSEN VON ANON-LEADS

HINWEIS - Vielleicht wurde erwähnt, wie der Anwendungsfall von Werken/Anzeigen-Anon lautet, Lead-E-Mail ist leer

## Gruppen hinzufügen {#add-groups}

Sie haben auch die Möglichkeit, Attribute zu gruppieren, falls Sie alle Attribute zusammen mit &quot;beliebig&quot;eines anderen Attributs haben möchten.

ABSCHLIESSEN

## Ziel {#target}

Hier geben Sie die spezifischen URLs ein, für die ein bestimmtes Dialogfeld angezeigt werden soll.

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

TABELLE

Nachricht: Verwenden Sie diese Option, wenn Sie eine Anweisung ohne Antwort erstellen möchten (z. B.: &quot;Hallo! Mit dem Code SAVE25 sind alle Artikel heute um 25 % billiger.&quot;)

Frage: Verwenden Sie diese Option, wenn Sie eine Multiple-Choice-Frage stellen möchten, von der Sie die verfügbaren Antworten bereitstellen (z. B.: An welcher Art von Fahrzeug interessiert Sie sich? Antworten = SUV, Compact, Truck usw.)

Informationserfassung: Verwenden Sie diese Option, wenn Sie Informationen erfassen möchten. Die drei Felder, aus denen Sie wählen können, sind E-Mail-Adresse, Telefonnummer und Text (mit denen der Besucher eine eigene Nachricht schreiben kann).

Termin-Planung: Bietet dem Besucher einen Kalender der verfügbaren Daten, um eine Weiterverfolgung zu planen. Die Kalenderverfügbarkeit spiegelt [den nächsten Agenten in Zeile](help/marketo/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.md#routing) wider.

Ziel: Dies ist die einzige Karte, die die Besucher nicht sehen werden. Es liegt an Ihnen zu bestimmen, an welchem Punkt ein Ziel innerhalb des spezifischen Chat erreicht wird (z. B.: Wenn das Sammeln der E-Mail des Besuchers Ihr Ziel ist, platzieren Sie die Zielkarte nach &quot;Informationserfassung&quot;im Stream.)

MÖGLICHER EIGENER ABSCHNITT

BEISPIEL ANZEIGEN UNTEN