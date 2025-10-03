---
unique-page-id: 2359416
description: Automatische Antwort-E-Mail – Marketo-Dokumente – Produktdokumentation
title: Automatische Antwort-E-Mail
exl-id: c9c0a154-65ec-4845-97a0-a2100223cb13
feature: Getting Started
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: ht
source-wordcount: '380'
ht-degree: 100%

---

# Automatische Antwort-E-Mail {#email-auto-response}

## Aufgabe: Senden einer Danksagungs-E-Mail, wenn jemand ein Formular ausfüllt {#mission-send-out-a-thank-you-email-when-a-person-fills-out-a-form}

>[!PREREQUISITES]
>
>* [Einrichten und eine Person hinzufügen](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [Landingpage mit einem Formular](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## Schritt 1: Erstellen einer E-Mail {#step-create-an-email}

1. Navigieren Sie zum Bereich [!UICONTROL Marketing-Aktivitäten].

   ![](assets/email-auto-response-1.png)

1. Wählen Sie im linken Menü Ihr Programm aus, klicken Sie auf die Dropwdown-Liste **[!UICONTROL Neu]** und wählen Sie **[!UICONTROL Neues lokales Asset]**.

   ![](assets/email-auto-response-2.png)

1. Wählen Sie **[!UICONTROL E-Mail]** aus.

   ![](assets/email-auto-response-3.png)

1. Nennen Sie Ihre E-Mail „Automatische Antwort-E-Mail“, wählen Sie eine Vorlage aus und klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/email-auto-response-4.png)

   Ein E-Mail-Editor wird in einem neuen Fenster oder in einer neuen Registerkarte geöffnet. Wenn Popup-Fenster blockiert sind, klicken Sie auf der Seite mit der Asset-Zusammenfassung auf **[!UICONTROL Entwurf bearbeiten]**, um die E-Mail aufzurufen.

1. Geben Sie eine Betreffzeile ein und doppelklicken Sie dann auf den bearbeitbaren Bereich der E-Mail.

   ![](assets/email-auto-response-5.png)

   _Ein Rich-Text-Editor wird über dem E-Mail-Editor geöffnet._

1. Markieren Sie den vorhandenen E-Mail-Inhalt.

   ![](assets/email-auto-response-6.png)

1. Geben Sie Ihren E-Mail-Inhalt ein und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/email-auto-response-7.png)

1. Klicken Sie auf das Dropdown-Menü **[!UICONTROL E-Mail-Aktionen]** und wählen Sie **[!UICONTROL Genehmigen und schließen]**.

   ![](assets/email-auto-response-8.png)

## Schritt 2: Erstellen einer intelligenten Kampagne {#step-create-a-smart-campaign}

1. Wählen Sie Ihr Programm aus, klicken Sie auf das Dropdown-Menü **[!UICONTROL Neu]** und wählen Sie **[!UICONTROL Neue intelligente Kampagne]**.

   ![](assets/email-auto-response-9.png)

1. **Nennen** Sie die intelligente Kampagne „Automatische Antwortkampagne“ und klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/email-auto-response-10.png)

1. Gehen Sie zur Registerkarte **[!UICONTROL Intelligente Liste]**.

   ![](assets/email-auto-response-11.png)

   Wir richten diese Kampagne so ein, dass sie immer dann ausgeführt wird, wenn eine Person das Formular ausfüllt, das Sie unter [**Landingpage mit einem Formular**](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"} erstellt haben.

1. Suchen Sie den Auslöser **[!UICONTROL Füllt Formular aus]** und ziehen Sie ihn auf die Arbeitsfläche.

   ![](assets/email-auto-response-12.png)

1. Wählen Sie **[!UICONTROL Mein Formular]** in der Dropdown-Liste aus. Klicken Sie dann auf die Registerkarte **[!UICONTROL Fluss]**.

   ![](assets/email-auto-response-13.png)

1. Ziehen Sie die Flussaktion **[!UICONTROL E-Mail senden]** in die linke Arbeitsfläche.

   ![](assets/email-auto-response-14.png)

1. Wählen Sie Ihre **Automatische Antwort-E-Mail** aus. Klicken Sie dann auf die Registerkarte **[!UICONTROL Zeitplan]**.

   ![](assets/email-auto-response-15.png)

1. Klicken Sie auf **[!UICONTROL Bearbeiten]**.

   ![](assets/email-auto-response-16.png)

1. Wählen Sie **[!UICONTROL immer]** aus und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/email-auto-response-17.png)

1. Klicken Sie auf **[!UICONTROL Aktivieren]**.

   ![](assets/email-auto-response-18.png)

1. Klicken Sie auf dem Bestätigungsbildschirm auf **[!UICONTROL Aktivieren]**.

   ![](assets/email-auto-response-19.png)

>[!NOTE]
>
>Sobald die Kampagne aktiv ist, wird sie jedes Mal ausgeführt, wenn eine Person ein bestimmtes Formular ausfüllt. Die Kampagne läuft so lange, bis sie deaktiviert wird.

## Schritt 3: Ausfüllen des Formulars {#step-fill-out-the-form}

1. Wählen Sie **Meine Seite** (diese wurde im Schnellverfahren [Landingpage mit einem Formular](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"} erstellt) und klicken Sie auf **[!UICONTROL Vorschau]**.

   ![](assets/email-auto-response-20.png)

   _Ihre Landingpage „Kostenlose Testversion“ wird in einer neuen Registerkarte geöffnet._

1. Füllen Sie das Formular mit Ihrem Vornamen, Nachnamen und Ihrer E-Mail-Adresse aus und klicken Sie auf **[!UICONTROL Senden]**.

   ![](assets/email-auto-response-21.png)

>[!NOTE]
>
>Stellen Sie sicher, dass Sie Ihre richtige E-Mail-Adresse verwenden, damit Sie E-Mails empfangen können.

## Aufgabe abgeschlossen {#mission-complete}

Innerhalb weniger Minuten sollten Sie die automatische Antwort-E-Mail in Ihrem Posteingang sehen.

[◄ Aufgabe 3: Einfache Bewertung](/help/marketo/getting-started/quick-wins/simple-scoring.md)

[Aufgabe 5: Importieren einer Liste mit Personen ►](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)
