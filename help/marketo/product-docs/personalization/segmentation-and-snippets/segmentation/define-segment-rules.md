---
unique-page-id: 2359449
description: Segmentregeln definieren - Marketing-Dokumente - Produktdokumentation
title: Segmentregeln definieren
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---


# Segmentregeln definieren {#define-segment-rules}

Durch die Definition von Segmentregeln können Sie Ihre Personen in verschiedene Gruppen kategorisieren, die sich gegenseitig ausschließen.

>[!PREREQUISITES]
>
>[Eine Segmentierung erstellen](create-a-segmentation.md)

1. Gehen Sie zur **Datenbank.**

   ![](assets/image2017-3-28-14-3a7-3a42.png)

1. Klicken Sie auf **Segmentierung **aus der Struktur und dann auf ein bestimmtes **Segment**.

   ![](assets/image2017-3-28-14-3a11-3a15.png)

1. Klicken Sie auf **Intelligente Liste** und fügen Sie Filter hinzu.

   ![](assets/image2017-3-28-14-3a18-3a19.png)

   >[!CAUTION]
   >
   >Segmente unterstützen derzeit nicht die Operatoren *In der Vergangenheit* und *In Zeitrahmen *auf Filtern. Das liegt daran, dass Segmentationen nur dann nach Updates suchen, wenn ein Wert für Änderungsdaten protokolliert wird. Diese Werte werden für Elemente, die sich automatisch ändern, wie z. B. Formelfelder und Datumsangaben, nicht *protokolliert.* Darüber hinaus werden Datumsoperatoren mit relativen Datumsbereichen nicht unterstützt, da sie zum Zeitpunkt der Segmentierungsgenehmigung und nicht zum Zeitpunkt der Aktivität &quot;Datenwert ändern&quot;berechnet werden.

   >[!NOTE]
   >
   >Die Filter &quot;SFDC-Typ&quot;und &quot;Microsoft-Typ&quot;werden derzeit in intelligenten Segmentierungslösungen nicht unterstützt.

1. Füllen Sie die entsprechenden Werte für die Filter aus.

   ![](assets/image2017-3-28-14-3a18-3a33.png)

   >[!NOTE]
   >
   >**Tieftauchen**
   >
   >
   >Intelligente Listen sind großartig. Erfahren Sie alles, was Sie mit [Smart-Listen und statischen Listen](https://docs.marketo.com/display/docs/smart+lists+and+static+lists) tun können.

1. Klicken Sie auf die Registerkarte **Personen (Entwurf)**, um die Personen Ansicht, die sich als Mitglied dieses Segments qualifizieren können.

   ![](assets/image2017-3-28-14-3a20-3a15.png)

1. Gehen Sie zu **Segmentierungsaktionen**. Klicken Sie auf **Genehmigen**.

   ![](assets/image2014-9-15-11-3a36-3a7.png)

   >[!CAUTION]
   >
   >Die Gesamtanzahl der Segmente, die Sie in einer Segmentierung erstellen können, hängt von der Anzahl und dem Typ der verwendeten Filter sowie davon ab, wie komplex die Segmentlogik ist. Sie können zwar bis zu 100 Segmente mithilfe von Standardfeldern erstellen, andere Filter können jedoch die Komplexität erhöhen und Ihre Segmentierung kann möglicherweise nicht genehmigt werden. Beispiele: benutzerdefinierte Felder, Liste, Interessenteninhaberfelder und Umsatzstufen.
   >
   >
   >Wenn Sie während der Genehmigung eine Fehlermeldung erhalten und Hilfe bei der Reduzierung der Komplexität Ihrer Segmentierung benötigen, wenden Sie sich bitte an [Marketing Support](https://nation.marketo.com/t5/Support/ct-p/Support).

1. Sehen Sie sich das Dashboard an, um einen schnellen Überblick über Ihre Segmente in einem Kreisdiagramm sowie die angewendeten Regeln zu erhalten.

   ![](assets/image2014-9-15-11-3a36-3a19.png)

Gute Arbeit! Diese Segmente werden an vielen Orten in Marketo praktisch sein.

>[!NOTE]
>
>Eine Person kann sich für verschiedene Segmente qualifizieren, gehört aber letztendlich zu nur einem Segment, das von der Reihenfolge [Priorität der Segmente](segmentation-order-priority.md) abhängt.

>[!NOTE]
>
>**Erinnerung**
>
>Der Bildschirm &quot;Personen (Entwurf)&quot;zeigt alle Personen an, die sich als Mitglied qualifizieren und nicht immer die endgültige Liste von Personen ist. Genehmigen Sie Ihr Segment, um die endgültige Liste anzuzeigen.

>[!MORELIKETHIS]
>
>* [Genehmigen einer Segmentierung](approve-a-segmentation.md)

>



