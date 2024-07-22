---
unique-page-id: 2360309
description: Grundlegendes zu Arbeitsbereichen und Personen-Partitionen - Marketo-Dokumente - Produktdokumentation
title: Grundlagen zu Arbeitsbereichen und Personen-Partitionen
exl-id: 27d00a0d-ebf1-4dff-b41e-1644ec9dbd28
feature: Partitions, Workspaces
source-git-commit: 91b6460bf0fa7fed85d48887ec38203f2ee7440f
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 3%

---

# Grundlagen zu Arbeitsbereichen und Personen-Partitionen {#understanding-workspaces-and-person-partitions}

## Arbeitsbereiche {#workspaces}

>[!CAUTION]
>
>Die Einrichtung von Arbeitsbereichen kann kompliziert sein. Wenden Sie sich an den [Marketo-Support](https://nation.marketo.com/t5/Support/ct-p/Support) , um herauszufinden, ob sie für Sie geeignet sind.

Arbeitsbereiche sind separate Bereiche in Marketo, die Marketing-Assets wie Programme, Landingpages, E-Mails und mehr enthalten. Sie können von mehreren Personen verwendet werden. Jeder Benutzer hat Zugriff auf einen oder mehrere Arbeitsbereiche.

>[!NOTE]
>
>**Beispiel**
>
>Einige Gründe für die Verwendung eines Arbeitsbereichs:
>
>* Geografie: Marketing-Abteilungen in Europa, Asien und Nordamerika erhalten jeweils einen Arbeitsbereich
>* Geschäftseinheit: [!DNL Quicken], [!DNL Quickbooks] und [!DNL TurboTax] erhalten jeweils einen Arbeitsbereich
>
>In jedem Fall liegt die Trennung darin, dass sich die Marketing-Assets vollständig unterscheiden. Wenn sie Marketing-Assets gemeinsam nutzen, sind Arbeitsbereiche möglicherweise nicht das richtige Tool für Sie.

>[!NOTE]
>
>Erfahren Sie, wie Sie [einen neuen Arbeitsbereich erstellen](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-new-workspace.md).

## Freigeben über Arbeitsbereiche hinweg {#sharing-across-workspaces}

So können Sie Assets über Arbeitsbereiche hinweg freigeben. Es funktioniert für alles, was Sie freigeben möchten. Dieses Beispiel zeigt Segmentierungen.

>[!NOTE]
>
>Der übergeordnete Ordner, der Ihre Assets enthält, ist der einzige Ordner, der freigegeben werden kann, nicht die untergeordneten Ordner.

1. Klicken Sie auf **[!UICONTROL Database]**.

   ![](assets/understanding-workspaces-and-person-partitions-1.png)

1. Klicken Sie mit der rechten Maustaste auf den Ordner Segmentierung und klicken Sie auf **[!UICONTROL Neuer Ordner]**.

   ![](assets/understanding-workspaces-and-person-partitions-2.png)

1. Benennen Sie den Ordner und klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/understanding-workspaces-and-person-partitions-3.png)

1. Verschieben Sie die Assets, die Sie freigeben möchten, in den Ordner .

   ![](assets/understanding-workspaces-and-person-partitions-4.png)

1. Klicken Sie mit der rechten Maustaste auf den Ordner und wählen Sie **[!UICONTROL Ordner freigeben]** aus.

   ![](assets/understanding-workspaces-and-person-partitions-5.png)

1. Wählen Sie die Arbeitsbereiche aus, für die Sie den Ordner freigeben möchten, und klicken Sie auf **[!UICONTROL Speichern]**. Im Dialogfeld Ordner freigeben werden nur Arbeitsbereiche angezeigt, für die Sie über die entsprechenden Berechtigungen verfügen.

   ![](assets/understanding-workspaces-and-person-partitions-6.png)

   >[!NOTE]
   >
   >Der Ursprungsordner hat jetzt einen kleinen grünen Pfeil, der angibt, dass er freigegeben wurde. Im freigegebenen Arbeitsbereich verfügt der Ordner über ein Vorhängeschloss, das schreibgeschützt ist.

Sie können diese Elemente über Arbeitsbereiche hinweg freigeben.

* E-Mail-Vorlagen
* Landing Page-Vorlagen
* Modelle
* Smart-Kampagnen
* [Smart-Listen](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/reference-a-list-or-smart-list-across-workspaces.md)
* [Segmentierungen](/help/marketo/product-docs/administration/workspaces-and-person-partitions/share-segmentations-across-workspaces-and-partitions.md)
* Ausschnitte

## Klonen über Arbeitsbereiche hinweg {#cloning-across-workspaces}

Bei Assets, die keine Vorlagen sind, empfiehlt es sich, sie als lokale Assets innerhalb eines Programms zu klonen. Mit der richtigen Zugriffsebene können Sie diese Assets in einen anderen Arbeitsbereich ziehen:

* Programme
* E-Mails
* Landing Pages
* Formulare

>[!IMPORTANT]
>
>Während alle oben aufgeführten Elemente über Arbeitsbereiche hinweg geklont werden können, müssen sich E-Mails, Formulare und Landingpages _zum Zeitpunkt des Klonens in einem Programm_ befinden.

>[!NOTE]
>
>Beim Klonen von Assets mit Vorlagen müssen diese Vorlagen für den Ziel-Workspace freigegeben werden.

## Verschieben von Assets in andere Arbeitsbereiche {#moving-assets-to-other-workspaces}

Um Assets in einen neuen Arbeitsbereich zu verschieben, legen Sie sie in einen Ordner ab und ziehen Sie den Ordner in den anderen Arbeitsbereich.

>[!NOTE]
>
>Sie können ein Programm, das Mitglieder enthält, nicht von einem Arbeitsbereich in einen anderen verschieben.

## Personen-Partitionen {#person-partitions}

Personenpartitionen verhalten sich wie separate Datenbanken. Jede Partition hat eigene Personen, die nicht deduplizieren oder mit anderen Partitionen mischen. Wenden Sie sich an den [Marketo-Support](https://nation.marketo.com/t5/Support/ct-p/Support), wenn Sie denken, dass ein geschäftlicher Anwendungsfall möglicherweise doppelte Datensätze mit derselben E-Mail-Adresse erfordert.

Sie können [Arbeitsbereiche](create-a-new-workspace.md) Benutzerpartitionen in den folgenden Konfigurationen zuweisen:

* eine Partition zwischen Arbeitsbereich und Person (1:1)
* Partitionen von einer Arbeitsfläche zu mehreren Personen (1:x)
* viele Arbeitsbereiche zu einer Personenpartition (x:1)

>[!NOTE]
>
>Gründe für die Verwendung einer Personenpartition:
>
>* Ihre Arbeitsbereiche verfügen nicht nur über verschiedene Assets, sondern teilen auch keine Personen.
>* Sie möchten aus anderen geschäftlichen Gründen Duplikate erstellen

>[!CAUTION]
>
>Personen-Partitionen interagieren nicht miteinander, also seien Sie vorsichtig bei der Einrichtung.

>[!NOTE]
>
>Erfahren Sie, wie Sie [eine Personenpartition erstellen](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md).
