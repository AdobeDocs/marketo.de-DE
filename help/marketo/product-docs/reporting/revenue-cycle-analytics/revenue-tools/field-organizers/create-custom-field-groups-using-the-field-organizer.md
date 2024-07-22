---
unique-page-id: 10094404
description: Erstellen benutzerdefinierter Feldergruppen mit dem Field Organizer - Marketo Docs - Produktdokumentation
title: Erstellen benutzerdefinierter Feldergruppen mit dem Feld-Organizer
exl-id: 0425a446-2c92-4a2a-85c4-e05c22118035
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '1000'
ht-degree: 3%

---

# Erstellen benutzerdefinierter Feldergruppen mit dem Feld-Organizer {#create-custom-field-groups-using-the-field-organizer}

Bevor Sie benutzerdefinierte Feldergruppen für die Berichterstellung im Bereich &quot;Modell-Leistungsanalyse&quot;(Leads) des Umsatz-Cycle-Explorers aktivieren können, müssen Sie Standardfelder oder benutzerdefinierte Felder über den Field Organizer in Marketo Lead Management in Gruppen für die Berichterstellung kategorisieren. Dies gilt nur für Lead- und Firmenattribute.
Wenn Sie im Dialogfeld &quot;New Field Organizer&quot;aus der Dropdown-Liste &quot;Feld&quot;ein standardmäßiges oder benutzerdefiniertes Feld auswählen, ordnet das System den Marketo-Lead-Management-Datentyp zu, der dem Feld zugeordnet ist, das Sie mit einem der drei verfügbaren Editoren im Field Organizer gruppieren möchten: Zeichenfolge, Ganzzahl oder Datum.

| Marketo Lead Management-Datentyp | Datentyp &quot;Field Organizer Editor&quot; |
|---|---|
| Zeichenfolge | Zeichenfolge |
| E-Mail | Zeichenfolge |
| Ganze Zahl | Ganze Zahl |
| Text | Zeichenfolge |
| URL | Zeichenfolge |
| Referenz | Nicht unterstützt |
| Währung | Ganze Zahl |
| Datum/Uhrzeit | Datum |
| Boolesch | Nicht unterstützt |
| Telefon | Zeichenfolge |
| Datum | Datum |
| Gleitkomma | Ganze Zahl |
| Berechnet | Nicht unterstützt |

In den nächsten drei Abschnitten wird beschrieben, wie Sie eine benutzerdefinierte Feldergruppe für einen String, eine Ganzzahl oder einen Datumstyp erstellen.

## Benutzerdefinierte Feldergruppe erstellen - Zeichenfolgen-Editor {#create-custom-field-group-string-editor}

1. Klicken Sie auf **Lead-Datenbank**.

   ![](assets/one.png)

1. Klicken Sie auf **Neu** und wählen Sie **Neuer Feld-Organizer** aus.

   ![](assets/two.png)

1. Klicken Sie auf **Feld** und wählen Sie ein standardmäßiges oder benutzerdefiniertes Feld mit einem Datentyp aus, der dem Zeichenfolgen-Editor zugeordnet ist (siehe Tabelle im vorherigen Abschnitt). Land wird hier verwendet.

   ![](assets/three.png)

1. Klicken Sie auf **Erstellen**.

   ![](assets/four.png)

   Die neue benutzerspezifische Gruppe wird in der Struktur &quot;Lead-Datenbank&quot;als Feldname > Feldernamengruppe angezeigt (Beispiel: Land > Ländergruppe).

   ![](assets/4.5.png)

1. Klicken Sie auf das Stiftsymbol, um den Namen anzupassen. Sie können beispielsweise &quot;Ländergruppe&quot;in &quot;Kontinent&quot;umbenennen. Geben Sie den gewünschten neuen Namen ein und klicken Sie auf das Feld, um es automatisch zu speichern.

   ![](assets/five.png)

1. Standardmäßig werden alle Datenwerte in die Untergruppe &quot;Sonstige&quot;eingefügt. Um die Datenwerte zu kategorisieren, klicken Sie auf **Gruppe hinzufügen** , um eine Untergruppe zu erstellen und ihr einen Namen zu geben.

   >[!NOTE]
   >
   >Sie können bis zu zehn Untergruppen hinzufügen, um die Datenwerte zu kategorisieren. Jeder erstellten Untergruppe wird eine ID-Nummer zugewiesen.

   In diesem Beispiel wurden Gruppen für die meisten Kontinente erstellt.

   ![](assets/six.png)

   >[!NOTE]
   >
   >Um eine Untergruppe zu löschen, klicken Sie einfach auf das rote X neben dem Untergruppennamen. Wenn die Gruppe Datenwerte enthält, werden die Datenwerte in die Standardgruppe Sonstige verschoben.

1. Markieren Sie einen oder mehrere Datenwerte auf der Arbeitsfläche und ziehen Sie die Datenwerte in die entsprechende Untergruppe.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Um einen Datenwert aus einer Untergruppe zu entfernen, weisen Sie den Datenwert der Standardgruppe Sonstige zu.

1. Verwenden Sie die Filteroption oben links direkt über der Arbeitsfläche, um die Datenwerte in einer oder mehreren Untergruppen auszuwählen und anzuzeigen. Die Datenwerte, die auf Ihrer Filterauswahl basieren, werden auf der Arbeitsfläche angezeigt.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Nachdem die Gruppen definiert wurden, können Sie die benutzerdefinierte Feldergruppe für die Berichterstellung in der Modell-Leistungsanalyse (Leads) über die Registerkarte &quot;Umsatzwyklusanalyse&quot;in Marketo Lead Management aktivieren.

## Benutzerdefinierte Feldergruppe erstellen - Ganzzahleditor {#create-custom-field-group-integer-editor}

1. Klicken Sie auf **Lead-Datenbank**.

   ![](assets/one.png)

1. Klicken Sie auf **Neu** und wählen Sie **Neuer Feld-Organizer** aus.

   ![](assets/two.png)

1. Klicken Sie auf **Feld** und wählen Sie ein standardmäßiges oder benutzerdefiniertes Feld mit einem Datentyp aus, der dem Zeichenfolgen-Editor zugeordnet ist (siehe Tabelle im vorherigen Abschnitt). Hier wird der Jahresumsatz verwendet.

   ![](assets/nine.png)

1. Klicken Sie auf **Erstellen**.

   ![](assets/9.5.png)

   Die neue benutzerspezifische Gruppe wird in der Baumstruktur der Lead-Datenbank angezeigt, die als Feldname > Feldnamengruppe dargestellt wird (Beispiel: Jahresumsatz > Jährliche Umsatzgruppe).

   ![](assets/9.6.png)

1. Klicken Sie auf den standardmäßigen benutzerspezifischen Gruppennamen über dem Integer-Editor, um den Namen anzupassen. Sie können beispielsweise &quot;Jährliche Umsatzgruppe&quot;in &quot;Jahresumsatz nach Größe&quot;umbenennen. Klicken Sie auf **Speichern**.

   ![](assets/eleven.png)

   Mit dem Integer-Editor können Sie mehrere Untergruppen erstellen, um jede Untergruppe nach Größe zu definieren. In diesem Beispiel werden drei Gruppen für kleine, Medium- und Enterprise-Unternehmen erstellt.

1. Um Ihre erste Gruppe hinzuzufügen, geben Sie einen Namen in das Feld **Gruppenname** ein (Beispiel: Klein) und geben Sie einen Höchstwert in das Feld **Gruppenbereich** ein (Beispiel: 200000). Klicken Sie auf **Gruppe hinzufügen**.

   ![](assets/twelve.png)

   Unter der soeben eingegebenen Gruppe wird ein leerer Gruppeneintrag angezeigt. Das folgende Beispiel zeigt einen Eintrag für kleine, Medium- und Enterprise-Unternehmen.

   >[!NOTE]
   >
   >Sie können bis zu zehn Untergruppen hinzufügen, um die Datenwerte zu kategorisieren. Jeder Gruppenbereichseintrag basiert auf dem vorherigen Eintrag. Wenn Sie den letzten Eintrag für den Gruppenbereich für die letzte von Ihnen erstellte benutzerdefinierte Untergruppe leer lassen, wird kein maximaler Datenwert festgelegt.

1. Klicken Sie auf die Registerkarte Zusammenfassung , um Ihre Einstellungen zu speichern und zu überprüfen.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Um eine Untergruppe zu löschen, klicken Sie auf das rote X neben dem Namen der Untergruppe.

1. Überprüfen Sie auf der Seite &quot;Zusammenfassung&quot;Ihre Einstellungen.

   ![](assets/13.5.png)

   >[!NOTE]
   >
   >Nachdem die Gruppen definiert wurden, können Sie die benutzerdefinierte Feldergruppe für die Berichterstellung in der Modell-Leistungsanalyse (Leads) über die Registerkarte &quot;Umsatzwyklusanalyse&quot;in Marketo Lead Management aktivieren.

## Benutzerdefinierte Feldergruppe erstellen - Datumseditor {#create-custom-field-group-date-editor}

1. Klicken Sie auf **Lead-Datenbank**.

   ![](assets/one.png)

1. Klicken Sie auf **Neu** und wählen Sie **Neuer Feld-Organizer** aus.

   ![](assets/two.png)

1. Klicken Sie auf **Feld** und wählen Sie ein standardmäßiges oder benutzerdefiniertes Feld mit einem Datentyp aus, der dem Zeichenfolgen-Editor zugeordnet ist (siehe Tabelle im vorherigen Abschnitt). Das Akquisedatum wird hier verwendet.

   ![](assets/fourteen.png)

1. Klicken Sie auf **Erstellen**.

   ![](assets/14.5.png)

   Die neue benutzerdefinierte Gruppe wird in der Struktur der Lead-Datenbank angezeigt, die als Feldname > Feldernamengruppe dargestellt wird (Beispiel: Akquisedatum > Akquise-Datumgruppe).

   ![](assets/14.6.png)

1. Klicken Sie auf den standardmäßigen Namen der benutzerspezifischen Gruppe über dem Datumseditor, um den Namen anzupassen. Sie können beispielsweise &quot;Akquise-Datumgruppe&quot;in &quot;Akquise-Datumskategorien&quot;umbenennen. Klicken Sie auf **Speichern**.

   ![](assets/fifteen.png)

   Mit dem Datumseditor können Sie mehrere Untergruppen erstellen und jede Untergruppe nach Datum definieren. In diesem Beispiel werden drei Gruppen erstellt: Q1-15 Leads, Q2-15 Leads und Q3-15 Leads.

1. Um Ihre erste Gruppe hinzuzufügen, geben Sie einen Namen in das Feld **Gruppenname** ein (Beispiel: Q1-15 Leads) und geben Sie ein Datum in das Datumsfeld ein, das das Datum darstellt, an dem der Lead erworben wurde (Beispiel: 3/31/2015 für den letzten Tag von Q1-15). Klicken Sie auf **Gruppe hinzufügen**.

   ![](assets/sixteen.png)

   >[!NOTE]
   >
   >Sie können bis zu zehn Untergruppen hinzufügen, um die Datenwerte zu kategorisieren. Jeder Gruppenbereichseintrag basiert auf dem vorherigen Eintrag. Wenn Sie den letzten Eintrag für den Gruppenbereich für die letzte von Ihnen erstellte benutzerspezifische Untergruppe leer lassen, wird kein Enddatumswert festgelegt.

   Das folgende Beispiel zeigt einen Eintrag für Q1 2015-Leads durch Q3.

   ![](assets/16.5.png)

   Und das ist es! Gute Arbeit.
