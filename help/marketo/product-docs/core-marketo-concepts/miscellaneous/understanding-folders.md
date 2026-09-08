---
unique-page-id: 4720779
description: Erfahren Sie mehr über Ordner in Programmen zum Organisieren von Smart-Kampagnen und Assets. Erstellen, Umbenennen und Löschen von Ordnern
title: Grundlegendes zu Ordnern
exl-id: 2ea914f6-ca64-4e87-806c-93beba075ab2
TQID: https://experienceleague.adobe.com/wAE129LK3Pk-CB5SSQqqSV50ng085soYsm4JHfh0CuI
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d65b4a73-87a3-4d56-b638-74e74d9939ce
  - id: f82558ea-6af5-44eb-a424-5b3389abb0a3
source-git-commit: 7c035bd266b25d19ab7406ca989e8fc9f13126b9
workflow-type: tm+mt
source-wordcount: 428
ht-degree: 1%

---

# Grundlegendes zu Ordnern {#understanding-folders}

Ordner in einem Programm können zum Organisieren von Smart-Kampagnen und Assets verwendet werden. Diese unterscheiden sich von [Kampagnenordnern](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/create-new-campaign-folder.md).

## Erstellen eines Ordners {#create-a-folder}

1. Navigieren Sie zum Bereich **[!UICONTROL Marketing-Aktivitäten]**.

   ![](assets/ma.png)

1. Klicken Sie mit der rechten Maustaste auf ein Programm und wählen Sie **[!UICONTROL Neuer Ordner]**.

   ![](assets/image2015-4-20-18-3a45-3a14.png)

1. Benennen Sie den neuen Ordner und drücken Sie die **[!UICONTROL Eingabetaste]**.

   ![](assets/image2015-4-20-18-3a46-3a57.png)

Der neue Ordner ist jetzt für Ihre lokalen Assets bereit.

## Umbenennen eines Ordners {#rename-a-folder}

1. Klicken Sie mit der rechten Maustaste auf den Ordner und wählen Sie **[!UICONTROL Ordner umbenennen]**.

   ![](assets/image2015-4-20-18-3a49-3a10.png)

1. Geben Sie einen neuen Namen ein und drücken Sie die **[!UICONTROL Eingabetaste]**.

   ![](assets/image2015-4-20-18-3a52-3a30.png)

## Löschen eines Ordners {#delete-a-folder}

>[!NOTE]
>
>Stellen Sie sicher, dass der Ordner leer ist, bevor Sie ihn löschen.

1. Klicken Sie mit der rechten Maustaste auf den Ordner und wählen Sie **[!UICONTROL Ordner löschen]**.

   ![](assets/image2015-4-20-18-3a55-3a51.png)

## Ordner archivieren {#archive-a-folder}

In Marketo haben Sie die Möglichkeit, vorhandene Ordner in Archivordner zu konvertieren. Archivordner sind in [!UICONTROL Marketing-Aktivitäten], [!UICONTROL Datenbank] und [!UICONTROL Design Studio] vorhanden.

![](assets/image2015-4-20-19-3a3-3a46.png)

Beim Archivieren eines Ordners:

* Der Ordner und die Assets sind nicht mehr in den Suchergebnissen sichtbar. Wenn Sie in einem archivierten Ordner nach einem Programm oder Ereignis suchen, geben die Ergebnisse eine reduzierte Ansicht des archivierten Ordners zurück
* Die Assets im Ordner werden nicht mehr in automatisch vorgeschlagen angezeigt
* Archivierte Vorlagen sind beim Erstellen einer E-Mail oder Landingpage in Design Studio nicht verfügbar
* Archivierte Seiten können nicht in Testgruppen für Landingpages verwendet werden

Funktionalität, die sich bei **Archivierung** ändert:

* Die globale Suche findet weiterhin Ergebnisse in archivierten Ordnern
* Sie können einen Filter verwenden, um archivierte Assets zur Verwendung in Berichten auszuwählen

### Smart Campaign bei Archivierung deaktiviert {#disable-smart-campaigns-archive}

Wenn ein Ordner oder ein Programm archiviert wird oder eine aktive Smart-Kampagne in einen bereits archivierten Ordner verschoben wird, verhindert Marketo Engage die Ausführung der betroffenen Kampagnen:

* **Ausgelöste Kampagnen** sind deaktiviert.
* **Batch-Kampagnen** deren ausstehende Ausführungen abgebrochen wurden.
* **Ausführbare Kampagnen** haben keinen Ausführungsstatus, sodass keine Aktion durchgeführt wird.

**Unterstützte Aktionen**

Die folgenden Aktionen deaktivieren Kampagnen:

* Ziehen eines Ordners **Ordner** mit aktiven Kampagnen in einen archivierten Ordner
* Ziehen eines (**)** Typs mit aktiven Kampagnen per Drag-and-Drop in einen archivierten Ordner
* Ziehen einer (einzelnen **intelligenten Kampagne** in einen archivierten Ordner
* Rechtsklick auf **Verschieben** auf einer einzelnen Smart-Kampagne in einen archivierten Ordner
* Rechtsklick auf **Ordner verschieben** auf einen Ordner mit aktiven Kampagnen in einen archivierten Ordner
* Rechtsklick auf **Verschieben** eines Programms mit aktiven Kampagnen in einen archivierten Ordner
* Rechtsklick auf **Ordner** In archivierten Ordner konvertieren), um ihn an einem Ort zu archivieren, ohne ihn zu verschieben

>[!NOTE]
>
>Wenn eine Smart-Kampagne im archivierten Ordner oder Programm an einer anderen Stelle referenziert wird (z. B. über den Flussschritt „Kampagne anfragen„), wird die Archivierung blockiert, um zu verhindern, dass die andere Kampagne beschädigt wird.
