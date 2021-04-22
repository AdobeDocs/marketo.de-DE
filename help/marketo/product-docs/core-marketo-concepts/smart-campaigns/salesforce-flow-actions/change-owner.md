---
unique-page-id: 1147021
description: Eigentümer ändern - Marketo Docs - Produktdokumentation
title: Eigentümer ändern
exl-id: b22c5cd8-1b53-4802-8b49-7f607c8a601b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 3%

---

# Eigentümer ändern {#change-owner}

Wenn Sie bereits vorhandene Personen haben, die bereits einem Eigentümer zugewiesen sind, können Sie diese mit diesem Flussschritt einem anderen Eigentümer erneut zuweisen.

![](assets/image2014-9-22-15-3a1-3a3.png)

**Nutzung**

1. Wählen Sie einfach den Inhaber oder die Interessentenwarteschlange aus, zu der Sie wechseln möchten!

   ![](assets/image2014-9-22-15-3a1-3a6.png)

   >[!CAUTION]
   >
   >Salesforce lässt die Zuweisung von Kontakten zu Interessentenwarteschlangen nicht zu. Für einen Datensatz, der ein SFDC-Kontakt ist:
   >
   >1. Marketo erstellt einen Duplikat-Lead **nur**, wenn der Kontakt mit Salesforce synchronisiert wird. Anders ausgedrückt: Wenn Sie den Schritt **[Person mit SFDC synchronisieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)** mit `AssignTo=<a lead queue>` verwenden, erstellt Marketo einen Duplikat-Lead in Salesforce und weist ihn der Interessentenwarteschlange zu.
      >
      >
   1. Wenn Sie versuchen, den Flussschritt **Ändern des Inhabers** für einen Kontakt zu verwenden, wird in Salesforce kein Duplikat erstellt.


   >[!NOTE]
   >
   >Wenn der Datensatz noch nicht in Ihrem Salesforce-Konto vorhanden ist, synchronisieren wir ihn und weisen ihn dann dem ausgewählten Benutzer zu.
