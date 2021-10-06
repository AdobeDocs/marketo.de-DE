---
unique-page-id: 2359418
description: Importieren einer Personenliste - Marketo Docs - Produktdokumentation
title: Eine Personenliste importieren
exl-id: a85ec787-7b22-4666-84fd-d7bf23d32cd4
source-git-commit: 1b37a750c5e609b9e43e942df752305d85153989
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 5%

---

# Eine Personenliste importieren {#import-a-list-of-people}

## Auftrag: Importieren Sie eine Tabellenliste mit den Teilnehmern einer Fachmesse in Ihre Datenbank. {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[Einrichten und Hinzufügen einer Person](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md)

In diesem Tutorial erfahren Sie, wie Sie Personen aus einer Tabellendatei in Marketo importieren.

## Schritt 1: Herunterladen und Bearbeiten einer Tabelle {#step-download-and-edit-a-spreadsheet}

1. Laden Sie zunächst unsere Übungs-Tabellendatei ([**tradeshow-attendes.csv**](/help/marketo/getting-started/assets/tradeshow-attendees.csv)) auf Ihren Computer herunter.

   ![](assets/image2014-9-24-12-3a5-3a0.png)

   >[!NOTE]
   >
   >Verwenden Sie beim Import eines Datums folgendes Format: **9/21/20** (Monat/Tag/Jahr).

   >[!NOTE]
   >
   >Alle Datums-/Uhrzeitfelder, die importiert werden, werden als Central Time behandelt. Wenn Sie Datums-/Uhrzeitfelder in einer anderen Zeitzone haben, können Sie eine Excel-Formel verwenden, um sie in Central Time (America/Chicago) umzuwandeln.

1. Fügen Sie Ihren eigenen Vornamen, Nachnamen, Ihre E-Mail-Adresse und Ihre Berufsbezeichnung hinzu und speichern Sie dann die Datei auf Ihrem Computer.

   ![](assets/image2014-9-24-12-3a5-3a30.png)

>[!NOTE]
>
>Geben Sie Ihre echte E-Mail-Adresse in die CSV-Datei ein, damit Sie die Pflege-E-Mails erhalten können, die Sie in der nächsten Mission versenden werden.

## Schritt 2: Programm erstellen {#step-create-a-program}

1. Gehen Sie zum Bereich **Marketingaktivitäten** .

   ![](assets/ma-2.png)

1. Wählen Sie den Ordner **Learning** und klicken Sie dann unter **New** auf **Neues Programm**.

   ![](assets/image2014-9-24-12-3a21-3a13.png)

1. **** Benennen Sie das Programm &quot;My Tradeshow Program&quot; und wählen Sie &quot;Event&quot; für den  **Programmtyp**.

   ![](assets/image2014-9-24-12-3a21-3a25.png)

1. Wählen Sie **Tradeshow** für **Kanal** und klicken Sie auf **Erstellen**.

   ![](assets/image2014-9-24-12-3a21-3a39.png)

>[!NOTE]
>
>Ereignisprogramme treten an bestimmten Daten auf. Erfahren Sie mehr über [**Ereignisse**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md).

## Schritt 3: Importieren Ihrer Tabelle in Marketo {#step-import-your-spreadsheet-into-marketo}

1. Klicken Sie in **My Tradeshow Program** auf **New** und wählen Sie **New Local Asset** aus.

   ![](assets/seven-3.png)

1. Klicken Sie auf **List**.

   ![](assets/image2014-9-24-12-3a22-3a56.png)

1. **** Benennen Sie die Liste &quot;Messebesucher&quot;und klicken Sie auf  **Erstellen**.

   ![](assets/image2014-9-24-12-3a23-3a9.png)

1. Klicken Sie in der Liste **Tradeshow-Teilnehmer** auf **Listenaktionen** und wählen Sie **Importliste** aus.

   ![](assets/ten-2.png)

   >[!CAUTION]
   >
   >Wenn Sie Ihre eigene CSV-Datei verwenden, stellen Sie sicher, dass sie UTF-8-, UTF-16-, Shift-JIS- oder EUC-JP-kodiert ist.

   >[!NOTE]
   >
   >Die maximale Größe für CSV-Dateien beträgt 100 MB.

1. **** Navigieren Sie zur Datei  **tradeshow-attendes.** csvspreadsheet auf Ihrem Computer und klicken Sie auf  **Weiter**.

   ![](assets/eleven-2.png)

   >[!NOTE]
   >
   >Wenn Sie im Listenimportmodus **Neue Personen und Updates überspringen** auswählen, haben Sie keine Auswirkungen auf vorhandene Personendatensätze oder Aktivitäten. Verwenden Sie diesen Modus, wenn Sie eine schnelle, vorgefilterte statische Liste vorhandener Personen zur Verwendung in Ihren Marketing-Aktivitäten wünschen. Durch Auswahl dieses Modus wird Folgendes ausgeführt:
   >
   > * Neue Personenerstellung überspringen
   > * Personen-Feldaktualisierungen überspringen
   > * Aktivitätsprotokollierung überspringen


1. Ordnen Sie Ihre Listenspaltenfelder dem entsprechenden Marketo-Feld zu und klicken Sie auf **Weiter**.

   ![](assets/image2014-9-24-12-3a24-3a49.png)

   >[!TIP]
   >
   >Spaltenüberschriften sollten immer genau mit dem Feld übereinstimmen (Groß-/Kleinschreibung beachten), um die besten Ergebnisse für die automatische Zuordnung zu erzielen. Wenn Sie benutzerdefinierte Felder verwenden und sie nicht in der Dropdown-Liste sehen, gehen Sie zurück und [erstellen Sie sie](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md), damit sie Optionen werden können.

   >[!NOTE]
   >
   >Wenn es Felder gibt, die Sie nicht importieren möchten, wählen Sie im Dropdown-Menü Marketo-Feld die Option **Ignorieren**.

1. Wählen Sie **My Tradeshow Program** für das **Akquiseprogramm** und klicken Sie dann auf **Import**.

   ![](assets/image2014-9-24-12-3a25-3a1.png)

1. Warten Sie, bis Ihre Personen importiert haben, und schließen Sie dann das Popup-Fenster für den Importfortschritt.

   ![](assets/image2014-9-24-12-3a25-3a13.png)

1. Klicken Sie in **My Tradeshow Program** auf den Tab **Mitglieder** . Du wirst alle Leute sehen, die du gerade importiert hast.

   ![](assets/fifteen-1.png)

>[!NOTE]
>
>Sie können den Erfolg Ihres Programms analysieren, indem Sie die Mitgliedschaft im Programm verfolgen. Erfahren Sie mehr über [**Programme**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md).

## Aufgabe abgeschlossen {#mission-complete}

Ihre Messeteilnehmer sind nun Mitglieder Ihres Marketo-Programms!

<br> 

[Auftrag 4: Automatische E-Mail-Antwort](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[Aufgabe 6: Schrittweises Lead-Nurturing ►](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)
