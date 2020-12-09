---
unique-page-id: 4720232
description: Erstellen einer Liste für ein neues Konto - Marketing Docs - Produktdokumentation
title: Eine Liste für ein neues Konto erstellen
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---


# Eine Liste für ein neues Konto erstellen {#create-a-new-account-list}

Erstellen Sie eine Liste von Organisations- und Domänennamen und laden Sie sie hoch, um diese wichtigen Konten mit personalisierten Kampagnen Zielgruppe.

>[!NOTE]
>
>Dieser Artikel gilt nur für ältere Web ABM-Kunden. Wenn Sie Web ABM nach September 2016 erworben haben, befolgen Sie bitte die Schritte in [diesem Artikel](http://docs.marketo.com/display/DOCS/Account+Lists#AccountLists-CreateaNewAccountList) .

## Eine Liste für ein neues Konto erstellen {#create-a-new-account-list-1}

1. Gehen Sie zu **Kontoeinstellungen**.

   ![](assets/dropdown-account-lists-hand.jpg)

1. Wählen Sie Neu **erstellen**.

   ![](assets/create-new-account-list-hand.jpg)

1. Wählen Sie &quot; **Durchsuchen** &quot;und laden Sie die CSV-Datei hoch (stellen Sie sicher, dass die CSV-Datei die Kriterien erfüllt). hinzufügen einen **Namen** und eine **Beschreibung**. Klicken Sie auf **Speichern**.

   ![](assets/create-account-list-hands.jpg)

   >[!NOTE]
   >
   >**Welches Format hat die CSV-Datei?**
   >
   >
   >Vergewissern Sie sich, dass die benannte CSV-Datei die folgenden Anforderungen erfüllt:
   >
   >* Als CSV-Format gespeichert
   >* Höchstens 10 MB
   >* Nur 4 Spalten mit der Kopfzeile Spalte A: Name, Spalte B: Domäne, Spalte C: Land, Spalte D: US-Staat.
   >* Datei-Uploads können bis zu 2 Werktage vor der Genehmigung dauern.
   >* Sie erhalten eine Genehmigungs-E-Mail-Benachrichtigung oder einen Prüfstatus auf der Seite &quot;Benannte Konten&quot;.
   >* Die Gesamtanzahl der Datensätze/Zeilen, die für alle Listen mit 10K hochgeladen wurden, wobei das größte Paket insgesamt 100K betrug.


   >[!NOTE]
   >
   >**Beispiel**
   >
   >**Beispiel der CSV-Datei**
   >
   >* Zeile 1 Spalte A Wert = Organisation
   >* Zeile 1 Spalte B Wert = Domäne
   >* Zeile 1 Spalte C Wert = Land
   >* Zeile 1 Spalte D Wert = US-Status
   >* Einer der Spaltenwerte ist obligatorisch. Wenn Sie jedoch sowohl Organisations- als auch Domänennamen angeben, werden die Übereinstimmungsraten in der Liste &quot;Konto&quot;verbessert.
   >* Land und Bundesland sind optionale Werte.

      >
      >  
   * Verwenden Sie für den Ländernamen den vollständigen Ländernamen oder den Abkürzungscode. z. USA oder USA.
   >  * Für einen US-Bundesstaat verwenden Sie den 2-Buchstaben-Abkürzungscode, d.h. CA. Nur US-Bundesstaaten werden anerkannt.

   >    
   >![](assets/image2015-2-25-12-3a19-3a10.png)

## Bearbeiten einer Konto-Liste {#edit-an-account-list}

Klicken Sie auf der Seite **Kontoeinstellungen** auf das Symbol **Bearbeiten **auf der Liste.

![](assets/create-new-account-list-edit.jpg)

Wählen Sie **Durchsuchen** und laden Sie die neue CSV-Datei hoch. Diese Datei ersetzt die Originaldatei. Klicken Sie auf **Speichern**. Die neue hochgeladene Datei befindet sich in einem ausstehenden Zustand, bis sie von der Marketing Support-Abteilung genehmigt wurde, wenn die Originaldatei in einem ausstehenden Status aktiv bleibt.

![](assets/set-account-list-edit-hands.jpg)

Die CSV-Datei ersetzt die vorhandene Datei. Die bestehende Liste bleibt solange aktiv, bis die Verarbeitung der neuen Datei abgeschlossen ist.

## Eine Liste für ein benanntes Konto löschen {#delete-a-named-account-list}

1. Klicken Sie auf der Seite **Kontoeinstellungen **auf das Symbol **Löschen **der Liste, die Sie löschen möchten.

   ![](assets/create-new-account-list-delete.jpg)

1. Es wird eine Meldung angezeigt, die bestätigt, ob Sie die Liste löschen möchten. Klicken Sie auf **OK**.

   ![](assets/delete-notification-hand.jpg)

>[!MORELIKETHIS]
>
>* [Erstellen eines Segments mit einer Kontoversion einer Liste](create-a-segment-using-an-account-list.md)
>* [Ansicht einer Liste mit einem benannten Konto](http://docs.marketo.com/pages/viewpage.action?pageid=4720244)

