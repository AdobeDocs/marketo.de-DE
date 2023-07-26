---
unique-page-id: 2359422
description: Personalisieren einer E-Mail - Marketo-Dokumente - Produktdokumentation
title: E-Mail personalisieren
exl-id: 1562796e-da47-4305-b950-3bed1d36d339
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 10%

---

# E-Mail personalisieren {#personalize-an-email}

## Auftrag: Personalisieren Sie Ihre E-Mails durch Hinzufügen von Daten-Token {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [Einrichten und Hinzufügen einer Person](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [Massen-E-Mail senden](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}
>* [Schrittweises Lead-Nurturing](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"}

## Schritt 1: E-Mail zur Personalisierung auswählen {#step-select-an-email-to-personalize}

1. Wählen Sie eine der E-Mails aus, die in der [vorheriger Schnellsieg](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"} und klicken **[!UICONTROL Entwurf erstellen]**.

   ![](assets/personalize-an-email-1.png)

   >[!NOTE]
   >
   >Damit wird eine Kopie der E-Mail als Entwurf erstellt. Denken Sie daran, den Entwurf zu validieren, damit die Änderungen live geschaltet werden.

Wenn Sie einen Popup-Blocker nicht aktiviert haben, wird der E-Mail-Editor in einer neuen Registerkarte/einem neuen Fenster geöffnet. Klicken Sie andernfalls auf **[!UICONTROL Entwurf erstellen]** zweimal.

## Schritt 2: Verkäufer zum Absender machen {#step-make-the-salesperson-the-sender}

1. Wählen Sie die **[!UICONTROL Von]** Feld, Hervorhebung und **delete** den aktuellen Namen.

   ![](assets/personalize-an-email-2.png)

1. Klicken Sie auf **Token** rechts neben dem **[!UICONTROL Von]** -Feld.

   ![](assets/personalize-an-email-3.png)

1. Suchen und Auswählen **`{{lead.Lead Owner First Name}}`** Token.

   ![](assets/personalize-an-email-4.png)

1. Geben Sie Ihren Firmennamen und einen Bindestrich für die **Standardwert** um sicherzustellen, dass etwas angezeigt wird, falls der Vorname des Verkaufsprotokolls nicht verfügbar ist. Klicken Sie auf **Einfügen**.

   ![](assets/personalize-an-email-5.png)

1. Drücken Sie die Leertaste im **[!UICONTROL Von]** -Feld, um sicherzustellen, dass der Cursor ein Leerzeichen nach dem soeben eingefügten Token blinkt. Klicken Sie anschließend auf **Token** erneut.

   ![](assets/personalize-an-email-6.png)

1. Suchen und Auswählen **`{{lead.Lead Owner Last Name}}`** Token.

   ![](assets/personalize-an-email-7.png)

1. Geben Sie &quot;Verkauf&quot;für die **Standardwert** und klicken **Einfügen**.

   ![](assets/personalize-an-email-8.png)

## Schritt 3: Hinzufügen des Lead-Namens zur E-Mail {#step-add-the-leads-name-to-the-email}

1. Wählen Sie den oberen bearbeitbaren Abschnitt aus, klicken Sie auf das Zahnradsymbol und wählen Sie **[!UICONTROL Bearbeiten]**.

   ![](assets/personalize-an-email-9.png)

1. Fügen Sie nach &quot;Hello&quot;ein Leerzeichen hinzu, platzieren Sie den Cursor vor dem Komma und klicken Sie dann auf die **Token einfügen** Symbol.

   ![](assets/personalize-an-email-10.png)

1. Suchen und Auswählen **`{{lead.First Name}}`** Token.

   ![](assets/personalize-an-email-11.png)

1. Geben Sie &quot;Friend&quot;(oder eine beliebige Bezeichnung) in den **[!UICONTROL Standardwert]** Feld und klicken Sie auf **[!UICONTROL Einfügen]**.

   ![](assets/personalize-an-email-12.png)

   >[!TIP]
   >
   >Fügen Sie immer einen Standardwert für Token hinzu. Dadurch wird sichergestellt, dass der Standardwert in der E-Mail angezeigt wird, wenn ein Teil der personenbezogenen Daten fehlt.

1. Klicks **[!UICONTROL Speichern]**.

   ![](assets/personalize-an-email-13.png)

1. under **[!UICONTROL E-Mail-Aktionen]** und wählen **[!UICONTROL Genehmigen und schließen]**.

   ![](assets/personalize-an-email-14.png)

>[!TIP]
>
>Benötigen Sie einen schnellen Auffrischungskurs dazu, wie Sie sich die E-Mail selbst senden können? Siehe [E-Mail-Blast senden](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}.

### Aufgabe abgeschlossen {#mission-complete}

Herzlichen Glückwunsch! Sie haben Ihre E-Mail personalisiert!

<br> 

[◄ Aufgabe 6: Schrittweises Lead-Nurturing](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[Aufgabe 8: Vertriebsmitarbeiter benachrichtigen ►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
