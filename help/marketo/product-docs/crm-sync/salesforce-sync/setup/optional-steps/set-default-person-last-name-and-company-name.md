---
unique-page-id: 4719291
description: Festlegen des Nachnamens der Person und des Firmennamens - Marketo-Dokumente - Produktdokumentation
title: Standardnamen für Nachnamen und Firmennamen von Personen festlegen
exl-id: 0216fb41-adf0-4ccf-be22-c064e90be65a
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---

# Standardnamen für Nachnamen und Firmennamen von Personen festlegen {#set-default-person-last-name-and-company-name}

[!DNL Salesforce] erfordert (mindestens) Nachnamen und Firmennamen für die Leads und Kontakte. Unvollständige Datensätze werden nicht mit [!DNL Salesforce] synchronisiert. Wenn Sie partielle Datensätze synchronisieren möchten, müssen Sie Standardwerte für die Verwendung von Marketo mit [!DNL Salesforce] festlegen.

1. Gehen Sie zu **[!UICONTROL Admin]** und klicken Sie auf **[!DNL Salesforce]**.

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. Klicken Sie **[!UICONTROL Synchronisierungsoptionen bearbeiten]**.

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. Geben Sie einen **[!UICONTROL Nachnamen der Standardperson]** und eine **[!UICONTROL Standardfirma der Person]** ein und klicken Sie dann auf **[!UICONTROL Speichern]**.

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >Marketo Engage weist nur dann einen Standardwert zu, wenn der Datensatz anfänglich mit Salesforce synchronisiert wird, und nur dann, wenn eines der erforderlichen Felder leer ist.

Und das war&#39;s! Jedes Mal, wenn einer Person ein Nachname und/oder ein Firmenname fehlt, fügt Marketo den Standardwert hinzu, wenn der Datensatz synchronisiert wird.
