---
unique-page-id: 2359418
description: Liste von Personen importieren - Marketing-Dokumente - Produktdokumentation
title: Eine Liste von Personen importieren
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---


# Eine Liste von Personen {#import-a-list-of-people} importieren

## Auftrag: Eine Liste der Messebesucher in eine Tabellenkalkulationsdatenbank importieren {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[Einrichten und Hinzufügen einer Person](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md)

In diesem Lernprogramm erfahren Sie, wie Sie Personen aus einer Tabellenkalkulationsdatei in Marketo importieren.

## Schritt 1: Herunterladen und Bearbeiten einer Tabelle {#step-download-and-edit-a-spreadsheet}

1. Um Beginn zu erhalten, laden Sie unsere Übungsdatenblattdatei ([**tradeshow-attendes.csv**](https://docs.marketo.com/display/docs/assets/tradeshow-attendees.csv)) auf Ihren Computer herunter.

   ![](assets/image2014-9-24-12-3a5-3a0.png)

   >[!NOTE]
   >
   >Verwenden Sie beim Importieren eines Datums folgendes Format: **9/21/20** (Monat/Tag/Jahr).

   >[!NOTE]
   >
   >Alle importierten Datums-/Uhrzeitfelder werden als &quot;Central Time&quot;behandelt. Wenn Sie Datums-/Uhrzeitfelder in einer anderen Zeitzone haben, können Sie eine Excel-Formel verwenden, um sie in Central Time (Amerika/Chicago) umzuwandeln.

1. hinzufügen Sie Ihren eigenen Vornamen, Nachnamen, Ihre E-Mail-Adresse und Ihren Auftragsnamen und speichern Sie die Datei dann auf Ihrem Computer.

   ![](assets/image2014-9-24-12-3a5-3a30.png)

>[!NOTE]
>
>Geben Sie Ihre echte E-Mail-Adresse in die CSV-Datei ein, damit Sie die Pflege-E-Mails erhalten können, die Sie bei der nächsten Mission senden werden.

## Schritt 2: Programm {#step-create-a-program} erstellen

1. Gehen Sie zum Bereich **Marketing-Aktivitäten**.

   ![](assets/ma-2.png)

1. Wählen Sie den Ordner **Lernen** und klicken Sie dann unter **Neu** auf **Neues Programm**.

   ![](assets/image2014-9-24-12-3a21-3a13.png)

1. **Benennen Sie** das Programm &quot;My Tradeshow Programm&quot;und wählen Sie &quot;Ereignis&quot;als  **Programm**.

   ![](assets/image2014-9-24-12-3a21-3a25.png)

1. Wählen Sie **Tradeshow** für **Kanal** und klicken Sie auf **Erstellen**.

   ![](assets/image2014-9-24-12-3a21-3a39.png)

>[!NOTE]
>
>Ereignis-Programm treten an bestimmten Daten auf. Erfahren Sie mehr über [**Ereignis**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md).

## Schritt 3: Importieren Sie Ihre Tabelle in das Marketing {#step-import-your-spreadsheet-into-marketo}

1. Klicken Sie in **Mein Programm für die Diashow** auf **Neu** und wählen Sie **Neues lokales Element**.

   ![](assets/seven-3.png)

1. Klicken Sie auf **Liste**.

   ![](assets/image2014-9-24-12-3a22-3a56.png)

1. **Benennen Sie** die Liste &quot;Händler-Teilnehmer&quot;und klicken Sie auf  **Erstellen**.

   ![](assets/image2014-9-24-12-3a23-3a9.png)

1. Klicken Sie in der Liste **Händler-Teilnehmer** auf **Listen-Aktionen** und wählen Sie **Liste importieren**.

   ![](assets/ten-2.png)

   >[!CAUTION]
   >
   >Wenn Sie Ihre eigene CSV-Datei verwenden, stellen Sie sicher, dass sie UTF-8-, UTF-16-, Shift-JIS- oder EUC-JP-kodiert ist.

   >[!NOTE]
   >
   >Die maximale Größe für CSV-Dateien beträgt 100 MB.

1. **Navigieren Sie** zu der Datei  **tradeshow-attendes.** csvspreadsheet auf Ihrem Computer und klicken Sie auf  **Weiter**.

   ![](assets/eleven-2.png)

   >[!NOTE]
   >
   >Wenn Sie im Listen-Importmodus **Neue Personen und Updates überspringen** wählen, haben Sie keine Auswirkungen auf vorhandene Personendaten oder auf Aktivitäten. Verwenden Sie diesen Modus, wenn Sie eine schnelle, vorgefilterte statische Liste von vorhandenen Personen zur Verwendung in Ihren Marketing-Aktivitäten benötigen. Die Auswahl dieses Modus führt zu:
   >
   > * Neue Personenerstellung überspringen
   > * Aktualisierung des Benutzerfelds überspringen
   > * Protokollierung von Aktivitäten überspringen


1. Ordnen Sie die Spaltenfelder Ihrer Liste dem jeweiligen Markierungsfeld zu und klicken Sie auf **Weiter**.

   ![](assets/image2014-9-24-12-3a24-3a49.png)

   >[!TIP]
   >
   >Spaltenüberschriften sollten immer exakt mit dem Feld übereinstimmen (Groß-/Kleinschreibung beachten), um die besten Ergebnisse für die automatische Zuordnung zu erzielen. Wenn Sie benutzerdefinierte Felder verwenden und sie nicht in der Dropdown-Liste sehen, gehen Sie zurück und [erstellen Sie sie](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md), damit sie Optionen werden können.

   >[!NOTE]
   >
   >Wenn es Felder gibt, die Sie nicht importieren möchten, wählen Sie **Ignore** im Dropdownmenü &quot;Feld markieren&quot;.

1. Wählen Sie **Mein Tradeshow-Programm** für das **Akquise-Programm** und klicken Sie dann auf **Import**.

   ![](assets/image2014-9-24-12-3a25-3a1.png)

1. Warten Sie, bis die Personen importiert wurden, und schließen Sie dann das Popup für den Importstatus.

   ![](assets/image2014-9-24-12-3a25-3a13.png)

1. Zurück in **Mein Programm für die Diashow** klicken Sie auf die Registerkarte **Mitglieder**. Du wirst alle Leute sehen, die du gerade importiert hast.

   ![](assets/fifteen-1.png)

>[!NOTE]
>
>Sie können den Erfolg Ihres Programms analysieren, indem Sie die Programm-Mitgliedschaft verfolgen. Erfahren Sie mehr über [**Programm**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md).

## Dienstabschluss {#mission-complete}

Ihre Messebesucher sind jetzt Mitglieder Ihres Marketo Programms!

<br> 

[Auftrag 4: Automatische E-Mail-Antwort](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[Mission 6: Tropfen, Tropfen, Nurtur ►](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)
