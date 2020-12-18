---
unique-page-id: 14352508
description: Benutzerdefinierte dynamische Felder erstellen - Marketing-Dokumente - Produktdokumentation
title: Benutzerdefinierte dynamische Felder erstellen
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---


# Benutzerdefinierte dynamische Felder erstellen {#create-custom-dynamic-fields}

Es gibt zwei Möglichkeiten, benutzerdefinierte dynamische Felder zu erstellen.

## Speichern benutzerdefinierter Felder für einen oder mehrere Kontakte {#saving-custom-fields-for-one-or-a-few-contacts}

1. Klicken Sie auf der Seite &quot;Personen&quot;auf den Namen eines Kontakts.
1. Wählen Sie die Dropdownliste neben Abmelden und wählen Sie **Bearbeiten**.
1. Blättern Sie nach unten zur Bearbeitungsseite. Anschließend können Sie einen Namen und einen Wert für Ihr Feld erstellen.
1. Klicken Sie auf **Speichern**.

## Speichern benutzerdefinierter Felder für viele Kontakte {#saving-custom-fields-for-many-contacts}

1. Erstellen Sie eine CSV-Tabelle mit Ihren benutzerdefinierten Feldern in ihrer eigenen Spalte.
1. Folgen Sie dem Vorgang [Normaler CSV-Upload](http://docs.marketo.com/x/HIPS) und beenden Sie ihn im Bildschirm &quot;Feldzuordnung&quot;.
1. Wählen Sie anstelle eines der vorgegebenen Felder **Hinzufügen ein neues benutzerdefiniertes Feld** aus der Dropdownliste.
1. Geben Sie den gewünschten Feldnamen ein und klicken Sie auf **OK**.
1. Schließen Sie das Hochladen der CSV-Datei ab. Ihre Kontakte werden mit dem hinzugefügten benutzerdefinierten Feld ausgefüllt.

>[!NOTE]
>
>Nachdem Sie Ihr benutzerdefiniertes Feld erstellt haben, kann es etwa 30 Minuten dauern, bis das Feld in der Dropdown-Liste &quot;Dynamisches Feld&quot;im Vorlageneditor angezeigt wird.

## So verwenden Sie Ihre benutzerdefinierten Felder in einer Vorlage {#how-to-use-your-custom-fields-in-a-template}

Sobald Ihre benutzerdefinierten Felder mit den oben genannten Methoden gespeichert wurden, können Sie sie in Ihren Vorlagen referenzieren.

1. [Erstellen Sie eine ](http://docs.marketo.com/x/OCDG) Vorlage und klicken Sie wie gewohnt auf die Schaltfläche  **Dynamische** Felder.
1. Wählen Sie **Benutzerdefinierte Felder** aus der Dropdown-Liste, die angezeigt wird.
1. Sie sehen Ihre vorab gespeicherten benutzerdefinierten Felder und können ein Feld auswählen, das Sie in Ihrer Vorlage ausfüllen möchten.

