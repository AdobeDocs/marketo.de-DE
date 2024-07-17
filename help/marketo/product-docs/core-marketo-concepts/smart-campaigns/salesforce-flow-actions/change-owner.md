---
unique-page-id: 1147021
description: Inhaber ändern - Marketo Docs - Produktdokumentation
title: Eigentümer ändern
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 934bb5f197f801e48cf8e7554335eb2d07289037
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 2%

---

# Eigentümer ändern {#change-owner}

Wenn Sie bereits vorhandene Personen haben, die bereits einem Eigentümer zugewiesen sind, können Sie diesen Flussschritt verwenden, um sie einem anderen Eigentümer erneut zuzuweisen.

![](assets/change-owner-1.png)

1. Wählen Sie einfach den Eigentümer oder die Lead-Warteschlange aus, in die Sie wechseln möchten.

   ![](assets/change-owner-2.png)

   >[!CAUTION]
   >
   >Salesforce lässt die Zuweisung von Kontakten zu Lead-Warteschlangen nicht zu. Für einen Datensatz, der ein SFDC-Kontakt ist:
   >
   >* Marketo erstellt einen doppelten Lead **nur** , wenn der Kontakt mit Salesforce synchronisiert wird. Wenn Sie also den Flussschritt **[Person mit SFDC synchronisieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** mit `AssignTo=<a lead queue>` verwenden, erstellt Marketo einen doppelten Lead in Salesforce und weist ihn der Lead-Warteschlange zu.
   >
   >* Wenn Sie den Flussschritt **[!UICONTROL Inhaber wechseln]** für einen Kontakt verwenden, erstellt Marketo einen doppelten Lead in Salesforce. Um dies zu vermeiden, verwenden Sie einen Filter für das Feld &quot;SFDC-Typ&quot;, der die Aktion auf Leads beschränkt.

   >[!NOTE]
   >
   >Wenn der Datensatz noch nicht in Ihrem Salesforce-Konto vorhanden ist, synchronisieren wir ihn und weisen ihn dann dem ausgewählten Benutzer zu.
