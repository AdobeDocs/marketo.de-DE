---
unique-page-id: 2359418
description: Liste von Personen importieren - Marketo-Dokumente - Produktdokumentation
title: Liste mit Personen importieren
exl-id: a85ec787-7b22-4666-84fd-d7bf23d32cd4
feature: Getting Started
source-git-commit: 292626741d3b2334da104a515c3e968fb340706a
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 4%

---

# Liste mit Personen importieren {#import-a-list-of-people}

## Mission: Importieren Sie eine Tabellenliste der Messeteilnehmer in Ihre Datenbank {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[Einrichten und Person hinzufügen](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}

In diesem Tutorial erfahren Sie, wie Sie Personen aus einer Tabellenkalkulationsdatei in Marketo importieren.

## Schritt 1: Herunterladen und Bearbeiten einer Tabelle {#step-download-and-edit-a-spreadsheet}

1. Laden Sie zunächst unsere Übungstabelle ([**tradeshow-attendes.csv**](/help/marketo/getting-started/assets/tradeshow-attendees.csv){target="_blank"}) auf Ihren Computer herunter.

   ![](assets/import-a-list-of-people-1.png)

   >[!NOTE]
   >
   >Verwenden Sie beim Importieren eines Datums dieses Format: **9/21/20** (Monat/Tag/Jahr).

   >[!NOTE]
   >
   >Alle Datums-/Uhrzeitfelder, die importiert werden, werden als zentrale Zeit behandelt. Wenn Sie Datums-/Zeitfelder in einer anderen Zeitzone haben, können Sie eine Excel-Formel verwenden, um sie in Central Time (America/Chicago) umzuwandeln.

1. Fügen Sie Ihren eigenen Vornamen, Nachnamen, die tatsächliche E-Mail-Adresse (damit Sie die pflegenden E-Mails erhalten können, die Sie in der nächsten Mission senden werden) und den Stellentitel hinzu. Speichern Sie die Datei auf Ihrem Computer.

   ![](assets/import-a-list-of-people-2.png)

   >[!CAUTION]
   >
   >* Stellen Sie sicher, dass E-Mail-Adressen nur ASCII-Zeichen enthalten.
   >
   >* Marketo unterstützt **nicht** E-Mail-Adressen, die Emojis enthalten.
   >
   >* Der Import von `NULL` über CSV könnte zu einer „Änderung des Datenwerts“ für numerische Felder im „Aktivitätsprotokoll[ einer Person führen ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/locate-the-activity-log-for-a-person.md){target="_blank"}auch _wenn die Felder bereits leer sind_. Wenn Sie über [Smart-Kampagnen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/understanding-smart-campaigns.md){target="_blank"} verfügen, die den Filter „Datenwertänderung“ oder den Trigger „Datenwertänderungen“ verwenden, kann dies dazu führen, dass sich Personen für diese Kampagnen qualifizieren, obwohl sich die Daten tatsächlich nicht ändern. Sie können [Beschränkungen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md){target="_blank"} verwenden, um sicherzustellen, dass sich beim Import niemand für diese Kampagnen qualifiziert.

## Schritt 2: Programm erstellen {#step-create-a-program}

1. Navigieren Sie zum Bereich **[!UICONTROL Marketing]** Aktivitäten.

   ![](assets/import-a-list-of-people-3.png)

1. Wählen Sie **Ordner** Lernen“ aus und klicken Sie dann unter **[!UICONTROL Neu]** auf **[!UICONTROL Neues Programm]**.

   ![](assets/import-a-list-of-people-4.png)

1. **Name** das Programm „Mein Messeprogramm“ und wählen Sie „Event“ für den **[!UICONTROL Programmtyp]**.

   ![](assets/import-a-list-of-people-5.png)

1. Wählen Sie **[!UICONTROL Fachmesse]** für den **[!UICONTROL Kanal]** und klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/import-a-list-of-people-6.png)

>[!NOTE]
>
>Veranstaltungsprogramme finden an bestimmten Daten statt. Weitere Informationen über [**Ereignisse**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md){target="_blank"}.

## Schritt 3: Importieren Sie Ihre Tabelle in Marketo {#step-import-your-spreadsheet-into-marketo}

1. Klicken **im** „Mein Messeprogramm“ auf **[!UICONTROL Neu]** und wählen Sie **[!UICONTROL Neues lokales Asset]**.

   ![](assets/import-a-list-of-people-7.png)

1. Wählen Sie **[!UICONTROL Liste]** aus.

   ![](assets/import-a-list-of-people-8.png)

1. **Name** die Liste „Messeteilnehmer“ und klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/import-a-list-of-people-9.png)

1. Klicken Sie in **[!UICONTROL Liste &quot;]**&quot; auf **[!UICONTROL Aktionen auflisten]** und wählen Sie **[!UICONTROL Liste importieren]**.

   ![](assets/import-a-list-of-people-10.png)

   >[!CAUTION]
   >
   >Wenn Sie Ihre eigene CSV-Datei verwenden, stellen Sie sicher, dass diese mit UTF-8, UTF-16, Shift-JIS oder EUC-JP codiert ist.

   >[!NOTE]
   >
   >Die Größenbeschränkung für CSV-Dateien beträgt 100 MB.

1. **[!UICONTROL Navigieren Sie]** Tabellendatei **tradeshow-attendes.csv** auf Ihrem Computer und klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/import-a-list-of-people-11.png)

   >[!NOTE]
   >
   >Im Listenimportmodus bedeutet die Auswahl von **[!UICONTROL Neue Personen und Aktualisierungen überspringen]**, dass keine Auswirkungen auf bestehende Personendatensätze haben und keine Aktivitäten protokolliert werden. Verwenden Sie diesen Modus, wenn Sie eine schnelle, vorab gefilterte statische Liste der vorhandenen Personen zur Verwendung in Ihren Marketing-Aktivitäten wünschen. Durch Auswahl dieses Modus geschieht Folgendes:
   >
   > * Erstellung neuer Personen überspringen
   > * Personen-Feldaktualisierungen überspringen
   > * Aktivitätsprotokollierung überspringen

1. Ordnen Sie Ihre [!UICONTROL Listenspalte]-Felder dem entsprechenden Marketo-Feld zu und klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/import-a-list-of-people-12.png)

   >[!TIP]
   >
   >Spaltenüberschriften sollten immer genau mit dem Feld übereinstimmen (Groß-/Kleinschreibung beachten), um die besten Ergebnisse der automatischen Zuordnung zu erzielen. Wenn Sie benutzerdefinierte Felder verwenden und sie nicht in der Dropdown-Liste angezeigt werden, gehen Sie zurück und [ Sie sie, ](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target="_blank"} sie zu Optionen werden können.

   >[!NOTE]
   >
   >Wenn Felder vorhanden sind, die nicht importiert werden sollen, wählen Sie **Dropdown-Menü** Marketo-Feld“ die Option „Ignorieren“ aus.

1. Wählen Sie **Mein Messeprogramm** für das **[!UICONTROL Akquiseprogramm]** und klicken Sie dann auf **[!UICONTROL Importieren]**.

   ![](assets/import-a-list-of-people-13.png)

1. Warten Sie, bis Ihre Benutzer importiert wurden, und schließen Sie dann das Popup Importfortschritt .

   ![](assets/import-a-list-of-people-14.png)

1. Zurück in **Mein Messeprogramm** klicken Sie auf die Registerkarte **[!UICONTROL Mitglieder]**. Sie werden alle Leute sehen, die Sie gerade importiert haben.

   ![](assets/import-a-list-of-people-15.png)

>[!NOTE]
>
>Sie können den Erfolg Ihres Programms analysieren, indem Sie die Programmmitgliedschaft verfolgen. Weitere Informationen über [**Programme**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target="_blank"}.

## Aufgabe abgeschlossen {#mission-complete}

Ihre Messeteilnehmer sind nun Mitglieder Ihres Marketo-Programms!

<br> 

[◄ Mission 4: Automatische E-Mail-Antwort](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[Mission 6: Tropfen, Tropfen, ►](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)
