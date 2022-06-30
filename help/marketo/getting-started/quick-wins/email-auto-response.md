---
unique-page-id: 2359416
description: Automatische E-Mail-Antwort - Marketo-Dokumente - Produktdokumentation
title: Automatische Antwort-E-Mail
exl-id: c9c0a154-65ec-4845-97a0-a2100223cb13
source-git-commit: 0da33dfa840dd1e5a5618fcd762b482f7a2e0789
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Automatische Antwort-E-Mail {#email-auto-response}

## Auftrag: Senden einer Dankesnachricht, wenn eine Person ein Formular ausfüllt {#mission-send-out-a-thank-you-email-when-a-person-fills-out-a-form}

>[!PREREQUISITES]
>
>* [Einrichten und Hinzufügen einer Person](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target=&quot;_blank&quot;}
>* [Landingpage mit einem Formular](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;}


## Schritt 1: E-Mail erstellen {#step-create-an-email}

1. Wechseln Sie zum Bereich Marketingaktivitäten .

   ![](assets/one-2.png)

1. Wählen Sie im linken Menü Mein Programm aus, klicken Sie auf das Dropdown-Menü Neu und wählen Sie Neues lokales Asset.

   ![](assets/two-3.png)

1. Klicken Sie auf die E-Mail.

   ![](assets/three-2.png)

1. Benennen Sie Ihre E-Mail mit &quot;Automatische Antwort-E-Mail&quot;, wählen Sie eine Vorlage aus und klicken Sie auf Erstellen.

   ![](assets/four-1.png)

   Ein E-Mail-Editor wird in einem neuen Fenster oder Tab geöffnet. Wenn Popups blockiert sind, klicken Sie auf **Entwurf bearbeiten** auf der Asset-Zusammenfassungsseite, um auf die E-Mail zuzugreifen.

1. Geben Sie eine Betreffzeile ein und doppelklicken Sie auf den bearbeitbaren Bereich der E-Mail.

   ![](assets/five-2.png)

   _Im E-Mail-Editor wird ein Rich-Text-Editor geöffnet._

1. Markieren Sie den vorhandenen E-Mail-Inhalt.

   ![](assets/six-2.png)

1. Geben Sie Ihren E-Mail-Inhalt ein und klicken Sie auf Speichern.

   ![](assets/seven-2.png)

1. Ihre Änderungen werden automatisch gespeichert. Schließen Sie den Tab/Fenster des E-Mail-Editors.

   ![](assets/eight-1.png)

1. Wählen Sie Ihre neue E-Mail aus. Klicken Sie unter &quot;E-Mail-Aktionen&quot;auf Genehmigen .

   ![](assets/image2014-9-24-11-3a55-3a16.png)

## Schritt 2: Intelligente Kampagne erstellen {#step-create-a-smart-campaign}

1. Rechtsklick **Mein Programm** und klicken Sie auf **Neue intelligente Kampagne**.

   ![](assets/image2014-9-24-11-3a56-3a13.png)

1. **Name** Ihre Smart-Kampagne &quot;Automatische Antwortkampagne&quot;und klicken Sie auf **Erstellen**.

   ![](assets/image2014-9-24-11-3a56-3a25.png)

1. Wechseln Sie zur Registerkarte **Intelligente Liste**.

   ![](assets/image2014-9-24-11-3a56-3a38.png)

   Wir richten diese Kampagne so ein, dass sie immer dann ausgeführt wird, wenn eine Person das in [**Landingpage mit einem Formular**](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;}.

1. Suchen und Ziehen **Formular ausfüllen** Trigger zur linken Arbeitsfläche.

   ![](assets/image2014-9-24-11-3a57-3a18.png)

1. Auswählen **Mein Formular** in der Dropdown-Liste. Klicken Sie auf die Registerkarte **“Flow“**.

   ![](assets/image2014-9-24-11-3a57-3a29.png)

1. Ziehen Sie die **E-Mail senden** Flussaktion auf die linke Arbeitsfläche.

   ![](assets/image2014-9-24-11-3a57-3a41.png)

1. Wählen Sie Ihre **Automatische Antwort-E-Mail** und gehen Sie zu **Zeitplan** Registerkarte.

   ![](assets/image2014-9-24-11-3a57-3a53.png)

1. Klicken **Bearbeiten**.

   ![](assets/8.png)

1. Wählen Sie **Immer** aus und klicken Sie dann auf **Speichern**.

   ![](assets/9.png)

1. Klicken Sie auf **Aktivieren**.

   ![](assets/10.png)

1. Klicken **Aktivieren** auf dem Bestätigungsbildschirm.

   ![](assets/11.png)

>[!NOTE]
>
>Nach der Aktivierung wird diese Kampagne jedes Mal ausgeführt, wenn eine Person das angegebene Formular ausfüllt. Die Kampagne läuft so lange, bis sie deaktiviert wird.

## Schritt 3: Formular ausfüllen {#step-fill-out-the-form}

1. Auswählen **Meine Seite**. Dies wurde im [Landingpage mit einem Formular](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target=&quot;_blank&quot;} schneller Sieg.

   ![](assets/image2014-9-24-12-3a0-3a8.png)

1. Klicken Sie auf **“Genehmigte Seite anzeigen“**.

   ![](assets/image2014-9-24-12-3a0-3a18.png)

   Ihre Landingpage &quot;Kostenlose Testversion&quot;wird in einem neuen Tab geöffnet.

1. Füllen Sie das Formular mit Vorname, Nachname und E-Mail-Adresse aus und klicken Sie auf **Einsenden**.

   ![](assets/image2014-9-24-12-3a0-3a28.png)

>[!NOTE]
>
>Stellen Sie sicher, dass Sie Ihre richtige E-Mail-Adresse verwenden, damit Sie E-Mails empfangen können.

## Aufgabe abgeschlossen {#mission-complete}

Innerhalb weniger Minuten sollte die automatische Antwort-E-Mail in Ihrem Posteingang angezeigt werden. Großartig gemacht!

<br> 

[◄ Aufgabe 3: Einfache Bewertung](/help/marketo/getting-started/quick-wins/simple-scoring.md)

[Auftrag 5: Import a List of People ►](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)
