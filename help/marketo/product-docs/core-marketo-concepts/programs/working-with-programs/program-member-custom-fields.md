---
unique-page-id: 37355569
description: Benutzerdefinierte Felder für Programmmitglieder - Marketo-Dokumente - Produktdokumentation
title: Benutzerdefinierte Felder für Programmmitglieder
exl-id: 66b5dac6-015f-4907-8c82-78c932102463
feature: Programs
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 1%

---

# Benutzerdefinierte Felder für Programmmitglieder {#program-member-custom-fields}

Benutzerdefinierte Felder für Programmmitglieder ermöglichen die Erfassung programmspezifischer Daten für jedes Mitglied. Sie können in folgenden Aktionen verwendet werden: Marketo-Formulare, Smart-List-Filter und -Trigger sowie Flussaktionen für Smart-Campaign. Die Daten können im Tab Mitglieder des Programms eingesehen werden.

## Benutzerdefiniertes Feld für Programmteilnehmer erstellen {#create-a-program-member-custom-field}

1. Klicken Sie in Marketo auf **[!UICONTROL Admin]**.

   ![](assets/one.png)

1. Klicken Sie auf **[!UICONTROL Feldverwaltung]**.

   ![](assets/two.png)

1. Klicken Sie auf **[!UICONTROL Neues benutzerdefiniertes Feld]**.

   ![](assets/three.png)

1. Klicken Sie auf die Dropdownliste Objekt und wählen Sie das gewünschte Objekt aus.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Benutzerdefinierte Felder für Personen und Programmmitglieder können nicht denselben Namen verwenden.

1. Füllen Sie die restlichen Felder aus und klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Unterstützte Typen für benutzerdefinierte Felder des Programmmitglieds sind: boolesch, Datum, Datum, Uhrzeit, Gleitkommazahl, Ganzzahl, Zeichenfolge, URL. [Erfahren Sie mehr über Feldtypen](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md){target="_blank"}.

## Objektbeschreibungen {#object-descriptions}

| Objekt | Beschreibung |
|---|---|
| Unternehmen | Der Name des mit der Person verknüpften Unternehmens. |
| Opportunity | Eine Möglichkeit kann mit einer Person oder einem Konto als potenzieller künftiger Verkauf verbunden werden. Normalerweise gelangen sie über ein CRM-System oder eine API in Marketo. |
| Person | Eine Person in Ihrer Marketo-Datenbank, mit der Sie über Marketingkampagnen interagieren. |
| Programmmitglied | Person, die auch Mitglied eines Programms ist |

## Trigger und Filter {#triggers-and-filters}

Sie können diese programmspezifischen Daten in Smart-Listen über [Trigger](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"} und/oder [Filter](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"} nutzen.

![](assets/six.png)

## Was zu wissen ist {#things-to-know}

* Benutzerdefinierte Felder für Programmmitglieder sind nur in lokalen Assets verfügbar. Sie werden in Design Studio nicht unterstützt, da es keine Möglichkeit gibt, sie mit einem bestimmten Programm zu verknüpfen.
* Sie können ein Formular (oder eine Landingpage mit einem Formular), das benutzerdefinierte Felder für Programmmitglieder enthält, nicht in Design Studio klonen/verschieben.
* [Sie können die benutzerdefinierten Felder des Programmmitglieds mit den benutzerdefinierten Feldern des Kampagnenmitglieds synchronisieren.](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md){target="_blank"}
* Das Programmteilobjekt kann über bis zu 20 benutzerdefinierte Felder verfügen. Diese Felder stehen jedem Programm zur Verfügung.
* Wenn Sie ein Mitglied eines Programms entfernen und im benutzerdefinierten Feld Programmteilnehmer Daten enthalten, werden die Daten aus diesem Feld gescrollt.
* Um die Daten anzuzeigen, klicken Sie im Programm auf den Tab Mitglieder und erstellen Sie eine benutzerdefinierte Ansicht, die diese Felder enthält.
* Der Import und Export über [list](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md){target="_blank"} und [API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/home){target="_blank"} wird unterstützt. Exporte funktionieren nur auf Programmteilslisten, nicht auf statischen Listen.
* Wenn Sie zwei Personen zusammenführen, werden die benutzerdefinierten Felddaten des Gewinners für das Programmmitglied verwendet. Aber wenn der Gewinner keinen hat, wird der Wert des Verlierers verwendet.
* Der Änderungstyp ist in den Feldern &quot;Programmteilnehmer-Info&quot;nicht zulässig.
* Die Beschränkung &quot;enthält&quot;der intelligenten Liste wird für benutzerdefinierte Felder des Programmmitglieds nicht unterstützt.

>[!MORELIKETHIS]
>
>* [Benutzerdefiniertes Feld in Marketo erstellen](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target="_blank"}
>
>* [Benutzerdefinierte Feldsynchronisierung für Programmteilnehmer](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md){target="_blank"}
