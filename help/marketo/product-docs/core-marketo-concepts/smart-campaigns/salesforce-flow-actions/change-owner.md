---
unique-page-id: 1147021
description: Inhaber ändern - Marketo Docs - Produktdokumentation
title: Eigentümer ändern
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
feature: Smart Campaigns, Salesforce Integration
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 2%

---

# Eigentümer ändern {#change-owner}

Wenn Sie bereits vorhandene Personen haben, die bereits einem Eigentümer zugewiesen sind, können Sie diesen Flussschritt verwenden, um sie einem anderen Eigentümer erneut zuzuweisen.

![](assets/image2014-9-22-15-3a1-3a3.png)

**Nutzung**

1. Wählen Sie einfach den Eigentümer oder die Lead-Warteschlange aus, in die Sie wechseln möchten.

   ![](assets/image2014-9-22-15-3a1-3a6.png)

   >[!CAUTION]
   >
   >Salesforce lässt die Zuweisung von Kontakten zu Lead-Warteschlangen nicht zu. Für einen Datensatz, der ein SFDC-Kontakt ist:
   >
   >1. Marketo erstellt ein doppeltes Lead **only** wenn der Kontakt mit Salesforce synchronisiert wird. Mit anderen Worten, wenn Sie die **[Person mit SFDC synchronisieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** Flussschritt mit `AssignTo=<a lead queue>`, erstellt Marketo einen doppelten Lead in Salesforce und weist ihn der Lead-Warteschlange zu.
   >
   >1. Wenn Sie **Inhaber ändern** Flussschritt bei einem Kontakt erstellt Marketo in Salesforce ein doppeltes Lead. Um dies zu vermeiden, verwenden Sie einen Filter für das Feld &quot;SFDC-Typ&quot;, der die Aktion auf Leads beschränkt.

   >[!NOTE]
   >
   >Wenn der Datensatz noch nicht in Ihrem Salesforce-Konto vorhanden ist, synchronisieren wir ihn und weisen ihn dann dem ausgewählten Benutzer zu.
