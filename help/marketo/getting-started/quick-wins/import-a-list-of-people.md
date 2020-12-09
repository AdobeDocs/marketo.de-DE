---
unique-page-id: 2359418
description: Liste von Personen importieren - Marketing-Dokumente - Produktdokumentation
title: Eine Liste von Personen importieren
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---


# Eine Liste von Personen importieren {#import-a-list-of-people}

## Auftrag: Eine Liste der Messebesucher in Ihre Datenbank importieren {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!NOTE]
>
>**FYI**
>
>Marketo standardisiert nun die Sprache für alle Abonnements, sodass Sie möglicherweise Interessenten in Ihrem Abonnement und Personen/Personen in docs.marketo.com sehen können. Diese Begriffe bedeuten dasselbe. Es hat keine Auswirkungen auf die Artikelanweisungen. Es gibt auch noch einige andere Änderungen. [Weitere Informationen](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!PREREQUISITES]
>
>* [Einrichten und Hinzufügen einer Person](get-set-up-and-add-a-person.md)

>



`   
`  In diesem Lernprogramm erfahren Sie, wie Sie Personen aus einer Tabellenkalkulationsdatei in Marketo importieren.

## Schritt 1: Herunterladen und Bearbeiten einer Tabelle {#step-download-and-edit-a-spreadsheet}

1. Um Beginn zu erhalten, laden Sie unsere Übungsdatenblattdatei (** [tradeshow-attendes.csv](http://docs.marketo.com/display/docs/assets/tradeshow-attendees.csv)**) auf Ihren Computer herunter.

   ![](assets/image2014-9-24-12-3a5-3a0.png)

   >[!NOTE]
   >
   >**Erinnerung**
   >
   >
   >Verwenden Sie beim Importieren eines Datums folgendes Format: **21.09.15** (Monat/Tag/Jahr).

   >[!NOTE]
   >
   >Alle importierten Datums-/Uhrzeitfelder werden als &quot;Central Time&quot;behandelt. Wenn Sie Datums-/Uhrzeitfelder in einer anderen Zeitzone haben, können Sie eine Excel-Formel verwenden, um sie in Central Time (Amerika/Chicago) umzuwandeln.

1. hinzufügen Sie Ihren eigenen Vornamen, Nachnamen, Ihre E-Mail-Adresse und Ihren Auftragsnamen und speichern Sie die Datei dann auf Ihrem Computer.

   ![](assets/image2014-9-24-12-3a5-3a30.png)

>[!NOTE]
>
>Geben Sie Ihre echte E-Mail-Adresse in die CSV-Datei ein, damit Sie die Pflege-E-Mails erhalten können, die Sie bei der nächsten Mission senden werden.

## Schritt 2: Programm erstellen {#step-create-a-program}

1. Gehen Sie zum Bereich **Marketing-Aktivitäten** .

   ![](assets/ma-2.png)

1. Wählen Sie Ihren **Lernordner** und klicken Sie dann unter **Neu** auf **Neues Programm**.

   ![](assets/image2014-9-24-12-3a21-3a13.png)

1. **Benennen** Sie das Programm &quot;Mein Programm für die Diashow&quot;und wählen Sie &quot;Ereignis&quot;für den **Programm-Typ.**

   ![](assets/image2014-9-24-12-3a21-3a25.png)

1. Wählen Sie **Tradeshow** für den **Kanal** und klicken Sie auf **Erstellen**.

   ![](assets/image2014-9-24-12-3a21-3a39.png)

>[!NOTE]
>
>**Tieftauchen**
>
>Ereignis-Programm treten an bestimmten Daten auf. Weitere Informationen zu [**Ereignissen**](http://docs.marketo.com/display/docs/events).

## Schritt 3: Importieren der Tabelle in Marketing {#step-import-your-spreadsheet-into-marketo}

1. Klicken Sie im Programm **** Meine Präsentation auf **Neu** und wählen Sie **Neues lokales Asset**.

   ![](assets/seven-3.png)

1. Klicken Sie auf **Liste**.

   ![](assets/image2014-9-24-12-3a22-3a56.png)

1. **Benennen** Sie die Liste &quot;Händler-Teilnehmer&quot;und klicken Sie auf **Erstellen**.

   ![](assets/image2014-9-24-12-3a23-3a9.png)

1. Klicken Sie in der Liste der **Teilnehmer** auf **Listen** und wählen Sie Liste **** importieren.

   ![](assets/ten-2.png)

   >[!CAUTION]
   >
   >Wenn Sie Ihre eigene CSV-Datei verwenden, stellen Sie sicher, dass sie UTF-8-, UTF-16-, Shift-JIS- oder EUC-JP-kodiert ist.

   >[!NOTE]
   >
   >Die maximale Größe für CSV-Dateien beträgt 100 MB.

1. **Navigieren Sie** zur **Datei &quot;tradeshow-attendes.csv** &quot;auf Ihrem Computer und klicken Sie auf **Weiter**.

   ![](assets/eleven-2.png)

   >[!NOTE]
   >
   >Wenn Sie im Liste-Importmodus die Option &quot;Neue Personen und Updates **** überspringen&quot;wählen, wirkt sich dies nicht auf vorhandene Personendaten aus oder protokolliert keine Aktivitäten. Verwenden Sie diesen Modus, wenn Sie eine schnelle, vorgefilterte statische Liste von vorhandenen Personen zur Verwendung in Ihren Marketing-Aktivitäten benötigen. Die Auswahl dieses Modus führt zu:
   >
   >    
   >    
   >    * Neue Personenerstellung überspringen
   >    * Aktualisierung des Benutzerfelds überspringen
   >    * Protokollierung von Aktivitäten überspringen


1. Ordnen Sie die Spaltenfelder Ihrer Liste dem jeweiligen Markierungsfeld zu und klicken Sie auf **Weiter**.

   ![](assets/image2014-9-24-12-3a24-3a49.png)

   >[!TIP]
   >
   >Spaltenüberschriften sollten immer exakt mit dem Feld übereinstimmen (Groß-/Kleinschreibung beachten), um die besten Ergebnisse für die automatische Zuordnung zu erzielen. Wenn Sie benutzerdefinierte Felder verwenden und sie nicht in der Dropdown-Liste sehen, gehen Sie zurück und [erstellen Sie sie](http://docs.marketo.com/display/DOCS/Create+a+Custom+Field+in+Marketo) , damit sie Optionen werden können.

   >[!NOTE]
   >
   >Wenn es Felder gibt, die Sie nicht importieren möchten, wählen Sie im Dropdown-Menü &quot;Feld markieren&quot;die Option &quot; **Ignorieren** &quot;.

1. Wählen Sie **Mein Tradeshow-Programm** für das **Akquise-Programm** und klicken Sie dann auf **Importieren**.

   ![](assets/image2014-9-24-12-3a25-3a1.png)

1. Warten Sie, bis die Personen importiert wurden, und schließen Sie dann das Popup für den Importstatus.

   ![](assets/image2014-9-24-12-3a25-3a13.png)

1. Klicken Sie in **Mein Programm** auf die Registerkarte **Mitglieder** . Du wirst alle Leute sehen, die du gerade importiert hast.

   ![](assets/fifteen-1.png)

>[!NOTE]
>
>**Tieftauchen**
>
>Sie können den Erfolg Ihres Programms analysieren, indem Sie die Programm-Mitgliedschaft verfolgen. Weitere Informationen zu [**Programmen**](http://docs.marketo.com/display/docs/programs).

## Abschluss der Mission {#mission-complete}

Ihre Messebesucher sind jetzt Mitglieder Ihres Marketo Programms!

<br> 

[Auftrag 4: Email Auto Response](email-auto-response.md) [Mission 6: Tropfen, Tropfen, Nurtur ►](drip-drip-nurture.md)