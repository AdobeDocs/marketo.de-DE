---
unique-page-id: 2359416
description: E-Mail für automatische Reaktion - Marketo-Dokumente - Produktdokumentation
title: Automatische Antwort-E-Mail
exl-id: c9c0a154-65ec-4845-97a0-a2100223cb13
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 19%

---

# Automatische Antwort-E-Mail {#email-auto-response}

## Auftrag: Senden Sie eine Dankesemail, wenn eine Person ein Formular {#mission-send-out-a-thank-you-email-when-a-person-fills-out-a-form} ausfüllt

>[!PREREQUISITES]
>
>* [Einrichten und Hinzufügen einer Person](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md)
>* [Landing Page mit Formular](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)


## Schritt 1: E-Mail erstellen {#step-create-an-email}

1. Gehen Sie zum Bereich Marketing-Aktivitäten.

   ![](assets/one-2.png)

1. Wählen Sie im linken Menü &quot;Mein Programm&quot;aus, klicken Sie auf die Dropdownliste &quot;Neu&quot;und wählen Sie &quot;Neues lokales Asset&quot;.

   ![](assets/two-3.png)

1. Klicken Sie auf die E-Mail.

   ![](assets/three-2.png)

1. Benennen Sie Ihre E-Mail mit &quot;Auto Response Email&quot;, wählen Sie eine Vorlage und klicken Sie auf Erstellen.

   ![](assets/four-1.png)

   Ein E-Mail-Editor wird in einem neuen Fenster oder auf einer neuen Registerkarte geöffnet. Wenn Popups blockiert sind, klicken Sie auf der Seite mit der Asset-Zusammenfassung auf **Entwurf bearbeiten**, um auf die E-Mail zuzugreifen.

1. Geben Sie eine Betreffzeile ein und klicken Sie dann bei gedrückter Dublette auf den bearbeitbaren Bereich der E-Mail.

   ![](assets/five-2.png)

   _Über dem E-Mail-Editor wird ein Rich-Text-Editor geöffnet._

1. Markieren Sie den vorhandenen E-Mail-Inhalt.

   ![](assets/six-2.png)

1. Geben Sie Ihren E-Mail-Inhalt ein und klicken Sie auf Speichern.

   ![](assets/seven-2.png)

1. Ihre Änderungen werden automatisch gespeichert. Schließen Sie die Registerkarte/das Fenster des E-Mail-Editors.

   ![](assets/eight-1.png)

1. Wählen Sie Ihre neue E-Mail aus. Klicken Sie unter &quot;E-Mail-Aktionen&quot;auf Genehmigen.

   ![](assets/image2014-9-24-11-3a55-3a16.png)

## Schritt 2: Intelligente Kampagne erstellen {#step-create-a-smart-campaign}

1. Klicken Sie mit der rechten Maustaste auf **Mein Programm** und klicken Sie auf **Neue Smart-Kampagne**.

   ![](assets/image2014-9-24-11-3a56-3a13.png)

1. **Benennen Sie** Ihre intelligente Kampagne &quot;Auto Response Kampagne&quot; und klicken Sie auf  **Erstellen**.

   ![](assets/image2014-9-24-11-3a56-3a25.png)

1. Wechseln Sie zur Registerkarte **Intelligente Liste**.

   ![](assets/image2014-9-24-11-3a56-3a38.png)

   Diese Kampagne wird ausgeführt, wenn ein Benutzer das in [**Landingpage erstellte Formular mit einem Formular**](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md) ausfüllt.

1. Suchen Sie den Trigger **Ausfüllen des Formulars** und ziehen Sie ihn auf die linke Arbeitsfläche.

   ![](assets/image2014-9-24-11-3a57-3a18.png)

1. Wählen Sie **Mein Formular** in der Dropdownliste aus. Klicken Sie auf die Registerkarte **“Flow“**.

   ![](assets/image2014-9-24-11-3a57-3a29.png)

1. Ziehen Sie die Aktion **E-Mail senden** in die linke Arbeitsfläche.

   ![](assets/image2014-9-24-11-3a57-3a41.png)

1. Wählen Sie **E-Mail zur automatischen Antwort** und gehen Sie zur Registerkarte **Plan**.

   ![](assets/image2014-9-24-11-3a57-3a53.png)

1. Klicken Sie auf **Bearbeiten**.

   ![](assets/8.png)

1. Wählen Sie **Immer** aus und klicken Sie dann auf **Speichern**.

   ![](assets/9.png)

1. Klicken Sie auf **Aktivieren**.

   ![](assets/10.png)

1. Klicken Sie im Bestätigungsbildschirm auf **Aktivieren**.

   ![](assets/11.png)

>[!NOTE]
>
>Sobald diese Kampagne aktiv ist, wird sie jedes Mal ausgeführt, wenn eine Person das angegebene Formular ausfüllt. Die Kampagne läuft, bis sie deaktiviert ist.

## Schritt 3: Formular ausfüllen {#step-fill-out-the-form}

1. Wählen Sie **Meine Seite**. Dies wurde in der [Landingpage mit einem Formular](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md) Quick win erstellt.

   ![](assets/image2014-9-24-12-3a0-3a8.png)

1. Klicken Sie auf **“Genehmigte Seite anzeigen“**.

   ![](assets/image2014-9-24-12-3a0-3a18.png)

   Ihre Landingpage &quot;Kostenlose Testversion&quot;wird in einem neuen Register geöffnet.

1. Füllen Sie das Formular mit Ihrem Vornamen, Nachnamen und Ihrer E-Mail-Adresse aus und klicken Sie dann auf **Senden**.

   ![](assets/image2014-9-24-12-3a0-3a28.png)

>[!NOTE]
>
>Stellen Sie sicher, dass Sie Ihre richtige E-Mail-Adresse verwenden, damit Sie E-Mails empfangen können.

## Aufgabe abgeschlossen  {#mission-complete}

Innerhalb weniger Minuten sollten Sie die automatische Antwort-E-Mail in Ihrem Posteingang sehen. Großartig gemacht!

<br> 

[◄ Aufgabe 3: Einfache Bewertung](/help/marketo/getting-started/quick-wins/simple-scoring.md)

[Aufgabe 5: Liste mit Leads importieren ►](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)
