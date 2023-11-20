---
unique-page-id: 4719291
description: Standardnamen der Person und des Unternehmens festlegen - Marketo Docs - Produktdokumentation
title: Standardnamen der Person und des Unternehmens festlegen
exl-id: 0216fb41-adf0-4ccf-be22-c064e90be65a
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---

# Standardnamen der Person und des Unternehmens festlegen {#set-default-person-last-name-and-company-name}

Salesforce benötigt (mindestens) Nachname und Firmenname für Leads und Kontakte. Unvollständige Datensätze werden nicht mit Salesforce synchronisiert. Wenn Sie partielle Datensätze synchronisieren möchten, müssen Sie Standardwerte für die Verwendung von Marketo mit Salesforce festlegen.

1. Navigieren Sie zu **[!UICONTROL Admin]** und klicken **[!DNL Salesforce]**.

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. Klicks **[!UICONTROL Synchronisierungsoptionen bearbeiten]**.

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. Geben Sie einen **[!UICONTROL Standardname des Nachnamens der Person]** und **[!UICONTROL Standard-Personenunternehmen]** Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >Marketo Engage weist nur dann einen Standardwert zu, wenn der Datensatz erstmals mit Salesforce synchronisiert wird, und nur dann, wenn eines der erforderlichen Felder leer ist.

Und das ist das! Jedes Mal, wenn einer Person ein Nachname und/oder ein Firmenname fehlt, fügt Marketo den Standardwert hinzu, während der Datensatz synchronisiert wird.
