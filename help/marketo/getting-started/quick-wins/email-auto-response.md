---
unique-page-id: 2359416
description: Automatische E-Mail-Antwort - Marketo-Dokumente - Produktdokumentation
title: Automatische Antwort-E-Mail
exl-id: c9c0a154-65ec-4845-97a0-a2100223cb13
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 15%

---

# Automatische Antwort-E-Mail {#email-auto-response}

## Auftrag: Senden einer Dankesnachricht, wenn eine Person ein Formular ausfüllt {#mission-send-out-a-thank-you-email-when-a-person-fills-out-a-form}

>[!PREREQUISITES]
>
>* [Einrichten und Hinzufügen einer Person](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [Landing Page mit Formular](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## Schritt 1: E-Mail erstellen {#step-create-an-email}

1. Navigieren Sie zu **[!UICONTROL Marketingaktivitäten]** Bereich.

   ![](assets/email-auto-response-1.png)

1. Wählen Sie Ihr Programm im linken Menü aus und klicken Sie auf die Schaltfläche **[!UICONTROL Neu]** und wählen Sie **[!UICONTROL Neues lokales Asset]**.

   ![](assets/email-auto-response-2.png)

1. Auswählen **[!UICONTROL Email]**.

   ![](assets/email-auto-response-3.png)

1. Benennen Sie Ihre E-Mail mit &quot;Automatische Antwort-E-Mail&quot;, wählen Sie eine Vorlage aus und klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/email-auto-response-4.png)

   Ein E-Mail-Editor wird in einem neuen Fenster oder Tab geöffnet. Wenn Popups blockiert sind, klicken Sie auf **[!UICONTROL Entwurf bearbeiten]** auf der Asset-Zusammenfassungsseite, um auf die E-Mail zuzugreifen.

1. Geben Sie eine Betreffzeile ein und doppelklicken Sie auf den bearbeitbaren Bereich der E-Mail.

   ![](assets/email-auto-response-5.png)

   _Im E-Mail-Editor wird ein Rich-Text-Editor geöffnet._

1. Markieren Sie den vorhandenen E-Mail-Inhalt.

   ![](assets/email-auto-response-6.png)

1. Geben Sie Ihren E-Mail-Inhalt ein und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/email-auto-response-7.png)

1. Klicken Sie auf **[!UICONTROL E-Mail-Aktionen]** und wählen Sie **[!UICONTROL Genehmigen und schließen]**.

   ![](assets/email-auto-response-8.png)

## Schritt 2: Intelligente Kampagne erstellen {#step-create-a-smart-campaign}

1. Wählen Sie Ihr Programm aus, klicken Sie auf das **[!UICONTROL Neu]** und wählen Sie **[!UICONTROL Neue intelligente Kampagne]**.

   ![](assets/email-auto-response-9.png)

1. **Name** Ihre Smart-Kampagne &quot;Automatische Antwortkampagne&quot;und klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/email-auto-response-10.png)

1. Wechseln Sie zur Registerkarte **[!UICONTROL Intelligente Liste]**.

   ![](assets/email-auto-response-11.png)

   Wir richten diese Kampagne so ein, dass sie immer dann ausgeführt wird, wenn eine Person das in [**Landingpage mit einem Formular**](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}.

1. Suchen und Ziehen **[!UICONTROL Formular ausfüllen]** Trigger zur Arbeitsfläche.

   ![](assets/email-auto-response-12.png)

1. Auswählen **[!UICONTROL Mein Formular]** in der Dropdown-Liste. Klicken Sie anschließend auf **[!UICONTROL Fluss]** Registerkarte.

   ![](assets/email-auto-response-13.png)

1. Ziehen Sie die **[!UICONTROL E-Mail senden]** Flussaktion auf die linke Arbeitsfläche.

   ![](assets/email-auto-response-14.png)

1. Wählen Sie Ihre **Automatische Antwort-E-Mail**. Klicken Sie anschließend auf **[!UICONTROL Zeitplan]** Registerkarte.

   ![](assets/email-auto-response-15.png)

1. Klicken **[!UICONTROL Bearbeiten]**.

   ![](assets/email-auto-response-16.png)

1. Wählen Sie **[!UICONTROL Immer]** aus und klicken Sie dann auf **[!UICONTROL Speichern]**.

   ![](assets/email-auto-response-17.png)

1. Klicken Sie auf **[!UICONTROL Aktivieren]**.

   ![](assets/email-auto-response-18.png)

1. Klicken **[!UICONTROL Aktivieren]** auf dem Bestätigungsbildschirm.

   ![](assets/email-auto-response-19.png)

>[!NOTE]
>
>Nach der Aktivierung wird diese Kampagne jedes Mal ausgeführt, wenn eine Person das angegebene Formular ausfüllt. Die Kampagne läuft so lange, bis sie deaktiviert wird.

## Schritt 3: Formular ausfüllen {#step-fill-out-the-form}

1. Auswählen **Meine Seite** (Dies wurde im [Landingpage mit einem Formular](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"} quick win) und klicken Sie auf **[!UICONTROL Vorschau]**.

   ![](assets/email-auto-response-20.png)

   _Ihre Landingpage &quot;Kostenlose Testversion&quot;wird in einem neuen Tab geöffnet._

1. Füllen Sie das Formular mit Vorname, Nachname und E-Mail-Adresse aus und klicken Sie auf **[!UICONTROL Einsenden]**.

   ![](assets/email-auto-response-21.png)

>[!NOTE]
>
>Stellen Sie sicher, dass Sie Ihre richtige E-Mail-Adresse verwenden, damit Sie E-Mails empfangen können.

## Aufgabe abgeschlossen {#mission-complete}

Innerhalb weniger Minuten sollte die automatische Antwort-E-Mail in Ihrem Posteingang angezeigt werden. Großartig gemacht!

<br> 

[◄ Aufgabe 3: Einfache Bewertung](/help/marketo/getting-started/quick-wins/simple-scoring.md)

[Auftrag 5: Import a List of People ►](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)
