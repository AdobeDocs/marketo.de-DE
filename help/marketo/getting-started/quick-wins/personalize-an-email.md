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

## Auftrag: Personalisieren Sie Ihre E-Mails durch Hinzufügen von Daten-Token {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!PREREQUISITES]
>
>* [Einrichten und Hinzufügen einer Person](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [E-Mail-Blast senden](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}
>* [Drip, Drip, Nurture](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"}

## Schritt 1: E-Mail zur Personalisierung auswählen {#step-select-an-email-to-personalize}

1. Wählen Sie eine der E-Mails, die in der Vorlesung &quot;[previous quick win](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md){target="_blank"}&quot;erstellt wurden, und klicken Sie auf &quot;**[!UICONTROL Entwurf erstellen]**&quot;.

   ![](assets/personalize-an-email-1.png)

   >[!NOTE]
   >
   >Dadurch wird eine Kopie der E-Mail als Entwurf erstellt. Denken Sie daran, den Entwurf zu validieren, damit die Änderungen live geschaltet werden.

Wenn Sie einen Popup-Blocker nicht aktiviert haben, wird der E-Mail-Editor in einer neuen Registerkarte/einem neuen Fenster geöffnet. Klicken Sie andernfalls zweimal auf **[!UICONTROL Entwurf erstellen]** .

## Schritt 2: Verkäufer zum Absender machen {#step-make-the-salesperson-the-sender}

1. Markieren Sie das Feld **[!UICONTROL From]** , markieren Sie den aktuellen Namen und **delete** .

   ![](assets/personalize-an-email-2.png)

1. Klicken Sie auf das Symbol **Token** rechts neben dem Feld **[!UICONTROL Von]**.

   ![](assets/personalize-an-email-3.png)

1. Suchen und wählen Sie das Token **`{{lead.Lead Owner First Name}}`** aus.

   ![](assets/personalize-an-email-4.png)

1. Geben Sie Ihren Unternehmensnamen und einen Bindestrich für den **Standardwert** ein, um sicherzustellen, dass etwas angezeigt wird, falls der Vorname des Verkaufs-Reps nicht verfügbar ist. Klicken Sie auf **Einfügen**.

   ![](assets/personalize-an-email-5.png)

1. Drücken Sie die Leertaste im Feld **[!UICONTROL Von]** , um sicherzustellen, dass der Cursor einen Leerraum nach dem soeben eingefügten Token blinkt. Klicken Sie dann erneut auf das Symbol **Token** .

   ![](assets/personalize-an-email-6.png)

1. Suchen und wählen Sie das Token **`{{lead.Lead Owner Last Name}}`** aus.

   ![](assets/personalize-an-email-7.png)

1. Geben Sie &quot;Sales&quot;für den **Standardwert** ein und klicken Sie auf **Insert**.

   ![](assets/personalize-an-email-8.png)

## Schritt 3: Hinzufügen des Lead-Namens zur E-Mail {#step-add-the-leads-name-to-the-email}

1. Wählen Sie den oberen bearbeitbaren Abschnitt aus, klicken Sie auf das Zahnradsymbol und wählen Sie **[!UICONTROL Bearbeiten]** aus.

   ![](assets/personalize-an-email-9.png)

1. Fügen Sie nach &quot;Hello&quot;ein Leerzeichen hinzu, platzieren Sie den Cursor vor dem Komma und klicken Sie dann auf das Symbol **Token einfügen** .

   ![](assets/personalize-an-email-10.png)

1. Suchen und wählen Sie das Token **`{{lead.First Name}}`** aus.

   ![](assets/personalize-an-email-11.png)

1. Geben Sie &quot;Friend&quot;(oder eine beliebige Beschriftung) in das Feld **[!UICONTROL Standardwert]** ein und klicken Sie auf **[!UICONTROL Einfügen]**.

   ![](assets/personalize-an-email-12.png)

   >[!TIP]
   >
   >Fügen Sie immer einen Standardwert für Token hinzu. Dadurch wird sichergestellt, dass der Standardwert in der E-Mail angezeigt wird, wenn ein Teil der personenbezogenen Daten fehlt.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/personalize-an-email-13.png)

1. Wählen Sie unter &quot;**[!UICONTROL E-Mail-Aktionen]**&quot;die Option &quot;**[!UICONTROL Genehmigen und schließen]**&quot;.

   ![](assets/personalize-an-email-14.png)

>[!TIP]
>
>Benötigen Sie einen schnellen Auffrischungskurs dazu, wie Sie sich die E-Mail selbst senden können? Siehe [E-Mail-Blast senden](/help/marketo/getting-started/quick-wins/send-an-email.md){target="_blank"}.

### Aufgabe abgeschlossen {#mission-complete}

Herzlichen Glückwunsch! Sie haben Ihre E-Mail personalisiert!

<br> 

[Auftrag 6: Drip, Drip, Nurture](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)

[Mission 8: Warnung des Vertriebsmitarbeiters ►](/help/marketo/getting-started/quick-wins/alert-the-sales-rep.md)
