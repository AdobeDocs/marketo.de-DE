---
unique-page-id: 1147027
description: Person mit SFDC synchronisieren - Marketo-Dokumente - Produktdokumentation
title: Synchronisieren von Personen mit SFDC
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
feature: Smart Campaigns, Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '125'
ht-degree: 6%

---

# Synchronisieren von Personen mit SFDC {#sync-person-to-sfdc}

In diesem Flussschritt werden von Marketo erstellte Personen als Leads in Ihr Salesforce CRM eingefügt.

>[!NOTE]
>
>Nur verfügbar, wenn mit [!DNL Salesforce] integriert.

1. Standardmäßig werden diese Flussschritte den Lead-Inhabern auf der Grundlage der Salesforce-Regeln für die automatische Zuweisung zugewiesen.

   ![](assets/sync-person-to-sfdc-1.png)

   >[!TIP]
   >
   >[!DNL Salesforce] muss die Person die Felder Firma und Nachname ausgefüllt haben. Andernfalls wird der Lead-Datensatz abgelehnt.

1. Sie können einen bestimmten [!DNL Salesforce] oder eine bestimmte Lead-Warteschlange als Lead-Inhaber festlegen.

   ![](assets/sync-person-to-sfdc-2.png)

   Bei Verwendung dieses Flussschritts wird die Person sofort als [!DNL Salesforce] Lead synchronisiert und muss nicht auf die reguläre Synchronisierung warten.

   >[!CAUTION]
   >
   >[!DNL Salesforce] erlaubt es nicht, „Kontakte“ Lead-Warteschlangen zuzuweisen. In diesem Fall erstellt Marketo in [!DNL Salesforce] ein doppeltes „Lead“.
