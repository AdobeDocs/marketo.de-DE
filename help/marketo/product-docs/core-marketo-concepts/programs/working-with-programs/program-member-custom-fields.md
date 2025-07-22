---
unique-page-id: 37355569
description: Benutzerdefinierte Felder für Programmteilnehmer - Marketo-Dokumente - Produktdokumentation
title: Benutzerdefinierte Felder für Programmteilnehmer
exl-id: 66b5dac6-015f-4907-8c82-78c932102463
feature: Programs
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 1%

---

# Benutzerdefinierte Felder für Programmteilnehmer {#program-member-custom-fields}

Benutzerdefinierte Felder für Programmteilnehmer ermöglichen es Ihnen, programmspezifische Daten für jedes Mitglied zu erfassen. Sie können in folgenden Bereichen verwendet werden: Marketo-Formulare, Filter und Trigger für Smart-Listen und Fluss-Aktionen für Smart-Kampagnen. Die Daten werden auf der Registerkarte Programmmitglieder angezeigt.

## Benutzerdefiniertes Feld für Programmteilnehmer erstellen {#create-a-program-member-custom-field}

1. Klicken Sie in Marketo auf **[!UICONTROL Admin]**.

   ![](assets/one.png)

1. Klicken Sie **[!UICONTROL Feldverwaltung]**.

   ![](assets/two.png)

1. Klicken Sie auf **[!UICONTROL Neues benutzerdefiniertes Feld]**.

   ![](assets/three.png)

1. Klicken Sie auf **[!UICONTROL Objekt]** und wählen Sie das gewünschte Objekt aus.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Benutzerdefinierte Felder [!UICONTROL Person] und [!UICONTROL Programmteilnehmer] können nicht denselben Namen haben.

1. Füllen Sie die restlichen Felder aus und klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Für [!UICONTROL Programmteilnehmer] benutzerdefinierte Felder werden folgende Typen unterstützt: Boolesch, Datum, Uhrzeit, Gleitkommazahl, Ganzzahl, Zeichenfolge, URL. [Weitere Informationen zu Feldtypen](/help/marketo/product-docs/administration/field-management/custom-field-type-glossary.md){target="_blank"}.

## Objektbeschreibungen {#object-descriptions}

| Objekt | Beschreibung |
|---|---|
| Unternehmen | Der Name der Firma, die mit der Person verknüpft ist. |
| Opportunity | Eine Opportunity kann mit einer Person oder einem Konto als potenzieller künftiger Verkauf verknüpft werden. Sie gelangen normalerweise über ein CRM oder eine API in Marketo. |
| Person | Eine Person in Ihrer Marketo-Datenbank, mit der Sie über Marketing-Kampagnen interagieren. |
| Programmmitglied | Person, die auch Mitglied eines Programms ist |

## Trigger und Filter {#triggers-and-filters}

Sie können diese programmspezifischen Daten in Smart Lists über [Trigger ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"} und/oder [Filter](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"} nutzen.

![](assets/six.png)

## Was man wissen muss {#things-to-know}

* Benutzerdefinierte Felder für Programmteilnehmer sind nur in lokalen Assets verfügbar. Sie werden in Design Studio nicht unterstützt, da es nicht möglich ist, sie mit einem bestimmten Programm zu verknüpfen.
* Sie können ein Formular (oder eine Landingpage mit einem Formular), das benutzerdefinierte Felder für Programmteilnehmer enthält, nicht klonen/in das Design Studio verschieben.
* [Sie können die benutzerdefinierten Felder ](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md){target="_blank"} Programmmitglieds mit den benutzerdefinierten Feldern für Kampagnenmitglieder synchronisieren.
* Das Objekt Programmteilnehmer kann bis zu 20 benutzerdefinierte Felder enthalten. Diese Felder stehen jedem Programm zur Verfügung.
* Wenn Sie ein Mitglied eines Programms entfernen und im benutzerdefinierten Feld Programmteilnehmer Daten vorhanden sind, werden die Daten aus diesem Feld bereinigt.
* Um die Daten anzuzeigen, klicken Sie im Programm auf die Registerkarte Mitglieder und erstellen Sie eine benutzerdefinierte Ansicht, die diese Felder enthält.
* Import und Export über [list](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md){target="_blank"} und [API](https://experienceleague.adobe.com/de/docs/marketo-developer/marketo/home){target="_blank"} werden unterstützt. Exportiert nur Arbeiten aus Programmteilnehmerlisten, keine statischen Listen.
* Wenn Sie zwei Personen zusammenführen, werden die benutzerdefinierten Felddaten des Programmmitglieds des Gewinners verwendet. Hat der Gewinner jedoch keinen, wird der Wert des Verlierers verwendet.
* Der Änderungstyp ist in den Informationsfeldern für Programmteilnehmer nicht zulässig.
* Die Smart-Listen-Einschränkung „enthält“ wird für benutzerdefinierte Felder von Programmmitgliedern nicht unterstützt.

>[!MORELIKETHIS]
>
>* [Erstellen eines benutzerdefinierten Felds in Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target="_blank"}
>
>* [Synchronisierung benutzerdefinierter Felder für Programmteilnehmer](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md){target="_blank"}
