---
unique-page-id: 2359414
description: Einfache Bewertung - Marketo-Dokumente - Produktdokumentation
title: Einfache Bewertung
exl-id: 6129d46a-e6d2-4819-9b6c-ccbf37060712
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 4%

---

# Einfache Bewertung {#simple-scoring}

>[!PREREQUISITES]
>
>* [Einrichten und Person hinzufügen](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [Landingpage mit einem Formular](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## Schritt 1: Bewertungskampagne erstellen {#step-create-a-scoring-campaign}

1. Navigieren Sie zum Bereich **[!UICONTROL Marketing]** Aktivitäten.

   ![](assets/simple-scoring-1.png)

1. Klicken Sie mit der rechten Maustaste auf **Ordner** Lernen) und klicken Sie auf **[!UICONTROL Neuer Kampagnenordner]**.

   ![](assets/simple-scoring-2.png)

1. Nennen Sie den Kampagnenordner Scoring und klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/simple-scoring-3.png)

   >[!NOTE]
   >
   >Wenn Sie bereits über einen Bewertungsordner verfügen, benennen Sie diesen Ordner anders, z. B. Bewertung 1. Ordnernamen müssen eindeutig sein.

1. Klicken Sie mit der rechten Maustaste auf **Ordner** Scoring“ und wählen Sie **[!UICONTROL Neue intelligente Kampagne]**.

   ![](assets/simple-scoring-4.png)

1. Nennen Sie die Kampagne „Ergebnis ändern“ und klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/simple-scoring-5.png)

1. Klicken Sie auf **[!UICONTROL Registerkarte]** Smart-Liste“.

   ![](assets/simple-scoring-6.png)

   Wir möchten, dass diese Kampagne immer dann ausgeführt wird, wenn eine Person Ihr **Testanfrageformular“**.

1. Suchen Sie den Trigger **[!UICONTROL Formular ausfüllen]** und ziehen Sie ihn auf die linke Arbeitsfläche.

   ![](assets/simple-scoring-7.png)

1. Wählen Sie **Mein Formular** aus.

   ![](assets/simple-scoring-8.png)

   >[!NOTE]
   >
   >Wenn Sie die [Landingpage mit einem Formular](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"} Quick Win ausgefüllt haben, sollten Sie das Formular verwenden. Wenn Sie einen anderen Namen für Ihr Formular verwendet haben, wählen Sie diesen aus.

1. Klicken Sie auf **[!UICONTROL Registerkarte]** Fluss“.

   ![](assets/simple-scoring-9.png)

1. Ziehen Sie **Flussaktion** Score ändern“ auf die linke Arbeitsfläche.

   ![](assets/simple-scoring-10.png)

1. Sie können einen beliebigen Wert eingeben, der zum Score der Person hinzugefügt werden soll. Geben wir &quot;+5“ in das Feld &quot;**[!UICONTROL &quot;]**.

   ![](assets/simple-scoring-11.png)

   >[!TIP]
   >
   >Gute Scoring-Kampagnen sind der Schlüssel zur Bereitstellung hochwertiger Mitarbeiter im Vertrieb. Lesen Sie [**Endgültige Anleitung zur Lead-Bewertung**](https://www.marketo.com/definitive-guides/lead-scoring/){target="_blank"}.

1. Klicken Sie auf die **[!UICONTROL Zeitplan]** und auf die Schaltfläche **[!UICONTROL Aktivieren]**.

   ![](assets/simple-scoring-12.png)

1. Klicken Sie **[!UICONTROL Bestätigungsbildschirm]** Aktivieren“.

   ![](assets/simple-scoring-13.png)

>[!NOTE]
>
>Nach der Aktivierung wird diese Kampagne jedes Mal ausgeführt, wenn eine Person das Formular ausfüllt. Die Kampagne wird weiter ausgeführt, bis sie deaktiviert wird.

## Schritt 2: Formular ausfüllen {#step-fill-out-the-form}

1. Wählen Sie die Landingpage aus, die Sie in der [Landingpage mit einem Formular](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"} Quick Win erstellt haben.

   ![](assets/simple-scoring-14.png)

1. Klicken Sie **[!UICONTROL Vorschau]**. Die Landingpage wird in einer neuen Registerkarte geöffnet.

   ![](assets/simple-scoring-15.png)

1. Füllen Sie das Formular mit Vorname, Nachname und E-Mail-Adresse aus und klicken Sie dann auf **[!UICONTROL Senden]**.

   ![](assets/simple-scoring-16.png)

   >[!NOTE]
   >
   >Verwenden Sie denselben Namen und dieselbe E-Mail-Adresse, die Sie bei der ersten Eingabe als Person verwendet haben, um die Punktzahl &quot;+5“ zu erhöhen.

## Schritt 3: Anzeigen der Personeninformationen {#step-view-the-person-info}

1. Wechseln Sie zum Bereich **[!UICONTROL Datenbank]**.

   ![](assets/simple-scoring-17.png)

1. Suchen Sie nach der E-Mail-Adresse, die Sie beim Ausfüllen des Formulars verwendet haben.

   ![](assets/simple-scoring-18.png)

1. Doppelklicken Sie auf Ihre Person.

   ![](assets/simple-scoring-19.png)

Ihre Personendaten werden in einer neuen Registerkarte oder einem neuen Fenster geöffnet. Sehen Sie, wie Ihr Punktestand beim Ausfüllen des Formulars um 5 Punkte gestiegen ist?

![](assets/simple-scoring-20.png)

## Mission abgeschlossen! {#mission-complete}

<br> 

[◄ Mission 2: Landingpage mit einem Formular](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

[Mission 4: E-Mail-►](/help/marketo/getting-started/quick-wins/email-auto-response.md)
