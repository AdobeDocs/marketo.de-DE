---
unique-page-id: 2360423
description: Alle Leads in einem Umsatzzyklusmodell suchen - Marketo-Dokumente - Produktdokumentation
title: Alle Leads in einem Umsatzzyklusmodell suchen
exl-id: 428dbfa1-2f19-41ce-bfc6-e63edfdaba17
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 0%

---

# Alle Leads in einem Umsatzzyklusmodell suchen {#find-all-leads-in-a-revenue-cycle-model}

Durch die Verwendung von Smart Lists können Sie alle Mitglieder des Umsatzzyklusmodells leicht finden.

>[!PREREQUISITES]
>
>[Erstellen einer Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)

1. Klicken Sie bei ausgewählter Smart-Liste auf die Registerkarte **Smart-Liste**.

   ![](assets/image2015-4-29-14-3a6-3a36.png)

1. Suchen Sie den **Mitglied des Umsatzmodells** und ziehen Sie ihn auf die Arbeitsfläche.

   ![](assets/image2015-4-29-14-3a12-3a33.png)

1. Wählen Sie ein **Modell** aus.

   ![](assets/image2015-5-13-18-3a2-3a23.png)

   Dadurch bekämen Sie alle Leads in diesem Modell, unabhängig von der Phase. Normalerweise ist ein bestimmter Schritt erforderlich. Verwenden Sie stattdessen den folgenden Filter.

1. Suchen Sie den Filter **Umsatzstufe** und ziehen Sie ihn auf die Arbeitsfläche.

   ![](assets/image2015-5-13-17-3a27-3a0.png)

1. Wählen Sie ein **Stadium**.

   ![](assets/image2015-5-13-17-3a31-3a9.png)

1. Gehen Sie zur Registerkarte **Leads**, um die Ergebnisse anzuzeigen.

   ![](assets/2.png)

   >[!TIP]
   >
   >Sie benötigen nicht beide Filter, wählen Sie einfach den gewünschten Filter aus. Wir zeigen Ihnen nur, dass Sie beide gründlich sind.

   >[!CAUTION]
   >
   >Wenn der Schritt eines Leads durch eine externe Kampagne während der ersten Erstellung des Leads geändert wird, wird eine Aktivität nicht in der Datenbank protokolliert. Das bedeutet, dass der Lead nicht in den Filter der Smart-Liste aufgenommen wird.
