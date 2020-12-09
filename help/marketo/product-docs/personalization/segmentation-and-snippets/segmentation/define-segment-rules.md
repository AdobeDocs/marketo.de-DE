---
unique-page-id: 2359449
description: Segmentregeln definieren - Marketing-Dokumente - Produktdokumentation
title: Segmentregeln definieren
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '444'
ht-degree: 0%

---


# Segmentregeln definieren {#define-segment-rules}

Durch die Definition von Segmentregeln können Sie Ihre Personen in verschiedene Gruppen kategorisieren, die sich gegenseitig ausschließen.

>[!NOTE]
>
>**FYI**
>
>Marketo standardisiert nun die Sprache für alle Abonnements, sodass Sie möglicherweise Interessenten in Ihrem Abonnement und Personen/Personen in docs.marketo.com sehen können. Diese Begriffe bedeuten dasselbe. Es hat keine Auswirkungen auf die Artikelanweisungen. Es gibt auch noch einige andere Änderungen. [Weitere Informationen](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

>[!PREREQUISITES]
>
>[Eine Segmentierung erstellen](create-a-segmentation.md)

1. Wechseln Sie zur **Datenbank.**

   ![](assets/image2017-3-28-14-3a7-3a42.png)

1. Klicken Sie in der Struktur auf **Segmentierung **und dann auf ein bestimmtes **Segment**.

   ![](assets/image2017-3-28-14-3a11-3a15.png)

1. Klicken Sie auf **Intelligente Liste** und fügen Sie Filter hinzu.

   ![](assets/image2017-3-28-14-3a18-3a19.png)

   >[!CAUTION]
   >
   >Segmente unterstützen derzeit keine Operatoren *in Vergangenheit* und *In Zeitrahmen *auf Filtern. Das liegt daran, dass Segmentationen nur dann nach Updates suchen, wenn ein Wert für Änderungsdaten protokolliert wird. Diese Werte werden *nicht* für Dinge protokolliert, die sich automatisch ändern, z. B. Formelfelder und Datumsangaben. Darüber hinaus werden Datumsoperatoren mit relativen Datumsbereichen nicht unterstützt, da sie zum Zeitpunkt der Segmentierungsgenehmigung und nicht zum Zeitpunkt der Aktivität &quot;Datenwert ändern&quot;berechnet werden.

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
   >Intelligente Listen sind großartig. Erfahren Sie alles, was Sie mit [intelligenten Listen und statischen Listen](http://docs.marketo.com/display/docs/smart+lists+and+static+lists)tun können.

1. Klicken Sie auf die Registerkarte &quot; **Personen (Entwurf)** &quot;, um die Personen Ansicht, die sich als Mitglied dieses Segments qualifizieren können.

   ![](assets/image2017-3-28-14-3a20-3a15.png)

1. Gehen Sie zu **Segmentierungsaktionen**. Klicken Sie auf **Genehmigen**.

   ![](assets/image2014-9-15-11-3a36-3a7.png)

   >[!CAUTION]
   >
   >Die Gesamtanzahl der Segmente, die Sie in einer Segmentierung erstellen können, hängt von der Anzahl und dem Typ der verwendeten Filter sowie davon ab, wie komplex die Segmentlogik ist. Sie können zwar bis zu 100 Segmente mithilfe von Standardfeldern erstellen, andere Filter können jedoch die Komplexität erhöhen und Ihre Segmentierung kann möglicherweise nicht genehmigt werden. Beispiele: benutzerdefinierte Felder, Liste, Interessenteninhaberfelder und Umsatzstufen.
   >
   >
   >Wenn Sie während der Genehmigung eine Fehlermeldung erhalten und Hilfe bei der Reduzierung der Komplexität Ihrer Segmentierung benötigen, wenden Sie sich bitte an den [MarketingTo Support](http://nation.marketo.com/t5/Support/ct-p/Support).

1. Sehen Sie sich das Dashboard an, um einen schnellen Überblick über Ihre Segmente in einem Kreisdiagramm sowie die angewendeten Regeln zu erhalten.

   ![](assets/image2014-9-15-11-3a36-3a19.png)

Gute Arbeit! Diese Segmente werden an vielen Orten in Marketo praktisch sein.

>[!NOTE]
>
>Eine Person kann sich für verschiedene Segmente qualifizieren, gehört aber letztendlich zu nur einem Segment, das von der [Prioritätsreihenfolge der Segmente](segmentation-order-priority.md)abhängt.

>[!NOTE]
>
>**Erinnerung**
>
>Der Bildschirm &quot;Personen (Entwurf)&quot;zeigt alle Personen an, die sich als Mitglied qualifizieren und nicht immer die endgültige Liste von Personen ist. Genehmigen Sie Ihr Segment, um die endgültige Liste anzuzeigen.

>[!NOTE]
>
>**Verwandte Artikel**
>
>* [Genehmigen einer Segmentierung](approve-a-segmentation.md)

>



