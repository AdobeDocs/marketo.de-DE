---
unique-page-id: 2359422
description: Personalisieren einer E-Mail - Marketo-Dokumente - Produktdokumentation
title: E-Mail personalisieren
exl-id: 1562796e-da47-4305-b950-3bed1d36d339
source-git-commit: 0da33dfa840dd1e5a5618fcd762b482f7a2e0789
workflow-type: tm+mt
source-wordcount: '345'
ht-degree: 8%

---

# E-Mail personalisieren {#personalize-an-email}

## Auftrag: Personalisieren von E-Mails durch Hinzufügen von Daten-Token {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [Einrichten und Hinzufügen einer Person](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target=&quot;_blank&quot;}
>* [E-Mail-Blast senden](/help/marketo/getting-started/quick-wins/send-an-email.md){target=&quot;_blank&quot;}
>* [Tropfen, Tropfen, Verdauung](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target=&quot;_blank&quot;}


## Schritt 1: E-Mail zum Personalisieren auswählen {#step-select-an-email-to-personalize}

1. Wählen Sie eine der E-Mails aus, die in der [vorheriger Schnellsieg](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target=&quot;_blank&quot;} und klicken Sie auf **Entwurf bearbeiten**.

   ![](assets/one-4.png)

   >[!NOTE]
   >
   >Damit wird eine Kopie der E-Mail als Entwurf erstellt. Sie müssen den Entwurf genehmigen, damit die Änderungen live geschaltet werden.

Wenn Sie einen Popup-Blocker nicht aktiviert haben, wird der E-Mail-Editor in einer neuen Registerkarte/einem neuen Fenster geöffnet. Klicken Sie andernfalls auf **Entwurf bearbeiten** zweimal.

## Schritt 2: Verkäufer zum Absender machen {#step-make-the-salesperson-the-sender}

1. Wählen Sie die **Von** Feld, Hervorhebung und **delete** den aktuellen Namen.

   ![](assets/two-5.png)

1. Klicken Sie auf **Token** rechts neben dem **Von** -Feld.

   ![](assets/three-4.png)

1. Suchen und Auswählen **`{{lead.Lead Owner First Name}}`** Token.

   ![](assets/four-3.png)

1. Geben Sie Ihren Firmennamen und einen Bindestrich für die **Standardwert** um sicherzustellen, dass etwas angezeigt wird, falls der Vorname des Verkaufsprotokolls nicht verfügbar ist. Klicken Sie auf **Einfügen**.

   ![](assets/five-4.png)

1. Drücken Sie die Leertaste im **Von** -Feld, um sicherzustellen, dass der Cursor ein Leerzeichen nach dem soeben eingefügten Token blinkt. Klicken Sie anschließend auf **Token** erneut.

   ![](assets/six-4.png)

1. Suchen und Auswählen **`{{lead.Lead Owner Last Name}}`** Token.

   ![](assets/seven-5.png)

1. Geben Sie &quot;Verkauf&quot;für die **Standardwert** und klicken Sie auf **Einfügen**.

   ![](assets/eight-3.png)

## Schritt 3: Fügen Sie den Namen des Leads zur E-Mail hinzu {#step-add-the-leads-name-to-the-email}

1. Wählen Sie den oberen bearbeitbaren Abschnitt aus, klicken Sie auf das Zahnradsymbol und wählen Sie **Bearbeiten**.

   ![](assets/nine-2.png)

1. Fügen Sie nach &quot;Hello&quot;ein Leerzeichen hinzu, platzieren Sie den Cursor vor dem Komma und klicken Sie dann auf die **Token einfügen** Symbol.

   ![](assets/ten-4.png)

1. Suchen und Auswählen **`{{lead.First Name}}`** Token.

   ![](assets/eleven-4.png)

1. Geben Sie &quot;Friend&quot;(oder eine beliebige Bezeichnung) in den **Standardwert** Feld und klicken Sie auf **Einfügen**.

   ![](assets/twelve-3.png)

   >[!TIP]
   >
   >Fügen Sie immer einen Standardwert für Token hinzu. Dadurch wird sichergestellt, dass der Standardwert in der E-Mail angezeigt wird, wenn ein Teil der personenbezogenen Daten fehlt.

1. Klicken **Speichern**.

   ![](assets/thirteen-3.png)

1. Schließen Sie den Tab/Fenster des E-Mail-Editors.

   ![](assets/fourteen-3.png)

1. under **E-Mail-Aktionen** auswählen **Entwurf genehmigen**.

   ![](assets/fifteen-3.png)

>[!TIP]
>
>Benötigen Sie einen schnellen Auffrischungskurs dazu, wie Sie sich die E-Mail selbst senden können? Siehe [E-Mail-Blast senden](/help/marketo/getting-started/quick-wins/send-an-email.md){target=&quot;_blank&quot;}.

### Aufgabe abgeschlossen {#mission-complete}

Herzlichen Glückwunsch! Sie haben Ihre E-Mail personalisiert!

<br> 

[◄ Aufgabe 6: Schrittweises Lead-Nurturing](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[Aufgabe 8: Vertriebsmitarbeiter benachrichtigen ►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
