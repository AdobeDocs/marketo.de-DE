---
unique-page-id: 4719291
description: Standardnamen der Firma und des Benutzers festlegen - Marketing Docs - Produktdokumentation
title: Standardnamen der Person und Firma festlegen
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 0%

---


# Standardnamen der Person und Firma festlegen{#set-default-person-last-name-and-company-name}

Salesforce benötigt (mindestens) Nachname und Firma für seine Interessenten und Kontakte. Unvollständige Datensätze werden nicht mit Salesforce synchronisiert. Wenn Sie partielle Datensätze synchronisieren möchten, müssen Sie Standardwerte festlegen, die Marketo mit Salesforce verwenden soll.

1. Gehen Sie zu **Admin** und klicken Sie auf **Salesforce**.

   ![](assets/image2014-12-9-13-3a41-3a58.png)

1. Klicken Sie auf **Synchronisierungsoptionen bearbeiten**.

   ![](assets/image2014-12-9-13-3a42-3a6.png)

1. Geben Sie einen **Familiennamen der Standardperson** und eine **Standardperson-Firma** ein und klicken Sie dann auf **Speichern**.

   ![](assets/sync-options-hands.png)

   >[!NOTE]
   >
   >Marketo weist nur dann einen Standardwert zu, wenn der Datensatz zunächst mit Salesforce synchronisiert wird, und nur dann, wenn eines der erforderlichen Felder leer ist.

Und das ist das! Jedes Mal, wenn einem Benutzer ein Nachname und/oder ein Firma fehlt, fügt Marketo den Standardwert hinzu, während der Datensatz synchronisiert wird.
