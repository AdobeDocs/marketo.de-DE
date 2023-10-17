---
unique-page-id: 1147027
description: Person mit SFDC synchronisieren - Marketo Docs - Produktdokumentation
title: Person mit SFDC synchronisieren
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 4bae0126d6b36720e170bea7b6b973508c855633
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 6%

---

# Person mit SFDC synchronisieren {#sync-person-to-sfdc}

In diesem Flussschritt werden von Marketo erstellte Personen als Leads in Ihr Salesforce-CRM eingefügt.

![](assets/sync-person-to-sfdc.png)

>[!NOTE]
>
>Nur verfügbar bei Integration mit Salesforce.

1. Standardmäßig wird dieser Flussschritt den Lead-Eigentümern basierend auf den Salesforce-Regeln für die automatische Zuweisung zugewiesen.

   ![](assets/sync-person-to-sfdc.png)

   >[!TIP]
   >
   >Für Salesforce müssen die Felder Firma und Nachname ausgefüllt sein. Andernfalls wird der Lead-Datensatz zurückgewiesen.

1. Sie können einen bestimmten Salesforce-Benutzer oder eine Lead-Warteschlange als Lead-Inhaber festlegen.

   ![](assets/sync-person-to-sfdc-2.png)

   Bei Verwendung dieses Flussschritts wird die Person sofort als Salesforce-Lead synchronisiert und muss nicht auf die regelmäßige Synchronisierung warten.

   >[!CAUTION]
   >
   >Salesforce lässt die Zuweisung von &quot;Kontakten&quot;zu Lead-Warteschlangen nicht zu. In diesem Fall erstellt Marketo ein Duplikat &quot;Lead&quot;in Salesforce.
