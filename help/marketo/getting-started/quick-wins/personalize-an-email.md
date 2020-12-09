---
unique-page-id: 2359422
description: E-Mail personalisieren - Marketing-Dokumente - Produktdokumentation
title: E-Mail personalisieren
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '389'
ht-degree: 0%

---


# E-Mail personalisieren {#personalize-an-email}

## Auftrag: Persönliche Gestaltung Ihrer E-Mails durch Hinzufügen von Daten-Token {#mission-make-your-emails-personal-by-adding-data-tokens}

>[!NOTE]
>
>**FYI**
>
>Marketo standardisiert nun die Sprache für alle Abonnements, sodass Sie möglicherweise Interessenten in Ihrem Abonnement und Personen/Personen in docs.marketo.com sehen können. Diese Begriffe bedeuten dasselbe. Es hat keine Auswirkungen auf die Artikelanweisungen. Es gibt auch noch einige andere Änderungen. [Weitere Informationen](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!PREREQUISITES]
>
>* [Einrichten und Hinzufügen einer Person](get-set-up-and-add-a-person.md)
>* [E-Mail-Blast senden](send-an-email.md)
>* [Tropfen, Tropfen, Harnwege](drip-drip-nurture.md)


## Schritt 1: E-Mail zur Personalisierung auswählen {#step-select-an-email-to-personalize}

1. Wählen Sie eine der Baumschulen-E-Mails aus, die im [vorherigen Quick win](drip-drip-nurture.md) erstellt wurden, und klicken Sie auf Entwurf **bearbeiten**.

   ![](assets/one-4.png)

   >[!NOTE]
   >
   >Dadurch wird eine Kopie der E-Mail als Entwurf erstellt. Sie müssen den Entwurf genehmigen, damit die Änderungen wirksam werden.

   **Entwurf bearbeiten**

Wenn Sie keinen Popup-Blocker aktiviert haben, wird der E-Mail-Editor in einem neuen Register/Fenster geöffnet. Klicken Sie andernfalls zweimal.

## Schritt 2: Verkäufer zum Absender machen {#step-make-the-salesperson-the-sender}

1. Wählen Sie das Feld **Von** aus, markieren Sie den aktuellen Namen und **löschen Sie** ihn.

   ![](assets/two-5.png)

1. Klicken Sie auf das Symbol **Token** rechts neben dem Feld **Von** .

   ![](assets/three-4.png)

1. Suchen und wählen Sie das **`{{lead.Lead Owner First Name}}`** Token aus.

   ![](assets/four-3.png)

1. Geben Sie den Namen Ihrer Firma und einen Bindestrich für den **Standardwert** ein, um sicherzustellen, dass etwas angezeigt wird, falls der Vorname des Verkaufsprotokolls nicht verfügbar ist. Klicken Sie auf **Einfügen**.

   ![](assets/five-4.png)

1. Drücken Sie die Leertaste im Feld **Von** , und stellen Sie sicher, dass der Cursor ein Leerzeichen nach dem Token blinkt, das Sie gerade eingefügt haben. Klicken Sie dann erneut auf das Symbol **Token** .

   ![](assets/six-4.png)

1. Suchen und wählen Sie das **`{{lead.Lead Owner Last Name}}`** Token aus.

   ![](assets/seven-5.png)

1. Geben Sie &quot;Sales&quot;für den **Standardwert** ein und klicken Sie auf **Einfügen**.

   ![](assets/eight-3.png)

## Schritt 3: hinzufügen der E-Mail den Namen des Interessenten {#step-add-the-leads-name-to-the-email}

1. Wählen Sie den oberen bearbeitbaren Abschnitt aus, klicken Sie auf das Zahnradsymbol und wählen Sie &quot; **Bearbeiten&quot;**.

   ![](assets/nine-2.png)

1. hinzufügen Sie nach &quot;Hallo&quot;einen Leerzeichen und platzieren Sie den Cursor vor dem Komma. Klicken Sie dann auf das Symbol &quot;Token **einfügen&quot;** .

   ![](assets/ten-4.png)

1. Suchen und wählen Sie das **`{{lead.First Name}}`** Token aus.

   ![](assets/eleven-4.png)

1. Geben Sie &quot;Friend&quot;(oder eine beliebige Bezeichnung, die Sie möchten) in das Feld **Standardwert** ein und klicken Sie auf **Einfügen**.

   ![](assets/twelve-3.png)

   >[!TIP]
   >
   >Geben Sie immer einen Standardwert für Token ein. Dadurch wird sichergestellt, dass der Standardwert in der E-Mail angezeigt wird, wenn ein Teil der persönlichen Daten fehlt.

1. Klicken Sie auf **Speichern**.

   ![](assets/thirteen-3.png)

1. Schließen Sie die Registerkarte/das Fenster des E-Mail-Editors.

   ![](assets/fourteen-3.png)

1. Wählen Sie unter **E-Mail-Aktionen** die Option Entwurf **genehmigen**.

   ![](assets/fifteen-3.png)

>[!TIP]
>
>Benötigen Sie einen schnellen Auffrischungsbericht darüber, wie Sie sich die E-Mail senden? Siehe [Senden eines E-Mail-Schnelltests](send-an-email.md).

### Video ansehen {#watch-a-video}

`<iframe width="630" height="470" src="//play.vidyard.com/iRnqxMyJg6VKyuPeuxmHFb.html?v=3.1.1" frameborder="0" allowfullscreen></iframe>`

### Abschluss der Mission {#mission-complete}

Herzlichen Glückwunsch! Sie haben Ihre E-Mail personalisiert!

<br> 

[Auftrag 6: Tropfen, Tropfen, Krankenpflege](drip-drip-nurture.md) , [Mission 8: Warnung des Vertriebsmitarbeiters ►](alert-the-sales-rep.md)