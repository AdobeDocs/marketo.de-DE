---
unique-page-id: 37355569
description: Benutzerdefinierte Felder für Programmmitglieder - Marketo-Dokumente - Produktdokumentation
title: Benutzerdefinierte Felder für Programmmitglieder
exl-id: 66b5dac6-015f-4907-8c82-78c932102463
source-git-commit: 56f429dabf19c4425c68b0dcd745621681a038ae
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 1%

---

# Benutzerdefinierte Felder für Programmmitglieder {#program-member-custom-fields}

Benutzerdefinierte Felder für Programmmitglieder ermöglichen die Erfassung programmspezifischer Daten für jedes Mitglied. Sie können in folgenden Bereichen verwendet werden: Marketo-Formulare, Smart-List-Filter und -Trigger sowie Fluss-Aktionen für intelligente Kampagnen. Die Daten können im Tab Mitglieder des Programms eingesehen werden.

>[!NOTE]
>
>Benutzerdefinierte Felder des Programmmitglieds verfügen derzeit nicht über eine Integration mit Feldern des Salesforce-Campaign-Mitglieds.

## Benutzerdefiniertes Feld für Programmteilnehmer erstellen {#create-a-program-member-custom-field}

1. Klicken Sie in Marketo auf **Admin**.

   ![](assets/one.png)

1. Klicken **Feldverwaltung**.

   ![](assets/two.png)

1. Klicken **Neues benutzerdefiniertes Feld**.

   ![](assets/three.png)

1. Klicken Sie auf die Dropdown-Liste Objekt und wählen Sie das gewünschte Objekt aus.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Benutzerdefinierte Felder für Personen und Programmmitglieder können nicht denselben Namen verwenden.

1. Füllen Sie die übrigen Felder aus und klicken Sie auf **Erstellen**.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Unterstützte Typen für benutzerdefinierte Felder des Programmmitglieds sind: boolean, date, datetime, float, integer, string, URL. [Erfahren Sie mehr über Feldtypen](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md){target=&quot;_blank&quot;}.

## Objektbeschreibungen {#object-descriptions}

| Objekt | Beschreibung |
|---|---|
| Unternehmen | Der Name des mit der Person verknüpften Unternehmens. |
| Chance | Eine Möglichkeit kann mit einer Person oder einem Konto als potenzieller künftiger Verkauf verbunden werden. Normalerweise gelangen sie über ein CRM-System oder eine API in Marketo. |
| Person | Eine Person in Ihrer Marketo-Datenbank, mit der Sie über Marketingkampagnen interagieren. |
| Programmmitglied | Person, die auch Mitglied eines Programms ist |

## Trigger und Filter {#triggers-and-filters}

Sie können diese programmspezifischen Daten in Smart-Listen über [Trigger](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target=&quot;_blank&quot;} und/oder [Filter](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target=&quot;_blank&quot;}.

![](assets/six.png)

## Was zu wissen ist {#things-to-know}

* Benutzerdefinierte Felder für Programmmitglieder sind nur in lokalen Assets verfügbar. Sie werden in Design Studio nicht unterstützt, da es keine Möglichkeit gibt, sie mit einem bestimmten Programm zu verknüpfen.
* Sie können ein Formular (oder eine Landingpage mit einem Formular), das benutzerdefinierte Felder für Programmmitglieder enthält, nicht in Design Studio klonen/verschieben.
* Das Programmteilobjekt kann über bis zu 20 benutzerdefinierte Felder verfügen. Diese Felder stehen jedem Programm zur Verfügung.
* Wenn Sie ein Mitglied eines Programms entfernen und im benutzerdefinierten Feld Programmteilnehmer Daten enthalten, werden die Daten aus diesem Feld gescrollt.
* Um die Daten anzuzeigen, klicken Sie im Programm auf den Tab Mitglieder und erstellen Sie eine benutzerdefinierte Ansicht, die diese Felder enthält.
* Import und Export über [Liste](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md){target=&quot;_blank&quot;} und [API](https://developers.marketo.com/){target=&quot;_blank&quot;} werden unterstützt. Exporte funktionieren nur auf Programmteilslisten, nicht auf statischen Listen.
* Wenn Sie zwei Personen zusammenführen, werden die benutzerdefinierten Felddaten des Gewinners für das Programmmitglied verwendet. Wenn der Gewinner jedoch keinen hat, wird der Wert des Verlierers verwendet.
* Der Änderungstyp ist in den Feldern &quot;Programmteilnehmer-Info&quot;nicht zulässig.
* Die Beschränkung &quot;enthält&quot;der intelligenten Liste wird für benutzerdefinierte Felder des Programmmitglieds nicht unterstützt.

>[!MORELIKETHIS]
>
>[Benutzerdefiniertes Feld in Marketo erstellen](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target=&quot;_blank&quot;}
