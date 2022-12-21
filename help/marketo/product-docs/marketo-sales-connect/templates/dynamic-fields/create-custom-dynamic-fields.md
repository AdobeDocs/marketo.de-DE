---
unique-page-id: 14352508
description: Erstellen benutzerdefinierter dynamischer Felder - Marketo-Dokumente - Produktdokumentation
title: Benutzerdefinierte dynamische Felder erstellen
exl-id: 860511d2-4a8a-47a4-8362-ba4e715e44e9
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Benutzerdefinierte dynamische Felder erstellen {#create-custom-dynamic-fields}

Es gibt zwei Möglichkeiten, benutzerdefinierte dynamische Felder zu erstellen.

## Speichern benutzerdefinierter Felder für einen oder mehrere Kontakte {#saving-custom-fields-for-one-or-a-few-contacts}

1. Klicken Sie auf der Seite &quot;Personen&quot;auf den Namen eines Kontakts.

1. Wählen Sie das Dropdown-Menü neben Abonnement kündigen aus und wählen Sie **Bearbeiten**.

1. Scrollen Sie nach unten zum unteren Rand der Bearbeitungsseite. Anschließend können Sie einen Namen und einen Wert für Ihr Feld erstellen.

1. Klicken **Speichern**.

## Speichern benutzerdefinierter Felder für viele Kontakte {#saving-custom-fields-for-many-contacts}

1. Erstellen Sie eine CSV-Tabelle mit Ihren benutzerdefinierten Feldern in ihrer eigenen Spalte.

1. Befolgen Sie die [normaler CSV-Upload-Prozess](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md)auf dem Feld-Mapping-Bildschirm angehalten.

1. Wählen Sie anstelle eines der voreingestellten Felder die Option **Neues benutzerdefiniertes Feld hinzufügen** aus der Dropdown-Liste aus.

1. Geben Sie den gewünschten Feldnamen ein und klicken Sie auf **OK**.

1. Schließen Sie das Hochladen Ihrer CSV-Datei ab. Ihre Kontakte werden mit dem hinzugefügten benutzerdefinierten Feld ausgefüllt.

>[!NOTE]
>
>Nachdem Sie Ihr benutzerdefiniertes Feld erstellt haben, kann es etwa 30 Minuten dauern, bis das Feld in der Dropdown-Liste für dynamische Felder in Ihrem Vorlageneditor angezeigt wird.

## Verwenden benutzerdefinierter Felder in einer Vorlage {#how-to-use-your-custom-fields-in-a-template}

Sobald Ihre benutzerdefinierten Felder mit den oben genannten Methoden gespeichert wurden, können Sie sie in Ihren Vorlagen referenzieren.

1. [Erstellen einer Vorlage](/help/marketo/product-docs/marketo-sales-connect/templates/create-a-new-template.md) und klicken Sie auf **Dynamische Felder** -Schaltfläche, wie Sie es normalerweise tun würden.

1. Auswählen **Benutzerdefinierte Felder** aus der Dropdown-Liste, die angezeigt wird.

1. Sie sehen Ihre vorab gespeicherten benutzerdefinierten Felder und können eines auswählen, um die Vorlage auszufüllen.
