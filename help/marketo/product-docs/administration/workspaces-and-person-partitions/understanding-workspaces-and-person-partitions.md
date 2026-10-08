---
unique-page-id: 2360309
description: Erfahren Sie, wie Arbeitsbereiche Marketing-Assets organisieren und wie Personenpartitionen als separate Datenbanken fungieren.
title: Grundlegendes zu Arbeitsbereichen und Personen-Partitionen
exl-id: 27d00a0d-ebf1-4dff-b41e-1644ec9dbd28
feature: Partitions, Workspaces
TQID: 'https://experienceleague.adobe.com/Ex-WBSNYTFvevcwryuO4CzUsg79nOmjkVx4WMUx9nqA'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
    internal-label: Smart Campaigns
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
    internal-label: Forms
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
    internal-label: Programs
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
    internal-label: Templates
  - id: b4e49ca2-9149-5443-90e6-11978bb87c2f
    internal-label: Partitions
  - id: fffc2f21-ba05-5d98-924c-16da987a5b69
    internal-label: Workspaces
subfeature_v2:
  - id: d0251300-e25f-466f-9856-7e11ce8fa7aa
    internal-label: Smart lists
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 76%
---
# Grundlegendes zu Arbeitsbereichen und Personen-Partitionen&#x200B; {#understanding-workspaces-and-person-partitions}

## Arbeitsbereiche {#workspaces}

>[!CAUTION]
>
>Die Einrichtung von Arbeitsbereichen kann komplex sein. Wenden Sie sich an den [Marketo](https://nation.marketo.com/t5/support/ct-p/Support?profile.language=de)Support, um herauszufinden, ob er für Sie geeignet ist.

Arbeitsbereiche sind separate Bereiche in Marketo, die Marketing-Assets wie Programme, Landingpages, E-Mails und mehr enthalten. Sie können von mehreren Personen verwendet werden. Jede Benutzerin und jeder Benutzer hat Zugriff auf einen oder mehrere Arbeitsbereiche.

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
>Erfahren Sie, wie [einen neuen Arbeitsbereich erstellen](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-new-workspace.md).

## Freigeben über Arbeitsbereiche hinweg {#sharing-across-workspaces}

In den folgenden Schritten wird erläutert, wie Assets in Arbeitsbereichen freigegeben werden. Die Freigabe funktioniert für alle Assets gleich. Dieses Beispiel behandelt Segmentierungen.

>[!NOTE]
>
>Der übergeordnete Ordner mit den Assets ist der einzige Ordner, der freigegeben werden kann. Die untergeordneten Ordner/Elemente können nicht freigegeben werden.

1. Klicken Sie auf **[!UICONTROL Datenbank]**.

   ![](assets/understanding-workspaces-and-person-partitions-1.png)

1. Klicken Sie mit der rechten Maustaste auf den Ordner „Segmentierung“ und klicken Sie dann auf **[!UICONTROL Neuer Ordner]**.

   ![](assets/understanding-workspaces-and-person-partitions-2.png)

1. Benennen Sie den Ordner und klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/understanding-workspaces-and-person-partitions-3.png)

1. Verschieben Sie die freizugebenden Asset(s) in den Ordner.

   ![](assets/understanding-workspaces-and-person-partitions-4.png)

1. Klicken Sie mit der rechten Maustaste auf den Ordner und wählen Sie **[!UICONTROL Ordner freigeben]** aus.

   ![](assets/understanding-workspaces-and-person-partitions-5.png)

1. Wählen Sie die Arbeitsbereiche aus, für die Sie den Ordner freigeben möchten, und klicken Sie auf **[!UICONTROL Speichern]**. Im Dialogfeld „Ordner freigeben“ werden nur Arbeitsbereiche angezeigt, für die Sie eine Berechtigung zur Anzeige haben.

   ![](assets/understanding-workspaces-and-person-partitions-6.png)

   >[!NOTE]
   >
   >Der Ausgangsordner weist jetzt einen kleinen grünen Pfeil auf, der anzeigt, dass er freigegeben wurde. Am im Arbeitsbereich freigegebenen Ordner wird ein Vorhängeschloss angezeigt, das darauf hinweist, dass der Ordner schreibgeschützt ist.

Sie können diese Elemente über Arbeitsbereiche hinweg freigeben.

* E-Mail-Vorlagen
* Landingpage-Vorlagen
* Modelle
* Intelligente Kampagnen
* [Intelligente Listen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [Segmentierungen](/help/marketo/product-docs/administration/workspaces-and-person-partitions/share-segmentations-across-workspaces-and-partitions.md)
* Ausschnitte

## Klonen über Arbeitsbereiche hinweg {#cloning-across-workspaces}

Für Assets, die keine Vorlagen sind, wird empfohlen, sie als lokale Assets innerhalb eines Programms zu klonen. Über die richtige Zugriffsebene können Sie diese Assets per Drag-and-Drop in einen anderen Arbeitsbereich ziehen:

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
>Ein Programm, das Mitglieder enthält, kann nicht von einem Arbeitsbereich in einen anderen verschoben werden.

## Personen-Partitionen {#person-partitions}

Personen-Partitionen funktionieren wie separate Datenbanken. Jede Partition enthält ihre eigenen Personen, die nicht dedupliziert oder mit anderen Partitionen vermischt werden. Wenn für Ihren geschäftlichen Anwendungsfall doppelte Einträge mit derselben E-Mail-Adresse erforderlich sind, wenden Sie sich an den [Marketo-Support](https://nation.marketo.com/t5/support/ct-p/Support?profile.language=de).

Sie können Personen-Partitionen [Arbeitsbereichen](create-a-new-workspace.md) in den folgenden Konfigurationen zuweisen:

* 1:1-Partition (1:1)
* ein Arbeitsbereich für viele Personen-Partitionen (1:x)
* Viele Arbeitsbereiche zu einer Personenpartition (x:1)

>[!NOTE]
>
>Gründe für die Verwendung einer Personen-Partition:
>
>* Ihre Arbeitsbereiche verfügen nicht nur über verschiedene Assets, sondern geben auch keine Personen frei
>* Duplikate werden aus anderen geschäftlichen Gründen gewünscht

>[!CAUTION]
>
>Personen-Partitionen interagieren nicht miteinander, daher sollten Sie bei der Einrichtung sorgfältig vorgehen.

>[!NOTE]
>
>Erfahren Sie, wie Sie [eine Personen-Partition erstellen](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md).
