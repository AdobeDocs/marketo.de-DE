---
unique-page-id: 1147021
description: Inhaber ändern - Marketo-Dokumente - Produktdokumentation
title: Eigentümer ändern
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 2%

---

# Eigentümer ändern {#change-owner}

Wenn Sie über vorhandene Personen verfügen, die bereits einem Eigentümer zugewiesen sind, können Sie diesen Flussschritt verwenden, um sie einem anderen Eigentümer neu zuzuweisen.

![](assets/change-owner-1.png)

1. Wählen Sie einfach den Besitzer oder die Lead-Warteschlange, zu der Sie wechseln möchten, und gehen Sie!

   ![](assets/change-owner-2.png)

   >[!CAUTION]
   >
   >Salesforce erlaubt nicht, Kontakten Lead-Warteschlangen zuzuweisen. Für einen Datensatz, der ein SFDC-Kontakt ist:
   >
   >* Marketo erstellt ein doppeltes Lead **nur** wenn der Kontakt mit Salesforce synchronisiert wird. Anders ausgedrückt: Wenn Sie den Flussschritt **[Person mit SFDC synchronisieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** mit `AssignTo=<a lead queue>` verwenden, erstellt Marketo ein doppeltes Lead in Salesforce und weist es der Lead-Warteschlange zu.
   >
   >* Wenn Sie den **[!UICONTROL Inhaber ändern]** Flussschritt für einen Kontakt verwenden, erstellt Marketo ein doppeltes Lead in Salesforce. Um dies zu vermeiden, verwenden Sie einen Filter für das Feld &quot;SFDC-Typ“, der die Aktion auf Leads beschränkt.

   >[!NOTE]
   >
   >Wenn der Datensatz noch nicht in Ihrem Salesforce-Konto vorhanden ist, synchronisieren wir ihn und weisen ihn dann dem ausgewählten Benutzer zu.
