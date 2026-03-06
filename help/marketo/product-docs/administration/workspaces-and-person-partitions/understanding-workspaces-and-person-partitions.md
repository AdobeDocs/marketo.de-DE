---
unique-page-id: 2360309
description: Erfahren Sie, wie Arbeitsbereiche Marketing-Assets organisieren und wie Personenpartitionen als separate Datenbanken fungieren.
title: Grundlegendes zu Arbeitsbereichen und Personen-Partitionen
exl-id: 27d00a0d-ebf1-4dff-b41e-1644ec9dbd28
feature: Partitions, Workspaces
source-git-commit: e894ece3a643113fd3e1d8df9f8addefea5553f5
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 97%

---

# Grundlegendes zu Arbeitsbereichen und Personen-Partitionen {#understanding-workspaces-and-person-partitions}

## Arbeitsbereiche {#workspaces}

>[!CAUTION]
>
>Die Einrichtung von Arbeitsbereichen kann komplex sein. Wenden Sie sich an den [Marketo-Support](https://nation.marketo.com/t5/support/ct-p/Support?profile.language=de), um herauszufinden, ob Arbeitsbereiche für Sie geeignet sind.

Arbeitsbereiche sind separate Bereiche in Marketo, die Marketing-Assets wie Programme, Landingpages, E-Mails und mehr enthalten. Sie können von mehreren Personen verwendet werden. Alle Benutzenden haben Zugriff auf einen oder mehrere Arbeitsbereiche.

>[!NOTE]
>
>**Beispiel**
>
>Einige Gründe für die Verwendung eines Arbeitsbereichs:
>
>* Geografie: Marketing-Abteilungen in Europa, Asien und Nordamerika erhalten jeweils einen Arbeitsbereich
>* Geschäftseinheit: [!DNL Quicken], [!DNL Quickbooks] und [!DNL TurboTax] erhalten jeweils einen Arbeitsbereich
>
>Eine Trennung ist in jedem Fall notwendig, wenn die Marketing-Assets völlig unterschiedlich sind. Wenn sie jedoch dieselben Marketing-Assets nutzen, sind Arbeitsbereiche möglicherweise nicht das richtige Tool für Sie.

>[!NOTE]
>
>Erfahren Sie, wie Sie [einen neuen Arbeitsbereich erstellen](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-new-workspace.md).

## Freigeben über Arbeitsbereiche hinweg {#sharing-across-workspaces}

Im Folgenden erfahren Sie, wie Sie Assets über Arbeitsbereiche hinweg freigeben. Die Freigabe funktioniert für alle Assets gleich. Dieses Beispiel behandelt Segmentierungen.

>[!NOTE]
>
>Der übergeordnete Ordner mit den Assets ist der einzige Ordner, der freigegeben werden kann. Die untergeordneten Ordner können nicht freigegeben werden.

1. Klicken Sie auf **[!UICONTROL Datenbank]**.

   ![](assets/understanding-workspaces-and-person-partitions-1.png)

1. Klicken Sie mit der rechten Maustaste auf den Ordner „Segmentierung“ und klicken Sie dann auf **[!UICONTROL Neuer Ordner]**.

   ![](assets/understanding-workspaces-and-person-partitions-2.png)

1. Benennen Sie den Ordner und klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/understanding-workspaces-and-person-partitions-3.png)

1. Verschieben Sie die freizugebenden Assets in den Ordner.

   ![](assets/understanding-workspaces-and-person-partitions-4.png)

1. Klicken Sie mit der rechten Maustaste auf den Ordner und wählen Sie **[!UICONTROL Ordner freigeben]** aus.

   ![](assets/understanding-workspaces-and-person-partitions-5.png)

1. Wählen Sie die Arbeitsbereiche aus, für die Sie den Ordner freigeben möchten, und klicken Sie auf **[!UICONTROL Speichern]**. Im Dialogfeld „Ordner freigeben“ werden nur Arbeitsbereiche angezeigt, für die Sie über Anzeigeberechtigungen verfügen.

   ![](assets/understanding-workspaces-and-person-partitions-6.png)

   >[!NOTE]
   >
   >Am Ursprungsordner wird nun ein kleiner grüner Pfeil angezeigt, der darauf hinweist, dass der Ordner freigegeben wurde. Am im Arbeitsbereich freigegebenen Ordner wird ein Vorhängeschloss angezeigt, das darauf hinweist, dass der Ordner schreibgeschützt ist.

Sie können diese Elemente über Arbeitsbereiche hinweg freigeben.

* E-Mail-Vorlagen
* Landingpage-Vorlagen
* Modelle
* Intelligente Kampagnen
* [Intelligente Listen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [Segmentierungen](/help/marketo/product-docs/administration/workspaces-and-person-partitions/share-segmentations-across-workspaces-and-partitions.md)
* Ausschnitte

## Klonen über Arbeitsbereiche hinweg {#cloning-across-workspaces}

Assets, die keine Vorlagen sind, sollten am besten als lokale Assets in einem Programm geklont werden. Über die richtige Zugriffsebene können Sie diese Assets per Drag-and-Drop in einen anderen Arbeitsbereich ziehen:

* Programme
* E-Mails
* Landingpages
* Formulare

>[!IMPORTANT]
>
>Alle oben aufgeführten Elemente können über Arbeitsbereiche hinweg geklont werden. E-Mails, Formulare und Landingpages müssen sich zum Zeitpunkt des Klonens jedoch _in einem Programm befinden_.

>[!NOTE]
>
>Beim Klonen von Assets mit Vorlagen müssen diese Vorlagen für den Zielarbeitsbereich freigegeben sein.

## Verschieben von Assets in andere Arbeitsbereiche {#moving-assets-to-other-workspaces}

Um Assets in einen neuen Arbeitsbereich zu verschieben, legen Sie sie in einem Ordner ab und ziehen Sie den Ordner in den anderen Arbeitsbereich.

>[!NOTE]
>
>Sie können ein Programm mit Mitgliedern nicht von einem Arbeitsbereich in einen anderen verschieben.

## Personen-Partitionen {#person-partitions}

Personen-Partitionen funktionieren wie separate Datenbanken. Jede Partition enthält ihre eigenen Personen, die nicht dedupliziert oder mit anderen Partitionen vermischt werden. Wenn Sie der Meinung sind, dass ein geschäftlicher Anwendungsfall vorliegt, bei dem doppelte Einträge mit derselben E-Mail-Adresse erforderlich sein können, wenden Sie sich an den [Marketo-Support](https://nation.marketo.com/t5/support/ct-p/Support?profile.language=de).

Sie können Personen-Partitionen [Arbeitsbereichen](create-a-new-workspace.md) in den folgenden Konfigurationen zuweisen:

* ein Arbeitsbereich für eine Personen-Partition (1:1)
* ein Arbeitsbereich für viele Personen-Partitionen (1:x)
* viele Arbeitsbereiche für eine Personen-Partition (x:1)

>[!NOTE]
>
>Gründe für die Verwendung einer Personen-Partition:
>
>* Ihre Arbeitsbereiche verfügen über verschiedene Assets und enthalten auch keine gleichen Personen
>* Duplikate werden aus anderen geschäftlichen Gründen gewünscht

>[!CAUTION]
>
>Personen-Partitionen interagieren nicht miteinander, daher sollten Sie bei ihrer Einrichtung sorgfältig vorgehen.

>[!NOTE]
>
>Erfahren Sie, wie Sie [eine Personen-Partition erstellen](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md).
