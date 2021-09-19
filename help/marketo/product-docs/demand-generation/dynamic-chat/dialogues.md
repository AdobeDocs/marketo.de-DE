---
description: Dialogfelder - Marketo-Dokumente - Produktdokumentation
title: Dialogfelder
hide: true
hidefromtoc: true
source-git-commit: c46902686f1d5af63a51f5eaae2dc0e6afe99629
workflow-type: tm+mt
source-wordcount: '273'
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

Es gibt mehrere Attribute zur Auswahl. In diesem Beispiel wählen wir Lead State _is_ California und Company Size _ist größer als_ 50.

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
>Die Verwendung eines Sternchens dient als Platzhalter. `https://*.website.com` würde also den Dialog auf jede Seite der Site setzen, einschließlich Subdomains (z. B.: support.website.com). Und `https://website.com/folder/*` würde das Dialogfeld auf jede HTML-Seite im nachfolgenden Ordner platzieren (z. B.: Nehmen wir in diesem Fall an, der Ordner ist &quot;Sport&quot;, also: website.com/sports/baseball.html, website.com/sports/football.html usw.).
