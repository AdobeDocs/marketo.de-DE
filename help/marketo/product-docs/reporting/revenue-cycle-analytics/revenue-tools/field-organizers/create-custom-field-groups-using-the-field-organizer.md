---
unique-page-id: 10094404
description: Erstellen benutzerdefinierter Feldgruppen mit dem Feldorganisator - MarketingToDocs - Produktdokumentation
title: Erstellen benutzerdefinierter Feldgruppen mithilfe des Feldorganisierers
translation-type: tm+mt
source-git-commit: f28ff1acb0090892bdb92b75ef90d489db7abf20
workflow-type: tm+mt
source-wordcount: '992'
ht-degree: 0%

---


# Erstellen benutzerdefinierter Feldgruppen mit dem Feldorganisator {#create-custom-field-groups-using-the-field-organizer}

Bevor Sie benutzerdefinierte Feldgruppen für den Berichte im Bereich Modellleistung (Interessenten) des Umsatz-Cycle-Explorers aktivieren können, müssen Sie Standardfelder oder benutzerdefinierte Analysen für den Berichte über den Feldorganisator in der Marketing-Interessentenverwaltung in Gruppen kategorisieren. Dies gilt nur für die Attribute für Lead und Firma.
Wenn Sie ein Standard- oder benutzerdefiniertes Feld aus der Dropdown-Liste &quot;Feld&quot;im Dialogfeld &quot;Neuer Feld-Organizer&quot;auswählen, ordnet das System den Datentyp &quot;Anzeigen-zu-Interessentenverwaltung&quot;dem Feld zu, das Sie mit einem der drei verfügbaren Editoren im Feld-Organizer gruppieren möchten: Zeichenfolge, Ganzzahl oder Datum.

| Datentyp &quot;Marketing-Interessentenverwaltung&quot; | Datentyp &quot;Field Organizer Editor&quot; |
|---|---|
| Zeichenfolge | Zeichenfolge |
| Email | Zeichenfolge |
| Integer | Integer |
| Text | Zeichenfolge |
| URL | Zeichenfolge |
| Referenz | Nicht unterstützt |
| Währung | Integer |
| DateTime | Datum |
| Boolesch | Nicht unterstützt |
| Telefon | Zeichenfolge |
| Datum | Datum |
| Float | Integer |
| Berechnet | Nicht unterstützt |

In den nächsten drei Abschnitten wird beschrieben, wie Sie eine benutzerspezifische Feldgruppe für eine Zeichenfolge, eine Ganzzahl oder einen Datumstyp erstellen.

## Benutzerspezifische Feldgruppe erstellen - Zeichenfolgen-Editor {#create-custom-field-group-string-editor}

1. Klicken Sie auf **Interessentendatenbank**.

   ![](assets/one.png)

1. Klicken Sie auf **New** und wählen Sie **New Field Organizer**.

   ![](assets/two.png)

1. Klicken Sie auf **Feld** und wählen Sie ein Standard- oder benutzerdefiniertes Feld mit einem Datentyp aus, der dem Zeichenfolgeneditor zugeordnet ist (siehe Tabelle im vorherigen Abschnitt). Land wird hier verwendet.

   ![](assets/three.png)

1. Klicken Sie auf **Erstellen**.

   ![](assets/four.png)

   Die neue benutzerspezifische Gruppe wird in der Struktur der Interessentendatenbank angezeigt, die als Feldname > Feldnamengruppe dargestellt wird (Beispiel: Land > Ländergruppe).

   ![](assets/4.5.png)

1. Klicken Sie auf das Stiftsymbol, um den Namen anzupassen. Sie können beispielsweise &quot;Ländergruppe&quot;in &quot;Kontinent&quot;umbenennen. Geben Sie den gewünschten neuen Namen ein und klicken Sie zum automatischen Speichern auf eine andere Stelle.

   ![](assets/five.png)

1. Standardmäßig werden alle Datenwerte in der Untergruppe &quot;Sonstige&quot;platziert. Um die Datenwerte zu kategorisieren, klicken Sie auf **Hinzufügen Gruppe**, um eine Untergruppe zu erstellen und ihr einen Namen zu geben.

   >[!NOTE]
   >
   >Sie können bis zu zehn Untergruppen hinzufügen, um die Datenwerte zu kategorisieren. Jeder erstellten Untergruppe wird eine ID zugewiesen.

   In diesem Beispiel wurden Gruppen für die meisten Kontinente erstellt.

   ![](assets/six.png)

   >[!NOTE]
   >
   >Um eine Untergruppe zu löschen, klicken Sie einfach auf das rote X neben dem Namen der Untergruppe. Wenn die Gruppe Datenwerte enthält, werden die Datenwerte in die Standardgruppe Sonstige verschoben.

1. Markieren Sie einen oder mehrere Datenwerte auf der Arbeitsfläche und ziehen Sie die Datenwerte per Drag &amp; Drop in die entsprechende Untergruppe.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Um einen Datenwert aus einer Untergruppe zu entfernen, weisen Sie den Datenwert der Standardgruppe Sonstige zu.

1. Verwenden Sie die Filteroption in der oberen linken Ecke direkt über der Arbeitsfläche, um die Datenwerte in einer oder mehreren Untergruppen auszuwählen und Ansicht. Die Datenwerte, die auf Ihrer Filterauswahl basieren, werden auf der Arbeitsfläche angezeigt.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Nachdem die Gruppen definiert wurden, können Sie die benutzerspezifische Feldgruppe für den Berichte in der Modellleistung-Analyse (Interessenten) über die Registerkarte &quot;Analyse des Umsatzes&quot;in der Marketing-Interessentenverwaltung aktivieren.

## Benutzerspezifische Feldgruppe erstellen - Ganzzahleditor {#create-custom-field-group-integer-editor}

1. Klicken Sie auf **Interessentendatenbank**.

   ![](assets/one.png)

1. Klicken Sie auf **New** und wählen Sie **New Field Organizer**.

   ![](assets/two.png)

1. Klicken Sie auf **Feld** und wählen Sie ein Standard- oder benutzerdefiniertes Feld mit einem Datentyp aus, der dem Zeichenfolgeneditor zugeordnet ist (siehe Tabelle im vorherigen Abschnitt). Hier wird der Jahresumsatz verwendet.

   ![](assets/nine.png)

1. Klicken Sie auf **Erstellen**.

   ![](assets/9.5.png)

   Die neue benutzerspezifische Gruppe wird in der Struktur der Interessentendatenbank angezeigt, die als Feldname > Feldnamengruppe dargestellt wird (Beispiel: Jahresumsatz > Jährliche Umsatzgruppe).

   ![](assets/9.6.png)

1. Klicken Sie auf den standardmäßigen Namen der benutzerspezifischen Gruppe über dem Ganzzahleditor, um den Namen anzupassen. Sie können beispielsweise &quot;Jährliche Umsatzgruppe&quot;in &quot;Jahresumsatz nach Größe&quot;umbenennen. Klicken Sie auf **Speichern**.

   ![](assets/eleven.png)

   Mit dem Ganzzahleditor können Sie mehrere Untergruppen erstellen, um jede Untergruppe nach Größe zu definieren. In diesem Beispiel werden drei Gruppen für kleine, mittlere und große Unternehmen eingerichtet.

1. Um Ihre erste Gruppe hinzuzufügen, geben Sie einen Namen in das Feld **Gruppenname** ein (Beispiel: Klein) und geben Sie im Feld **Gruppenbereich** einen Maximalwert ein (Beispiel: 200000). Klicken Sie auf **Hinzufügen**.

   ![](assets/twelve.png)

   Unter der gerade eingegebenen Gruppe wird ein leerer Gruppeneintrag angezeigt. Das folgende Beispiel zeigt einen Eintrag für kleine, mittlere und Unternehmen.

   >[!NOTE]
   >
   >Sie können bis zu zehn Untergruppen hinzufügen, um die Datenwerte zu kategorisieren. Jeder Gruppenbereichseintrag baut auf dem vorherigen Eintrag auf. Wenn Sie den letzten Eintrag für den Gruppenbereich für die letzte von Ihnen erstellte benutzerspezifische Untergruppe leer lassen, wird kein Höchstwert für die Daten festgelegt.

1. Klicken Sie auf die Registerkarte Zusammenfassung, um Ihre Einstellungen zu speichern und zu überprüfen.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Um eine Untergruppe zu löschen, klicken Sie auf das rote X neben dem Namen der Untergruppe.

1. Überprüfen Sie auf der Seite &quot;Zusammenfassung&quot;Ihre Einstellungen.

   ![](assets/13.5.png)

   >[!NOTE]
   >
   >Nachdem die Gruppen definiert wurden, können Sie die benutzerspezifische Feldgruppe für den Berichte in der Modellleistung-Analyse (Interessenten) über die Registerkarte &quot;Analyse des Umsatzes&quot;in der Marketing-Interessentenverwaltung aktivieren.

## Benutzerspezifische Feldgruppe erstellen - Datumseditor {#create-custom-field-group-date-editor}

1. Klicken Sie auf **Interessentendatenbank**.

   ![](assets/one.png)

1. Klicken Sie auf **New** und wählen Sie **New Field Organizer**.

   ![](assets/two.png)

1. Klicken Sie auf **Feld** und wählen Sie ein Standard- oder benutzerdefiniertes Feld mit einem Datentyp aus, der dem Zeichenfolgeneditor zugeordnet ist (siehe Tabelle im vorherigen Abschnitt). Das Akquise-Datum wird hier verwendet.

   ![](assets/fourteen.png)

1. Klicken Sie auf **Erstellen**.

   ![](assets/14.5.png)

   Die neue benutzerspezifische Gruppe wird in der Struktur der Interessentendatenbank angezeigt, die als Feldname > Feldnamengruppe dargestellt wird (Beispiel: Akquise-Datum > Akquise-Datumgruppe).

   ![](assets/14.6.png)

1. Klicken Sie auf den standardmäßigen Namen der benutzerspezifischen Gruppe über dem Datumseditor, um den Namen anzupassen. Sie können beispielsweise &quot;Akquise-Datengruppe&quot;in &quot;Akquise-Datums-Kategorien&quot;umbenennen. Klicken Sie auf **Speichern**.

   ![](assets/fifteen.png)

   Mit dem Datumseditor können Sie mehrere Untergruppen erstellen und jede Untergruppe nach Datum definieren. In diesem Beispiel werden drei Gruppen erstellt: Q1-15 Leads, Q2-15 Leads und Q3-15 Leads.

1. Um Ihre erste Gruppe hinzuzufügen, geben Sie einen Namen in das Feld **Gruppenname** ein (Beispiel: Q1-15 Interessenten) und geben Sie ein Datum in das Datumsfeld ein, das dem Datum entspricht, an dem der Interessent am oder vor dem Kauf erworben wurde (Beispiel: 31.03.2015 für den letzten Tag des Q1-15). Klicken Sie auf **Hinzufügen**.

   ![](assets/sixteen.png)

   >[!NOTE]
   >
   >Sie können bis zu zehn Untergruppen hinzufügen, um die Datenwerte zu kategorisieren. Jeder Gruppenbereichseintrag baut auf dem vorherigen Eintrag auf. Wenn Sie den letzten Eintrag für den Gruppenbereich für die letzte von Ihnen erstellte benutzerspezifische Untergruppe leer lassen, wird kein Enddatumswert festgelegt.

   ![](assets/16.5.png)

   Und das ist es! Gute Arbeit.

Das folgende Beispiel zeigt einen Eintrag für Q1 2015-Interessenten bis zum 3. Quartal.