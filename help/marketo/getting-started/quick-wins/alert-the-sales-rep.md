---
unique-page-id: 2359424
description: Warnung des Vertriebsmitarbeiters - Marketing Docs - Produktdokumentation
title: Warnung an den Vertriebsmitarbeiter
translation-type: tm+mt
source-git-commit: 09dbd3a141fed0525aec8bf1ca6d141be2a6ce46
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---


# Warnung an den Vertriebsmitarbeiter {#alert-the-sales-rep}

## Auftrag: Warnung des Vertriebsmitarbeiters, wenn eine Person ein Formular auf Ihrer Website ausfüllt {#mission-alert-the-sales-rep-when-a-person-fills-out-a-form-on-your-web-site}

Um Warnungen automatisch an Vertriebsmitarbeiter zu senden, benötigen Sie lediglich eine Warn-E-Mail und eine E-Mail-Kampagne. Hier ist, wie man das macht.

>[!NOTE]
>
>**FYI**
>
>Marketo standardisiert nun die Sprache für alle Abonnements, sodass Sie möglicherweise Interessenten in Ihrem Abonnement und Personen/Personen in docs.marketo.com sehen können. Diese Begriffe bedeuten dasselbe. Es hat keine Auswirkungen auf die Artikelanweisungen. Es gibt auch noch einige andere Änderungen. [Weitere Informationen](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!NOTE]
>
>**Voraussetzungen**
>
>* [Landingpage mit einem Formular](landing-page-with-a-form.md)

>



## Schritt 1: Warnungs-E-Mail erstellen {#step-create-an-alert-email}

1. Gehen Sie zum Bereich **Marketing-Aktivitäten** .

   ![](assets/one-5.png)

1. Wählen Sie **Mein Programm** , das Sie in der [Landingpage mit einem Formular](landing-page-with-a-form.md) erstellt haben, schnell gewinnen und klicken Sie dann unter **Neu** auf **Neues lokales Asset**.

   ![](assets/two-6.png)

1. Klicken Sie auf **E-Mail**.

   ![](assets/three-5.png)

1. **Benennen** Sie die E-Mail mit &quot;Meine E-Mail-Warnung&quot;, wählen Sie eine Vorlage und klicken Sie auf **Erstellen**.

   ![](assets/four-4.png)

1. Geben Sie die **Formulardamen**, **Von E-Mail**, **Antwort auf** und **Betreff** ein, die Ihr Vertriebsteam sehen soll.

   ![](assets/five-5.png)

1. Klicken Sie mit der Dublette, um den E-Mail-Text zu bearbeiten.

   ![](assets/six-5.png)

1. Geben Sie den E-Mail-Inhalt ein.

   ![](assets/seven-6.png)

1. Platzieren Sie den Cursor an der Stelle, an der Sie die Kontaktinformationen der Person einfügen möchten, und klicken Sie auf das Symbol &quot;Token **einfügen&quot;** .

   ![](assets/eight-4.png)

1. Suchen Sie nach dem `{{SP_Send_Alert_Info}}` Token **, wählen Sie es aus und klicken Sie auf** Einfügen ****.

   ![](assets/image2014-9-24-13-3a10-3a0.png)

   >[!NOTE]
   >
   >{{SP_Send_Alert_Info}} ist ein spezielles Token für Warn-E-Mails. Weitere Informationen finden Sie unter [Verwenden des Tokens](../../product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md) für Warnhinweise senden.

1. Klicken Sie auf **Speichern**.

   ![](assets/ten-5.png)

1. Schließen Sie die Registerkarte/das Fenster des E-Mail-Editors.

   ![](assets/eleven-5.png)

1. Klicken Sie unter **E-Mail-Aktionen** auf **Genehmigen**.

   ![](assets/twelve-4.png)

## Schritt 2: Warnauslöser-Kampagne erstellen {#step-create-an-alert-trigger-campaign}

1. Wählen Sie **Mein Programm** , das zuvor erstellt wurde, und klicken Sie dann unter **Neu **auf **Neue intelligente Kampagne**.

   ![](assets/image2014-9-24-13-3a14-3a17.png)

1. **Benennen** Sie die Kampagne &quot;Meine Kampagne für Warnung&quot;und klicken Sie auf **Erstellen**.

   ![](assets/image2014-9-24-13-3a14-3a28.png)

1. Suchen Sie auf der Registerkarte &quot; **Intelligente Liste** &quot;den Auslöser &quot;Formular **ausfüllen** &quot;und ziehen Sie ihn auf die Arbeitsfläche.

   ![](assets/image2014-9-24-13-3a14-3a43.png)

1. Wählen Sie das zuvor erstellte Formular aus.

   ![](assets/image2014-9-24-13-3a14-3a58.png)

1. Suchen Sie auf der Registerkarte &quot; **Fluss** &quot;nach der Aktion &quot; **Warnung** senden&quot;und ziehen Sie sie auf die Arbeitsfläche.

   ![](assets/image2014-9-24-13-3a15-3a10.png)

1. Wählen Sie **Meine Warnhinweis-E-Mail** , die zuvor erstellt wurde, und lassen Sie &quot; **Senden an** &quot;als **Vertriebsmitarbeiter**.

   ![](assets/eighteen-1.png)

1. Geben Sie Ihre E-Mail-Adresse in das Feld **An andere E-Mails** ein.

   ![](assets/nineteen-2.png)

1. Gehen Sie zur Registerkarte **Plan** und klicken Sie auf die Schaltfläche **Aktivieren **s.

   ![](assets/twenty-2.png)

   >[!TIP]
   >
   >
   >Legen Sie die **Qualifikationsregeln** auf **jedes Mal** fest (durch Bearbeiten der intelligenten Kampagne), damit dieselbe Person Warnhinweise mehrmals auslösen kann.

1. Klicken Sie im Bestätigungsbildschirm auf **Aktivieren** .

   ![](assets/twenty-one-1.png)

## Schritt 3: Testen Sie es! {#step-test-it-out}

1. Wählen Sie Ihre Landingpage aus und klicken Sie auf &quot; **Ansicht genehmigt&quot;**.

   ![](assets/image2014-9-24-13-3a17-3a8.png)

   >[!NOTE]
   >
   >**Erinnerung**
   >
   >
   >Vergessen Sie nicht, Landingpages zu genehmigen; sie gehen erst nach Genehmigung live.

1. Füllen Sie das Formular aus und klicken Sie auf **Senden**.

   ![](assets/image2014-9-24-13-3a17-3a41.png)

1. Sie sollten Ihre E-Mail in Kürze erhalten. Nachdem Sie überprüft haben, ob alles ordnungsgemäß funktioniert, entfernen Sie Ihre E-Mail-Adresse aus dem Fluss Warnung senden (siehe Schritt 2.7 oben).

   >[!NOTE]
   >
   >Klicken Sie auf die Registerkarte **Personeninfo** in Marketo, um die Kontaktinformationen anzuzeigen.

## Auftrag abgeschlossen! {#mission-complete}

<br> 

[Auftrag 7: Personalisieren einer E-Mail](personalize-an-email.md) - [Mission 9: Lead-Daten aktualisieren ►](update-person-data.md)