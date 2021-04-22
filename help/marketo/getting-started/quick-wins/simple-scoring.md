---
unique-page-id: 2359414
description: Einfache Bewertung - Marketo Docs - Produktdokumentation
title: Einfache Bewertung
exl-id: 6129d46a-e6d2-4819-9b6c-ccbf37060712
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 14%

---

# Einfache Bewertung {#simple-scoring}

>[!PREREQUISITES]
>
>* [Einrichten und Hinzufügen einer Person](get-set-up-and-add-a-person.md)
>* [Landing Page mit Formular](landing-page-with-a-form.md)


## Schritt 1: Bewertungskampagne erstellen {#step-create-a-scoring-campaign}

1. Gehen Sie zum Bereich **Marketing-Aktivitäten**.

   ![](assets/ma-1.png)

1. Klicken Sie mit der rechten Maustaste auf den Ordner **Lernen** und klicken Sie auf **Neuer Kampagnenordner**.

   ![](assets/two-2.png)

1. Benennen Sie den Ordner &quot;Kampagne&quot;als &quot;Punktzahl&quot;.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Wenn Sie bereits über einen Scoring-Ordner verfügen, geben Sie diesem einen anderen Namen, z. B. Scoring 1. Ordnernamen müssen eindeutig sein.

1. Klicken Sie dann mit der rechten Maustaste auf den neuen Ordner **Scoring** und wählen Sie **Neue Smart-Kampagne**.

   ![](assets/four.png)

1. **Benennen Sie** die Kampagne &quot;Change Score&quot;und klicken Sie auf  **Create**.

   ![](assets/five-1.png)

1. Klicken Sie auf die Registerkarte **“Intelligente Liste“**.

   ![](assets/six-1.png)

   Diese Kampagne soll immer dann ausgeführt werden, wenn ein Benutzer das **Testanforderungsformular** ausfüllt.

1. Suchen Sie den Trigger **Ausfüllen des Formulars** und ziehen Sie ihn auf die linke Arbeitsfläche.

   ![](assets/image2014-9-24-11-3a43-3a35.png)

1. Wählen Sie **Mein Formular**.

   >[!NOTE]
   >
   >Wenn Sie die [Landingpage mit einem Formular](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md) Quick win abgeschlossen haben, sollten Sie das Formular haben. Wenn Sie einen anderen Namen für Ihr Formular verwendet haben, wählen Sie diesen aus.

   ![](assets/image2014-9-24-11-3a44-3a16.png)

1. Klicken Sie auf die Registerkarte **“Flow“**.

   ![](assets/image2014-9-24-11-3a44-3a33.png)

1. Ziehen Sie die Aktion **Wert ändern** auf die linke Arbeitsfläche.

   ![](assets/image2014-9-24-11-3a44-3a45.png)

1. Sie können einen beliebigen Wert eingeben, der dem Ergebnis der Person hinzugefügt werden soll. Geben Sie &quot;+5&quot;in das Feld **Change** ein.

   ![](assets/eleven-1.png)

   >[!TIP]
   >
   >Gute Kampagnen sind der Schlüssel zur Bereitstellung hochwertiger Mitarbeiter für den Vertrieb. Lesen Sie [**Die ultimative Anleitung für die Lead-Bewertung**](https://www.marketo.com/definitive-guides/lead-scoring/).

1. Klicken Sie auf die Registerkarte **Plan** und auf die Schaltfläche **Aktivieren**.

   ![](assets/twelve-1.png)

1. Klicken Sie im Bestätigungsbildschirm auf **Aktivieren**.

   ![](assets/thirteen-1.png)

>[!NOTE]
>
>Sobald diese Kampagne aktiv ist, wird sie jedes Mal ausgeführt, wenn ein Benutzer das Formular ausfüllt. Die Kampagne läuft, bis sie deaktiviert ist.

## Schritt 2: Formular ausfüllen {#step-fill-out-the-form}

1. Wählen Sie die Landingpage aus, die Sie in der Landingpage [mit einem Formular](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md) Quick win erstellt haben.

   ![](assets/fourteen-1.png)

1. Klicken Sie auf **“Genehmigte Seite anzeigen“**. Die Landingpage wird in einer neuen Registerkarte geöffnet.

   ![](assets/image2014-9-24-11-3a47-3a51.png)

1. Füllen Sie das Formular mit Ihrem Vornamen, Nachnamen und Ihrer E-Mail-Adresse aus und klicken Sie dann auf **Senden**.

   ![](assets/image2014-9-24-11-3a47-3a59.png)

   >[!NOTE]
   >
   >Verwenden Sie denselben Namen und dieselbe E-Mail-Adresse, die Sie beim ersten Einstieg als Person verwendet haben, um die &quot;+5&quot;-Ergebniserhöhung anzuwenden.

## Schritt 3: Ansicht der Personeninfo {#step-view-the-person-info}

1. Wechseln Sie zum Bereich &quot;Datenbank&quot;.

   ![](assets/db-2.png)

1. Suchen Sie nach der E-Mail-Adresse, die Sie beim Ausfüllen des Formulars verwendet haben.

   ![](assets/eighteen.png)

1. Klicken Sie mit der Dublette auf Ihre Person.

   ![](assets/nineteen.png)

Ihre persönlichen Daten werden in einem neuen Register oder Fenster geöffnet. Sehen Sie, wie Ihr Ergebnis um 5 Punkte für das Ausfüllen des Formulars erhöht wurde!!

![](assets/twenty.png)

**Herzlichen Glückwunsch!** Sie haben eine bewertete Kampagne erstellt.
[◄ Aufgabe 2: Landing Page mit Formular](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

[Aufgabe 4: Automatische Antwort-E-Mail ►](/help/marketo/getting-started/quick-wins/email-auto-response.md)
