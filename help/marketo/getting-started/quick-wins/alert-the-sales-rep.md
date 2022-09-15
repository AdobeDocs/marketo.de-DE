---
unique-page-id: 2359424
description: Warnhinweis an den Vertriebsmitarbeiter - Marketo-Dokumente - Produktdokumentation
title: Vertriebsmitarbeiter benachrichtigen
exl-id: 4ad7d7b8-ee1e-4605-b4e0-e72a7e573c05
source-git-commit: 1127928b43762086ed4d157719ff80d6c3de9ee3
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 4%

---

# Vertriebsmitarbeiter benachrichtigen {#alert-the-sales-rep}

## Auftrag: Warnen Sie den Vertriebsmitarbeiter, wenn eine Person ein Formular auf Ihrer Website ausfüllt. {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

Um Warn-E-Mails automatisch an Vertriebsmitarbeiter zu senden, benötigen Sie lediglich eine Warn-E-Mail und eine E-Mail-Kampagne. Hier ist, wie man das macht.

>[!PREREQUISITES]
>
>[Landingpage mit einem Formular](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;}

## Schritt 1: Erstellen einer Warnhinweis-E-Mail {#step-create-an-alert-email}

1. Navigieren Sie zu **Marketingaktivitäten** Bereich.

   ![](assets/alert-the-sales-rep-1.png)

1. Auswählen **Mein Programm** , die Sie in der [Landingpage mit einem Formular](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;} schneller Sieg, dann unter **Neu** click **Neues lokales Asset**.

   ![](assets/alert-the-sales-rep-2.png)

1. Klicken **Email**.

   ![](assets/alert-the-sales-rep-3.png)

1. **Name** die E-Mail &quot;Meine E-Mail-Warnung&quot;, wählen Sie eine Vorlage aus und klicken Sie auf **Erstellen**.

   ![](assets/alert-the-sales-rep-4.png)

1. Geben Sie die **Aus Name**, **Aus E-Mail**, **Antwort** und **Betreff** die Sie von Ihrem Verkaufsteam sehen wollen.

   ![](assets/alert-the-sales-rep-5.png)

1. Doppelklicken Sie, um den E-Mail-Text zu bearbeiten.

   ![](assets/alert-the-sales-rep-6.png)

1. Geben Sie den E-Mail-Inhalt ein.

   ![](assets/alert-the-sales-rep-7.png)

1. Platzieren Sie den Cursor an die Stelle, an der Sie die Kontaktinformationen der Person einfügen möchten, und klicken Sie auf die **Token einfügen** Symbol.

   ![](assets/alert-the-sales-rep-8.png)

1. Suchen und Auswählen `{{SP_Send_Alert_Info}}` **Token** und klicken Sie auf **Einfügen**.

   ![](assets/alert-the-sales-rep-9.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}} ist ein spezielles Token für Warnhinweis-E-Mails. Siehe [Verwenden des Tokens &quot;Send Alert Info&quot;](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target=&quot;_blank&quot;}{target=&quot;_blank&quot;}, um mehr zu erfahren.

1. Klicken **Speichern**.

   ![](assets/alert-the-sales-rep-10.png)

1. Klicken Sie auf **E-Mail-Aktionen** und wählen Sie **Genehmigen und schließen**.

   ![](assets/alert-the-sales-rep-11.png)

## Schritt 2: Erstellen einer Warnhinweis-Trigger-Kampagne {#step-create-an-alert-trigger-campaign}

1. Auswählen **Mein Programm** zuvor erstellt, dann unter **Neu** click **Neue intelligente Kampagne**.

   ![](assets/alert-the-sales-rep-12.png)

1. **Name** die Kampagne &quot;Meine Warnungskampagne&quot;und klicken Sie auf **Erstellen**.

   ![](assets/alert-the-sales-rep-13.png)

1. Unter dem **Smart List** Registerkarte, suchen und ziehen Sie die **Formular ausfüllen** Trigger zur Arbeitsfläche.

   ![](assets/alert-the-sales-rep-14.png)

1. Wählen Sie das zuvor erstellte Formular aus.

   ![](assets/alert-the-sales-rep-15.png)

1. Unter dem **Fluss** Registerkarte, suchen und ziehen Sie die **Warnhinweis senden** Flussaktion zur Arbeitsfläche.

   ![](assets/alert-the-sales-rep-16.png)

1. Auswählen **Meine Benachrichtigungs-E-Mail** zuvor erstellt und verlassen **Senden an** as **Vertriebsmitarbeiter**.

   ![](assets/alert-the-sales-rep-17.png)

1. Geben Sie Ihre E-Mail-Adresse in das Feld **zu anderen E-Mails** -Feld.

   ![](assets/alert-the-sales-rep-18.png)

1. Navigieren Sie zu **Zeitplan** und klicken Sie auf **Aktivieren** Schaltfläche.

   ![](assets/alert-the-sales-rep-19.png)

   >[!TIP]
   >
   >Legen Sie die **Qualifikationsregeln** nach **jedes Mal** (durch Bearbeiten der Smart-Kampagne), damit dieselbe Person Warnhinweise mehrmals Trigger.

1. Klicken **Aktivieren** auf dem Bestätigungsbildschirm.

   ![](assets/alert-the-sales-rep-20.png)

## Schritt 3: Testen Sie es! {#step-test-it-out}

1. Wählen Sie Ihre Landingpage aus und klicken Sie auf **Genehmigte Seite anzeigen**.

   ![](assets/alert-the-sales-21.png)

   >[!NOTE]
   >
   >Vergessen Sie nicht, Landingpages zu genehmigen. sie gehen erst live, wenn sie genehmigt wurden.

1. Füllen Sie das Formular aus und klicken Sie auf **Einsenden**.

   ![](assets/alert-the-sales-22.png)

1. Sie sollten Ihre E-Mail in Kürze erhalten. Nachdem Sie überprüft haben, ob alles wie gewünscht funktioniert, entfernen Sie Ihre E-Mail-Adresse aus dem Fluss Warnhinweis senden (siehe Schritt 2.7 oben).

   >[!NOTE]
   >
   >Klicken Sie auf **Personeninformationen** in Marketo, um die Kontaktinformationen anzuzeigen.

## Aufgabe abgeschlossen! {#mission-complete}

<br> 

[◄ Aufgabe 7: E-Mail personalisieren](/help/marketo/getting-started/quick-wins/personalize-an-email.md)

[Auftrag 9: Persönliche Daten aktualisieren ►](/help/marketo/getting-started/quick-wins/update-person-data.md)
