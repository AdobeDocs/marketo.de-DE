---
unique-page-id: 2359422
description: Personalisieren einer E-Mail - Marketo-Dokumente - Produktdokumentation
title: E-Mail personalisieren
exl-id: 1562796e-da47-4305-b950-3bed1d36d339
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 3%

---

# E-Mail personalisieren {#personalize-an-email}

## Mission: Personalisieren von E-Mails durch Hinzufügen von Daten-Token {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [Einrichten und Person hinzufügen](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [Senden einer E-Mail-Explosion](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}
>* [tropfen, tropfen, nähren](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"}

## Schritt 1: E-Mail zur Personalisierung auswählen {#step-select-an-email-to-personalize}

1. Wählen Sie eine der im vorherigen [ erstellten Nurture-E-Mails aus ](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"} klicken Sie auf **[!UICONTROL Entwurf erstellen]**.

   ![](assets/personalize-an-email-1.png)

   >[!NOTE]
   >
   >Dadurch wird eine Kopie der E-Mail als Entwurf erstellt. Denken Sie daran, den Entwurf zu genehmigen, damit die Änderungen live geschaltet werden.

Wenn Sie keinen Popup-Blocker aktiviert haben, wird der E-Mail-Editor in einer neuen Registerkarte/einem neuen Fenster geöffnet. Klicken Sie andernfalls zweimal **[!UICONTROL Entwurf erstellen]**.

## Schritt 2: Verkaufsberater zum Absender machen {#step-make-the-salesperson-the-sender}

1. Wählen Sie das Feld **[!UICONTROL Von]** aus, markieren Sie den aktuellen Namen **Löschen**.

   ![](assets/personalize-an-email-2.png)

1. Klicken Sie auf **Token** rechts neben dem Feld **[!UICONTROL Von]**.

   ![](assets/personalize-an-email-3.png)

1. Suchen Sie das **`{{lead.Lead Owner First Name}}`**-Token und wählen Sie es aus.

   ![](assets/personalize-an-email-4.png)

1. Geben Sie Ihren Firmennamen und einen Bindestrich für den **Standardwert** ein, um sicherzustellen, dass etwas angezeigt wird, falls der Vorname des Vertriebsmitarbeiters nicht verfügbar ist. Klicken Sie auf **Einfügen**.

   ![](assets/personalize-an-email-5.png)

1. Klicken Sie auf die Leertaste im Feld **[!UICONTROL Von]** und stellen Sie sicher, dass der Cursor ein Leerzeichen nach dem soeben eingefügten Token blinkt. Klicken Sie dann erneut auf **Token**-Symbol.

   ![](assets/personalize-an-email-6.png)

1. Suchen Sie das **`{{lead.Lead Owner Last Name}}`**-Token und wählen Sie es aus.

   ![](assets/personalize-an-email-7.png)

1. Geben Sie als **Standardwert“ „Verkauf“ ein** klicken Sie auf **Einfügen**.

   ![](assets/personalize-an-email-8.png)

## Schritt 3: Hinzufügen des Lead-Namens zur E-Mail {#step-add-the-leads-name-to-the-email}

1. Wählen Sie den oberen bearbeitbaren Abschnitt aus, klicken Sie auf das Zahnradsymbol und wählen Sie **[!UICONTROL Bearbeiten]**.

   ![](assets/personalize-an-email-9.png)

1. Fügen Sie nach „Hallo“ ein Leerzeichen hinzu, platzieren Sie den Cursor vor dem Komma und klicken Sie dann auf das Symbol **Token einfügen**.

   ![](assets/personalize-an-email-10.png)

1. Suchen Sie das **`{{lead.First Name}}`**-Token und wählen Sie es aus.

   ![](assets/personalize-an-email-11.png)

1. Geben Sie „Freund“ (oder eine beliebige Bezeichnung) in das Feld **[!UICONTROL Standardwert]** ein und klicken Sie auf **[!UICONTROL Einfügen]**.

   ![](assets/personalize-an-email-12.png)

   >[!TIP]
   >
   >Geben Sie immer einen Standardwert für Token an. Dadurch wird sichergestellt, dass der Standardwert in der E-Mail angezeigt wird, wenn ein Teil der persönlichen Informationen fehlt.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/personalize-an-email-13.png)

1. Wählen Sie unter **[!UICONTROL E]** Mail-Aktionen“ die Option **[!UICONTROL Genehmigen und schließen]** aus.

   ![](assets/personalize-an-email-14.png)

>[!TIP]
>
>Benötigen Sie eine kurze Auffrischung, wie Sie sich die E-Mail senden? Siehe [E-Mail-Versand](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}.

### Aufgabe abgeschlossen {#mission-complete}

Herzlichen Glückwunsch, Sie haben Ihre E-Mail personalisiert!

<br> 

[◄ Mission 6: Tropfen, Tropfen, Pflegen](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[Mission 8: Benachrichtigung des Vertriebsmitarbeiters ►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
