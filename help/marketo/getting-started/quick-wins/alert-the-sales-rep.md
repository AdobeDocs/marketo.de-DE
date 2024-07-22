---
unique-page-id: 2359424
description: Warnhinweis an den Vertriebsmitarbeiter - Marketo-Dokumente - Produktdokumentation
title: Vertriebsmitarbeiter benachrichtigen
exl-id: 4ad7d7b8-ee1e-4605-b4e0-e72a7e573c05
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 2%

---

# Vertriebsmitarbeiter benachrichtigen {#alert-the-sales-rep}

## Auftrag: Warnung des Vertriebsmitarbeiters, wenn ein Benutzer ein Formular auf Ihrer Website ausfüllt {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

Um Warn-E-Mails automatisch an Vertriebsmitarbeiter zu senden, benötigen Sie lediglich eine Warn-E-Mail und eine E-Mail-Kampagne. Hier ist, wie man das macht.

>[!PREREQUISITES]
>
>[Landingpage mit einem Formular](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## Schritt 1: Erstellen einer Warnhinweis-E-Mail {#step-create-an-alert-email}

1. Wechseln Sie zum Bereich **[!UICONTROL Marketingaktivitäten]** .

   ![](assets/alert-the-sales-rep-1.png)

1. Wählen Sie **Mein Programm** aus, das Sie auf der [Landingpage mit einem Schnellgewinn für Formular](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"} erstellt haben, und klicken Sie dann unter **[!UICONTROL Neu]** auf **[!UICONTROL Neues lokales Asset]**.

   ![](assets/alert-the-sales-rep-2.png)

1. Klicken Sie auf **[!UICONTROL E-Mail]**.

   ![](assets/alert-the-sales-rep-3.png)

1. **Name** der E-Mail &quot;Mein E-Mail-Warnhinweis&quot;, wählen Sie eine Vorlage aus und klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/alert-the-sales-rep-4.png)

1. Geben Sie die Werte **Von Name**, **Von E-Mail**, **[!UICONTROL Antwort auf]** und **[!UICONTROL Betreff]** ein, die Ihr Verkaufsteam sehen soll.

   ![](assets/alert-the-sales-rep-5.png)

1. Doppelklicken Sie auf , um den E-Mail-Text zu bearbeiten.

   ![](assets/alert-the-sales-rep-6.png)

1. Geben Sie den E-Mail-Inhalt ein.

   ![](assets/alert-the-sales-rep-7.png)

1. Platzieren Sie den Cursor an die Stelle, an der Sie die Kontaktinformationen der Person einfügen möchten, und klicken Sie auf das Symbol **Token einfügen** .

   ![](assets/alert-the-sales-rep-8.png)

1. Suchen und wählen Sie den `{{SP_Send_Alert_Info}}` **[!UICONTROL Token]** aus und klicken Sie auf **[!UICONTROL Einfügen]**.

   ![](assets/alert-the-sales-rep-9.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}} ist ein spezielles Token für Warn-E-Mails. Weitere Informationen finden Sie unter [Verwenden des Tokens &quot;Warnhinweisinformationen senden&quot;](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md){target="_blank"}{target="_blank"} .

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/alert-the-sales-rep-10.png)

1. Klicken Sie auf das Dropdown-Menü **[!UICONTROL E-Mail-Aktionen]** und wählen Sie **[!UICONTROL Genehmigen und schließen]** aus.

   ![](assets/alert-the-sales-rep-11.png)

## Schritt 2: Erstellen einer Warnhinweis-Trigger-Kampagne {#step-create-an-alert-trigger-campaign}

1. Wählen Sie **Mein zuvor erstelltes Programm** und klicken Sie dann unter **[!UICONTROL Neu]** auf **[!UICONTROL Neue Smart-Kampagne]** .

   ![](assets/alert-the-sales-rep-12.png)

1. **Nennen** Sie die Kampagne &quot;Meine Warnungskampagne&quot;und klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/alert-the-sales-rep-13.png)

1. Suchen Sie auf der Registerkarte **[!UICONTROL Smart List]** den Trigger **[!UICONTROL Fills Out Form]** und ziehen Sie ihn auf die Arbeitsfläche.

   ![](assets/alert-the-sales-rep-14.png)

1. Wählen Sie das zuvor erstellte Formular aus.

   ![](assets/alert-the-sales-rep-15.png)

1. Suchen Sie auf der Registerkarte **[!UICONTROL Fluss]** die Flussaktion **[!UICONTROL Warnung senden]** und ziehen Sie sie auf die Arbeitsfläche.

   ![](assets/alert-the-sales-rep-16.png)

1. Wählen Sie &quot;**[!UICONTROL Meine Benachrichtigungs-E-Mail]**&quot;, die zuvor erstellt wurde, und belassen Sie &quot;**[!UICONTROL Senden an]**&quot;als &quot;**[!UICONTROL Vertriebsmitarbeiter]**&quot;.

   ![](assets/alert-the-sales-rep-17.png)

1. Geben Sie Ihre E-Mail-Adresse in das Feld **[!UICONTROL An andere E-Mails]** ein.

   ![](assets/alert-the-sales-rep-18.png)

1. Gehen Sie zur Registerkarte **[!UICONTROL Plan]** und klicken Sie auf die Schaltfläche **[!UICONTROL Aktivieren]** .

   ![](assets/alert-the-sales-rep-19.png)

   >[!TIP]
   >
   >Setzen Sie die **[!UICONTROL Qualifikationsregeln]** auf **[!UICONTROL jedes Mal]** (durch Bearbeiten der Smart-Kampagne), damit dieselbe Person Warnhinweise mehrmals Trigger.

1. Klicken Sie auf dem Bestätigungsbildschirm auf **[!UICONTROL Aktivieren]** .

   ![](assets/alert-the-sales-rep-20.png)

## Schritt 3: Testen Sie es! {#step-test-it-out}

1. Wählen Sie Ihre Landingpage aus und klicken Sie auf **[!UICONTROL Genehmigte Seite anzeigen]**.

   ![](assets/alert-the-sales-21.png)

   >[!NOTE]
   >
   >Vergessen Sie nicht, Landingpages zu validieren. Sie werden erst live geschaltet, wenn sie genehmigt wurden.

1. Füllen Sie das Formular aus und klicken Sie auf **[!UICONTROL Senden]**.

   ![](assets/alert-the-sales-22.png)

1. Sie sollten Ihre E-Mail in Kürze erhalten. Nachdem Sie überprüft haben, ob alles wie gewünscht funktioniert, entfernen Sie Ihre E-Mail-Adresse aus dem Fluss Warnhinweis senden (siehe Schritt 2.7 oben).

   >[!NOTE]
   >
   >Klicken Sie in Marketo auf die Registerkarte **[!UICONTROL Persönliche Informationen]** , um die Kontaktinformationen anzuzeigen.

## Auftrag abgeschlossen! {#mission-complete}

<br> 

[Auftrag 7: E-Mail personalisieren](/help/marketo/getting-started/quick-wins/personalize-an-email.md)

[Mission 9: Aktualisieren der Daten des Benutzers ► ►](/help/marketo/getting-started/quick-wins/update-person-data.md)
