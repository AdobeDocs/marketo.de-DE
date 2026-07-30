---
description: Erfahren Sie, wie Sie die Funktion Smart Campaign on Archive deaktivieren aktivieren, sodass Kampagnen automatisch deaktiviert werden, wenn ein Ordner oder ein Programm in Marketo archiviert wird.
title: Deaktivieren von Smart-Kampagnen im Archiv
feature: Administration
hide: true
source-git-commit: 526d10bb96e059d251a76ca720ff81ab42ee9516
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# Deaktivieren von Smart-Kampagnen im Archiv {#disable-smart-campaigns-on-archive}

Wenn diese Funktion aktiviert ist, werden die Kampagnen eines Ordners oder Programms automatisch deaktiviert, um unerwartete Aktivitäten zu verhindern.

Wenn ein Ordner oder ein Programm archiviert wird oder eine aktive Smart-Kampagne in einen bereits archivierten Ordner verschoben wird, verhindert Marketo Engage die Ausführung der betroffenen Kampagnen:

* **Ausgelöste Kampagnen** sind deaktiviert.
* **Batch-Kampagnen** deren ausstehende Ausführungen abgebrochen wurden.
* **Ausführbare Kampagnen** haben keinen Ausführungsstatus, sodass keine Aktion durchgeführt wird.

## Aktivieren von {#how-to-enable}

1. Klicken Sie im **Admin**-Bereich auf **Schatztruhe**.

   ![Das Admin-Navigationsmenü mit hervorgehobener Schatztruhe](assets/disable-smart-campaigns-on-archive-1.png)

1. Scrollen Sie zu _Smart-Kampagnen im_ deaktivieren) und klicken Sie auf **Bearbeiten**.

   ![Treasure Chest settings-Seite, auf der die Schaltfläche „Smart-Kampagnen deaktivieren“ in der Zeile „Archiv“ mit der Schaltfläche „Bearbeiten“ angezeigt wird](assets/disable-smart-campaigns-on-archive-2.png)

1. Aktivieren Sie das **Aktiviert** und klicken Sie auf **Speichern**.

   ![Das Dialogfeld Smart-Kampagnen im Archiv deaktivieren mit dem Kontrollkästchen Aktiviert und der Schaltfläche Speichern](assets/disable-smart-campaigns-on-archive-3.png)

<table>
  <tr>
    <td><b>Aktiviert (markiert)</b></td>
    <td>Die Archivierung deaktiviert jede Kampagne gemäß den oben genannten Regeln.</td>
  </tr>
  <tr>
    <td><b>Deaktiviert (deaktiviert)</b></td>
    <td>Die Archivierung eines Ordners oder Programms funktioniert weiterhin, aber Kampagnen werden unverändert ausgeführt oder geplant.</td>
  </tr>
</table>

>[!IMPORTANT]
>
>Nachdem Sie diese Einstellung umgeschaltet haben, müssen Sie Ihren Browser aktualisieren, damit die Änderung wirksam wird.

## Unterstützte Aktionen

Die folgenden Aktionen deaktivieren Kampagnen, wenn _Smart-Kampagnen im Archiv deaktivieren_ aktiviert ist:

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
