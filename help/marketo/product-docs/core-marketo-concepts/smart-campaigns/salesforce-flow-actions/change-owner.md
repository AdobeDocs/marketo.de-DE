---
unique-page-id: 1147021
description: Inhaber ändern - Marketing-Dokumente - Produktdokumentation
title: Inhaber ändern
translation-type: tm+mt
source-git-commit: f27e2bac90570f9f795dc6bdd5fcf208c446be14
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---


# Inhaber ändern {#change-owner}

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
   2. Wenn Sie versuchen, den Flussschritt **Ändern des Inhabers** für einen Kontakt zu verwenden, wird in Salesforce kein Duplikat erstellt.


   >[!NOTE]
   >
   >Wenn der Datensatz noch nicht in Ihrem Salesforce-Konto vorhanden ist, synchronisieren wir ihn und weisen ihn dann dem ausgewählten Benutzer zu.
