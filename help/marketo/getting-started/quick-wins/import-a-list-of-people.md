---
unique-page-id: 2359418
description: Importieren einer Personenliste - Marketo Docs - Produktdokumentation
title: Eine Personenliste importieren
exl-id: a85ec787-7b22-4666-84fd-d7bf23d32cd4
feature: Getting Started
source-git-commit: 6733bca40fbe09fd1c5b6166aef7a74759d7808e
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 4%

---

# Eine Personenliste importieren {#import-a-list-of-people}

## Auftrag: Importieren Sie eine Tabellenkalkulation der Messebesucher in Ihre Datenbank {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[Einrichten und Hinzufügen einer Person](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}

In diesem Tutorial erfahren Sie, wie Sie Personen aus einer Tabellendatei in Marketo importieren.

## Schritt 1: Herunterladen und Bearbeiten einer Tabelle {#step-download-and-edit-a-spreadsheet}

1. Laden Sie zunächst unsere Übungsdatei ([**tradeshow-attendes.csv**](/help/marketo/getting-started/assets/tradeshow-attendees.csv){target="_blank"}) auf Ihren Computer herunter.

   ![](assets/import-a-list-of-people-1.png)

   >[!NOTE]
   >
   >Verwenden Sie beim Import eines Datums folgendes Format: **9/21/20** (Monat/Tag/Jahr).

   >[!NOTE]
   >
   >Alle Datums-/Uhrzeitfelder, die importiert werden, werden als Central Time behandelt. Wenn Sie Datums-/Uhrzeitfelder in einer anderen Zeitzone haben, können Sie eine Excel-Formel verwenden, um sie in Central Time (America/Chicago) umzuwandeln.

1. Fügen Sie Ihren eigenen Vornamen, Nachnamen, Ihre tatsächliche E-Mail-Adresse (sodass Sie die Pflege-E-Mails erhalten können, die Sie in der nächsten Mission senden werden) und Ihre Berufsbezeichnung hinzu. Speichern Sie die Datei auf Ihrem Computer.

   ![](assets/import-a-list-of-people-2.png)

   >[!CAUTION]
   >
   >* Stellen Sie sicher, dass E-Mail-Adressen nur ASCII-Zeichen enthalten.
   >
   >* Marketo unterstützt **nicht** E-Mail-Adressen, die Emojis enthalten.

## Schritt 2: Programm erstellen {#step-create-a-program}

1. Wechseln Sie zum Bereich **[!UICONTROL Marketingaktivitäten]** .

   ![](assets/import-a-list-of-people-3.png)

1. Wählen Sie Ihren Ordner **Lernen** aus und klicken Sie unter **[!UICONTROL Neu]** auf **[!UICONTROL Neues Programm]**.

   ![](assets/import-a-list-of-people-4.png)

1. **Name** das Programm &quot;My Tradeshow Program&quot;und wählen Sie &quot;Event&quot;für den **[!UICONTROL Programmtyp]** aus.

   ![](assets/import-a-list-of-people-5.png)

1. Wählen Sie **[!UICONTROL Tradeshow]** für den Kanal **[!UICONTROL 3} aus und klicken Sie auf**[!UICONTROL  Erstellen ]**.]**

   ![](assets/import-a-list-of-people-6.png)

>[!NOTE]
>
>Ereignisprogramme treten an bestimmten Daten auf. Erfahren Sie mehr über [**Ereignisse**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md){target="_blank"}.

## Schritt 3: Importieren Ihrer Tabelle in Marketo {#step-import-your-spreadsheet-into-marketo}

1. Klicken Sie in **My Tradeshow Program** auf **[!UICONTROL New]** und wählen Sie **[!UICONTROL New Local Asset]**.

   ![](assets/import-a-list-of-people-7.png)

1. Wählen Sie **[!UICONTROL Liste]** aus.

   ![](assets/import-a-list-of-people-8.png)

1. **Name** die Liste &quot;Messen, wie Teilnehmer&quot;und klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/import-a-list-of-people-9.png)

1. Klicken Sie in der Liste **[!UICONTROL Messebesuche]** auf **[!UICONTROL Listenaktionen]** und wählen Sie **[!UICONTROL Importliste]** aus.

   ![](assets/import-a-list-of-people-10.png)

   >[!CAUTION]
   >
   >Wenn Sie Ihre eigene CSV-Datei verwenden, stellen Sie sicher, dass sie UTF-8-, UTF-16-, Shift-JIS- oder EUC-JP-kodiert ist.

   >[!NOTE]
   >
   >Die maximale Größe für CSV-Dateien beträgt 100 MB.

1. **[!UICONTROL Durchsuchen Sie]** die Tabellendatei **tradeshow-attendes.csv** auf Ihrem Computer und klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/import-a-list-of-people-11.png)

   >[!NOTE]
   >
   >Wenn Sie im Listenimportmodus die Option **[!UICONTROL Neue Personen und Updates überspringen]** auswählen, haben Sie keine Auswirkungen auf vorhandene Personendatensätze und protokollieren keine Aktivitäten. Verwenden Sie diesen Modus, wenn Sie eine schnelle, vorgefilterte statische Liste vorhandener Personen zur Verwendung in Ihren Marketing-Aktivitäten wünschen. Durch Auswahl dieses Modus wird Folgendes ausgeführt:
   >
   > * Neue Personenerstellung überspringen
   > * Personen-Feldaktualisierungen überspringen
   > * Aktivitätsprotokollierung überspringen

1. Ordnen Sie Ihre Felder für die [!UICONTROL Listenspalte] ihrem jeweiligen Marketo-Feld zu und klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/import-a-list-of-people-12.png)

   >[!TIP]
   >
   >Spaltenüberschriften sollten immer genau mit dem Feld übereinstimmen (Groß-/Kleinschreibung beachten), um die besten Ergebnisse für die automatische Zuordnung zu erzielen. Wenn Sie benutzerdefinierte Felder verwenden und sie nicht in der Dropdown-Liste sehen, gehen Sie zurück und [erstellen Sie sie](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target="_blank"} , damit sie Optionen werden können.

   >[!NOTE]
   >
   >Wenn es Felder gibt, die Sie nicht importieren möchten, wählen Sie im Dropdown-Menü Marketo-Feld die Option **Ignorieren** aus.

1. Wählen Sie **My Tradeshow Program** für das **[!UICONTROL Akquise-Programm]** und klicken Sie dann auf **[!UICONTROL Import]**.

   ![](assets/import-a-list-of-people-13.png)

1. Warten Sie, bis Ihre Personen importiert haben, und schließen Sie dann das Popup-Fenster für den Importfortschritt.

   ![](assets/import-a-list-of-people-14.png)

1. Klicken Sie in **My Tradeshow Program** auf die Registerkarte **[!UICONTROL Members]** . Du wirst alle Leute sehen, die du gerade importiert hast.

   ![](assets/import-a-list-of-people-15.png)

>[!NOTE]
>
>Sie können den Erfolg Ihres Programms analysieren, indem Sie die Mitgliedschaft im Programm verfolgen. Erfahren Sie mehr über [**Programme**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target="_blank"}.

## Aufgabe abgeschlossen {#mission-complete}

Ihre Messeteilnehmer sind nun Mitglieder Ihres Marketo-Programms!

<br> 

[Auftrag 4: Automatische E-Mail-Antwort](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[Mission 6: Drip, Drip, Nurture ►](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)
