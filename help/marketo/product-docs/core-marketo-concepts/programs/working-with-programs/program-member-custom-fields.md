---
unique-page-id: 37355569
description: Benutzerdefinierte Felder für Programm-Mitglieder - Marketing-Dokumente - Produktdokumentation
title: Benutzerdefinierte Felder für Programm-Member
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---


# Benutzerdefinierte Felder für Programm-Member {#program-member-custom-fields}

Benutzerdefinierte Programm-Member-Felder ermöglichen die Erfassung von Programm-spezifischen Daten für jedes Mitglied. Sie können verwendet werden bei: Marketo-Formulare, Filter und Auslöser für intelligente Liste und Flussaktionen für intelligente Kampagnen. Die Daten sind auf der Registerkarte &quot;Mitglieder&quot;des Programms sichtbar.

## Erstellen eines benutzerspezifischen Programm-Mitglieds {#create-a-program-member-custom-field}

1. Klicken Sie in Marketo auf **Admin**.

   ![](assets/one.png)

1. Klicken Sie auf **Feldverwaltung**.

   ![](assets/two.png)

1. Klicken Sie auf **Neues benutzerdefiniertes Feld**.

   ![](assets/three.png)

1. Klicken Sie auf die Dropdown-Liste &quot;Objekt&quot;und wählen Sie das gewünschte Objekt aus.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Benutzerdefinierte Felder für Programm und Person können nicht denselben Namen haben.

1. Füllen Sie die übrigen Felder aus und klicken Sie auf **Erstellen**.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Unterstützte Typen für benutzerdefinierte Programm-Member-Felder: boolean, date, datetime, float, integer, string, URL. [Weitere Informationen zu Feldtypen](http://docs.marketo.com/x/Wwgt).

## Objektbeschreibungen {#object-descriptions}

| Objekt | Beschreibung |
|---|---|
| Firma | Der Name der Firma, die der Person zugeordnet ist. |
| Chancen | Eine Möglichkeit kann mit einer Person oder einem Konto als potenzieller künftiger Verkauf verbunden werden. Normalerweise gelangen sie über ein CRM oder über eine API nach Marketo. |
| Person | Eine Person in Ihrer Marketo-Datenbank, mit der Sie über Marketing-Kampagnen in Kontakt treten. |
| Programm | Person, die auch Mitglied eines Programms ist |

## Auslöser und Filter {#triggers-and-filters}

Sie können diese Programm-spezifischen Daten in intelligenten Listen über [Auslöser](http://docs.marketo.com/x/PoAR)und/oder [Filter](http://docs.marketo.com/x/2YAI) nutzen.

![](assets/six.png)

## Was Sie wissen sollten {#things-to-know}

* Benutzerdefinierte Programm-Member-Felder stehen nur in lokalen Assets zur Verfügung. Sie werden in Design Studio nicht unterstützt, da es nicht möglich ist, sie mit einem bestimmten Programm zu verknüpfen.
* Sie können ein Formular (oder eine Landingpage mit einem Formular), das benutzerdefinierte Programm-Member-Felder enthält, nicht in Design Studio klonen/verschieben.
* Benutzerdefinierte Programm-Member-Felder können nicht als Token verwendet werden.
* Das Programm Member-Objekt kann bis zu 20 benutzerdefinierte Felder enthalten. Diese Felder stehen jedem Programm zur Verfügung.
* Wenn Sie ein Mitglied eines Programms entfernen und das benutzerdefinierte Feld &quot;Programm-Mitglied&quot;Daten enthält, werden die Daten aus diesem Feld gescrubbt.
* Um die Daten Ansicht, klicken Sie im Programm auf die Registerkarte &quot;Mitglieder&quot;und erstellen Sie eine benutzerdefinierte Ansicht, die diese Felder enthält.
* Import und Export über [Liste](http://docs.marketo.com/x/egAk)und [API](http://developers.marketo.com/)werden unterstützt.
* Wenn Sie zwei Personen zusammenführen, werden die Felddaten des Gewinners für ein benutzerdefiniertes Programm verwendet. Hat der Gewinner jedoch keine, wird der Wert des Verlierers verwendet.

>[!MORELIKETHIS]
>
>[Benutzerdefiniertes Feld in Marketing erstellen](../../../../product-docs/administration/field-management/create-a-custom-field-in-marketo.md)

