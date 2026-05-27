---
unique-page-id: 1147027
description: Erfahren Sie, wie Sie eine Person mit einem Flussschritt mit Salesforce synchronisieren. Lead- oder Kontaktdaten an SFDC senden, wenn sie in den Fluss eintreten.
title: Synchronisieren von Personen mit SFDC
exl-id: 4284ec35-6ac5-4084-beb7-976eb6fd7e3c
feature: Smart Campaigns, Salesforce Integration
TQID: https://experienceleague.adobe.com/jU7Hg1x8TUfxR4GnO1oxvJXh-8X3LVXll9z8k5Eck80
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 143
ht-degree: 5%

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
