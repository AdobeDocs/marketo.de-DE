---
unique-page-id: 14352508
description: Erstellen benutzerdefinierter dynamischer Felder - Marketo-Dokumente - Produktdokumentation
title: Erstellen benutzerdefinierter dynamischer Felder
exl-id: 860511d2-4a8a-47a4-8362-ba4e715e44e9
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 4%

---

# Erstellen benutzerdefinierter dynamischer Felder {#create-custom-dynamic-fields}

Es gibt zwei Möglichkeiten, benutzerdefinierte dynamische Felder zu erstellen.

## Speichern benutzerdefinierter Felder für einen oder mehrere Kontakte {#saving-custom-fields-for-one-or-a-few-contacts}

1. Klicken Sie auf den Namen eines Kontakts auf der Seite [!UICONTROL Personen].

1. Wählen Sie die Dropdown-Liste neben [!UICONTROL Abmelden] und wählen Sie **[!UICONTROL Bearbeiten]**.

1. Scrollen Sie nach unten zum unteren Rand der Bearbeitungsseite. Anschließend können Sie einen Namen und einen Wert für Ihr Feld erstellen.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

## Speichern benutzerdefinierter Felder für viele Kontakte {#saving-custom-fields-for-many-contacts}

1. Erstellen Sie eine CSV-Tabelle mit Ihren benutzerdefinierten Feldern in einer eigenen Spalte.

1. Folgen Sie dem [normalen CSV-Upload](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) und stoppen Sie auf dem Bildschirm für die Feldzuordnung.

1. Wählen Sie aus der Dropdown-Liste **[!UICONTROL Neues benutzerdefiniertes Feld hinzufügen]** anstelle eines der Vorgabefelder aus.

1. Geben Sie den gewünschten Feldnamen ein und klicken Sie auf **[!UICONTROL OK]**.

1. CSV-Datei vollständig hochladen. Ihre Kontakte erhalten dann das hinzugefügte benutzerdefinierte Feld.

>[!NOTE]
>
>Nachdem Sie Ihr benutzerdefiniertes Feld erstellt haben, kann es etwa 30 Minuten dauern, bis das Feld in der Dropdown-Liste Dynamisches Feld im Vorlageneditor angezeigt wird.

## Verwenden von benutzerdefinierten Feldern in einer Vorlage {#how-to-use-your-custom-fields-in-a-template}

Nachdem Ihre benutzerdefinierten Felder mit den oben genannten Methoden gespeichert wurden, können Sie sie in Ihren Vorlagen referenzieren.

1. [Erstellen Sie eine Vorlage](/help/marketo/product-docs/marketo-sales-connect/templates/create-a-new-template.md) und klicken Sie auf die Schaltfläche **[!UICONTROL Dynamische Felder]** wie gewohnt.

1. Wählen Sie **[!UICONTROL Benutzerdefinierte Felder]** aus der angezeigten Dropdown-Liste aus.

1. Sie sehen Ihre vorab gespeicherten benutzerdefinierten Felder und können eines auswählen, um Ihre Vorlage auszufüllen.
