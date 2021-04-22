---
unique-page-id: 1147027
description: Person mit dem SFDC synchronisieren - Marketo Docs - Produktdokumentation
title: Person mit SFDC synchronisieren
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 7%

---

# Person mit SFDC synchronisieren {#sync-person-to-sfdc}

>[!NOTE]
>
>Nur verfügbar, wenn in Salesforce integriert.

## Übersicht {#overview}

Dieser Flussschritt fügt Marketo-erstellte Personen als Interessenten in Ihr Salesforce CRM ein.

![](assets/sync-person-to-sfdc.png)

## Nutzung {#usage}

1. Standardmäßig weist dieser Flussschritt Interessenteninhabern basierend auf den Salesforce-Regeln für die automatische Zuweisung zu.

   ![](assets/sync-person-to-sfdc.png)

   >[!TIP]
   >
   >Für Salesforce müssen die Felder &quot;Firma&quot;und &quot;Nachname&quot;ausgefüllt sein. Andernfalls wird der Interessentendatensatz abgelehnt.

1. Sie können einen bestimmten Salesforce-Benutzer oder eine Interessentenwarteschlange als Interessentenbesitzer festlegen.

   ![](assets/sync-person-to-sfdc-2.png)

   Bei Verwendung dieses Flussschritts wird die Person sofort als Salesforce-Lead synchronisiert und muss nicht auf die regelmäßige Synchronisierung warten.

   >[!CAUTION]
   >
   >Salesforce lässt die Zuweisung von &quot;Kontakten&quot;zu Interessentenwarteschlangen nicht zu. In diesem Fall wird Marketo ein Duplikat &quot;Lead&quot;in Salesforce erstellen.
