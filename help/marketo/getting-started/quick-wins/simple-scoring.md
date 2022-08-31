---
unique-page-id: 2359414
description: Einfache Bewertung - Marketo-Dokumente - Produktdokumentation
title: Einfache Bewertung
exl-id: 6129d46a-e6d2-4819-9b6c-ccbf37060712
source-git-commit: 10637f7853c5b0f8a076779d95b8163b2de8abcb
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 10%

---

# Einfache Bewertung {#simple-scoring}

>[!PREREQUISITES]
>
>* [Einrichten und Hinzufügen einer Person](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target=&quot;_blank&quot;}
>* [Landingpage mit einem Formular](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;}


## Schritt 1: Bewertungskampagne erstellen {#step-create-a-scoring-campaign}

1. Navigieren Sie zu **Marketingaktivitäten** Bereich.

   ![](assets/simple-scoring-1.png)

1. Rechtsklick auf Ihre **Lernen** Ordner und klicken Sie auf **Neuer Kampagnenordner**.

   ![](assets/simple-scoring-2.png)

1. Benennen Sie den Kampagnenordner &quot;Scoring&quot;und klicken Sie auf **Erstellen**.

   ![](assets/simple-scoring-3.png)

   >[!NOTE]
   >
   >Wenn Sie bereits über einen Scoring-Ordner verfügen, benennen Sie diesen etwas Anderes, z. B. Scoring 1. Ordnernamen müssen eindeutig sein.

1. Rechtsklick auf Ihre **Scoring** Ordner und wählen Sie **Neue intelligente Kampagne**.

   ![](assets/simple-scoring-4.png)

1. Benennen Sie die Kampagne &quot;Ergebnis ändern&quot;und klicken Sie auf **Erstellen**.

   ![](assets/simple-scoring-5.png)

1. Klicken Sie auf die Registerkarte **“Intelligente Liste“**.

   ![](assets/simple-scoring-6.png)

   Wir möchten, dass diese Kampagne ausgeführt wird, sobald eine Person Ihre **Testanfrageformular**.

1. Suchen und Ziehen **Formular ausfüllen** Trigger auf der linken Arbeitsfläche.

   ![](assets/simple-scoring-7.png)

1. Auswählen **Mein Formular**.

   ![](assets/simple-scoring-8.png)

   >[!NOTE]
   >
   >Wenn Sie die [Landingpage mit einem Formular](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;} Quick win, sollte das Formular vorhanden sein. Wenn Sie für Ihr Formular einen anderen Namen verwendet haben, wählen Sie diesen aus.

1. Klicken Sie auf die Registerkarte **“Flow“**.

   ![](assets/simple-scoring-9.png)

1. Ziehen Sie die **Bewertung ändern** Flussaktion auf die linke Arbeitsfläche.

   ![](assets/simple-scoring-10.png)

1. Sie können einen beliebigen Wert eingeben, der dem Ergebnis der Person hinzugefügt werden soll. Geben wir &quot;+5&quot;im **Änderung** -Feld.

   ![](assets/simple-scoring-11.png)

   >[!TIP]
   >
   >Gute Scoring-Kampagnen sind der Schlüssel zur Bereitstellung hochwertiger Mitarbeiter für den Vertrieb. Lesen [**Der endgültige Leitfaden für die Lead-Scoring**](https://www.marketo.com/definitive-guides/lead-scoring/){target=&quot;_blank&quot;}.

1. Klicken Sie auf **Zeitplan** und **Aktivieren** Schaltfläche.

   ![](assets/simple-scoring-12.png)

1. Klicken **Aktivieren** auf dem Bestätigungsbildschirm.

   ![](assets/simple-scoring-13.png)

>[!NOTE]
>
>Nach der Aktivierung wird diese Kampagne jedes Mal ausgeführt, wenn eine Person das Formular ausfüllt. Die Kampagne läuft so lange, bis sie deaktiviert wird.

## Schritt 2: Formular ausfüllen {#step-fill-out-the-form}

1. Wählen Sie die Landingpage aus, die Sie im [Landingpage mit einem Formular](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;} schneller Sieg.

   ![](assets/simple-scoring-14.png)

1. Klicken **Vorschau**. Die Landingpage wird in einem neuen Tab geöffnet.

   ![](assets/simple-scoring-15.png)

1. Füllen Sie das Formular mit Vorname, Nachname und E-Mail-Adresse aus und klicken Sie auf **Einsenden**.

   ![](assets/simple-scoring-16.png)

   >[!NOTE]
   >
   >Verwenden Sie denselben Namen und dieselbe E-Mail-Adresse, die Sie beim ersten Einstieg als Person verwendet haben, um die Erhöhung des Punktwerts &quot;+5&quot;anzuwenden.

## Schritt 3: Anzeigen der Personeninformationen {#step-view-the-person-info}

1. Wechseln Sie zum Bereich Datenbank .

   ![](assets/simple-scoring-17.png)

1. Suchen Sie nach der E-Mail-Adresse, die Sie beim Ausfüllen des Formulars verwendet haben.

   ![](assets/simple-scoring-18.png)

1. Doppelklicken Sie auf Ihre Person.

   ![](assets/simple-scoring-19.png)

Ihre Personendetails werden in einem neuen Tab oder Fenster geöffnet. Erfahren Sie, wie sich Ihr Ergebnis beim Ausfüllen des Formulars um 5 Punkte erhöht hat.

![](assets/simple-scoring-20.png)

## Aufgabe abgeschlossen! {#mission-complete}

<br> 

[◄ Aufgabe 2: Landing Page mit Formular](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

[Aufgabe 4: Automatische Antwort-E-Mail ►](/help/marketo/getting-started/quick-wins/email-auto-response.md)
