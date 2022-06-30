---
unique-page-id: 2359418
description: Importieren einer Personenliste - Marketo Docs - Produktdokumentation
title: Eine Personenliste importieren
exl-id: a85ec787-7b22-4666-84fd-d7bf23d32cd4
source-git-commit: 0da33dfa840dd1e5a5618fcd762b482f7a2e0789
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Eine Personenliste importieren {#import-a-list-of-people}

## Auftrag: Importieren Sie eine Tabellenliste mit den Teilnehmern einer Fachmesse in Ihre Datenbank. {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[Einrichten und Hinzufügen einer Person](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target=&quot;_blank&quot;}

In diesem Tutorial erfahren Sie, wie Sie Personen aus einer Tabellendatei in Marketo importieren.

## Schritt 1: Herunterladen und Bearbeiten einer Tabelle {#step-download-and-edit-a-spreadsheet}

1. Laden Sie zunächst unsere Übungs-Tabellendatei ([**tradeshow-attendes.csv**](/help/marketo/getting-started/assets/tradeshow-attendees.csv){target=&quot;_blank&quot;}) auf Ihrem Computer installiert.

   ![](assets/image2014-9-24-12-3a5-3a0.png)

   >[!NOTE]
   >
   >Verwenden Sie beim Import eines Datums folgendes Format: **21.09.20** (Monat/Tag/Jahr).

   >[!NOTE]
   >
   >Alle Datums-/Uhrzeitfelder, die importiert werden, werden als Central Time behandelt. Wenn Sie Datums-/Uhrzeitfelder in einer anderen Zeitzone haben, können Sie eine Excel-Formel verwenden, um sie in Central Time (America/Chicago) umzuwandeln.

1. Fügen Sie Ihren eigenen Vornamen, Nachnamen, Ihre tatsächliche E-Mail-Adresse (sodass Sie die Pflege-E-Mails erhalten können, die Sie in der nächsten Mission senden werden) und Ihre Berufsbezeichnung hinzu. Speichern Sie die Datei auf Ihrem Computer.

   ![](assets/image2014-9-24-12-3a5-3a30.png)

   >[!CAUTION]
   >
   >Marketo **not** unterstützen E-Mail-Adressen, die Emojis enthalten.

## Schritt 2: Programm erstellen {#step-create-a-program}

1. Navigieren Sie zu **Marketingaktivitäten** Bereich.

   ![](assets/ma-2.png)

1. Wählen Sie Ihre **Lernen** Ordner, dann unter **Neu** click **Neues Programm**.

   ![](assets/image2014-9-24-12-3a21-3a13.png)

1. **Name** das Programm &quot;My Tradeshow Program&quot; und wählen Sie &quot;Event&quot; für die **Programmtyp**.

   ![](assets/image2014-9-24-12-3a21-3a25.png)

1. Auswählen **Messen** für **Kanal** und klicken Sie auf **Erstellen**.

   ![](assets/image2014-9-24-12-3a21-3a39.png)

>[!NOTE]
>
>Ereignisprogramme treten an bestimmten Daten auf. Weitere Informationen [**Veranstaltungen**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md){target=&quot;_blank&quot;}.

## Schritt 3: Importieren Ihrer Tabelle in Marketo {#step-import-your-spreadsheet-into-marketo}

1. In **Eigenes Schulungsprogramm** klicken **Neu** und wählen Sie **Neues lokales Asset**.

   ![](assets/seven-3.png)

1. Klicken **Liste**.

   ![](assets/image2014-9-24-12-3a22-3a56.png)

1. **Name** die Liste &quot;Messen - Teilnehmer&quot;und klicken Sie auf **Erstellen**.

   ![](assets/image2014-9-24-12-3a23-3a9.png)

1. In **Messebesucher** Liste, klicken Sie auf **Aktionen auflisten** und wählen Sie **Importliste**.

   ![](assets/ten-2.png)

   >[!CAUTION]
   >
   >Wenn Sie Ihre eigene CSV-Datei verwenden, stellen Sie sicher, dass sie UTF-8-, UTF-16-, Shift-JIS- oder EUC-JP-kodiert ist.

   >[!NOTE]
   >
   >Die maximale Größe für CSV-Dateien beträgt 100 MB.

1. **Durchsuchen** der **tradeshow-attendes.csv** Tabellendatei auf Ihrem Computer und klicken Sie auf **Nächste**.

   ![](assets/eleven-2.png)

   >[!NOTE]
   >
   >Wählen Sie im Listenimportmodus die Option **Neue Personen und Updates überspringen** bedeutet, dass Sie keine Auswirkungen auf vorhandene Personendatensätze oder Aktivitäten protokollieren. Verwenden Sie diesen Modus, wenn Sie eine schnelle, vorgefilterte statische Liste vorhandener Personen zur Verwendung in Ihren Marketing-Aktivitäten wünschen. Durch Auswahl dieses Modus wird Folgendes ausgeführt:
   >
   > * Neue Personenerstellung überspringen
   > * Personen-Feldaktualisierungen überspringen
   > * Aktivitätsprotokollierung überspringen


1. Ordnen Sie die Listenspaltenfelder dem entsprechenden Marketo-Feld zu und klicken Sie auf **Nächste**.

   ![](assets/image2014-9-24-12-3a24-3a49.png)

   >[!TIP]
   >
   >Spaltenüberschriften sollten immer genau mit dem Feld übereinstimmen (Groß-/Kleinschreibung beachten), um die besten Ergebnisse für die automatische Zuordnung zu erzielen. Wenn Sie benutzerdefinierte Felder verwenden und sie nicht in der Dropdown-Liste sehen, gehen Sie zurück und [erstellen](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target=&quot;_blank&quot;}, damit sie Optionen werden können.

   >[!NOTE]
   >
   >Wenn es Felder gibt, die Sie nicht importieren möchten, wählen Sie **Ignorieren** im Dropdown-Menü Marketo-Feld.

1. Auswählen **Eigenes Schulungsprogramm** für **Akquiseprogramm** Klicken Sie auf **Import**.

   ![](assets/image2014-9-24-12-3a25-3a1.png)

1. Warten Sie, bis Ihre Personen importiert haben, und schließen Sie dann das Popup-Fenster für den Importfortschritt.

   ![](assets/image2014-9-24-12-3a25-3a13.png)

1. Zurück in **Eigenes Schulungsprogramm**, klicken Sie auf die **Mitglieder** Registerkarte. Du wirst alle Leute sehen, die du gerade importiert hast.

   ![](assets/fifteen-1.png)

>[!NOTE]
>
>Sie können den Erfolg Ihres Programms analysieren, indem Sie die Mitgliedschaft im Programm verfolgen. Weitere Informationen [**Programme**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target=&quot;_blank&quot;}.

## Aufgabe abgeschlossen {#mission-complete}

Ihre Messeteilnehmer sind nun Mitglieder Ihres Marketo-Programms!

<br> 

[Auftrag 4: Automatische E-Mail-Antwort](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[Aufgabe 6: Schrittweises Lead-Nurturing ►](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)
