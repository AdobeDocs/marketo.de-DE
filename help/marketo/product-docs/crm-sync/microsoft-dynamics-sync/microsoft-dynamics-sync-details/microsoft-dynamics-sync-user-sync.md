---
unique-page-id: 3571840
description: Microsoft Dynamics Sync - User Sync - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync - User Sync
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---

# Microsoft Dynamics Sync: Benutzersynchronisierung {#microsoft-dynamics-sync-user-sync}

Wussten Sie, dass Marketo Ihre gesamte Datenbank mit Dynamics synchronisiert? Es synchronisiert, wartet dann 5 Minuten und synchronisiert dann den ganzen Tag, jeden Tag. Hier sind einige Details darüber, wie Marketo Dynamics Accounts speziell behandelt.

Für die Integration benötigen Sie einen eigenen Microsoft Dynamics CRM-Benutzer. Wir nennen diesen Benutzer den Synchronisierungsbenutzer.

## Wie werden die Benutzerdetails zwischen den beiden Systemen synchronisiert? {#how-are-user-details-kept-in-sync-between-the-two-systems}

Die Benutzersynchronisierung ist eine Möglichkeit - Dynamics zu Marketo. Wenn Sie Änderungen an einem Benutzer in Dynamics vornehmen, werden die Änderungen in Marketo übernommen.

## Kann ich einen Benutzer mit Marketo erstellen? {#can-i-create-an-user-using-marketo}

Anz. Marketo kann keine Benutzer in Dynamics erstellen.

## Welche Felder werden mit Marketo synchronisiert? {#which-fields-will-sync-to-marketo}

Sie können die zu synchronisierenden Felder [während des Setups auswählen. ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-3-of-3-connect.md#select-fields-to-sync) Marketo synchronisiert jedoch nur die Felder, auf die Ihr Dynamics Sync-Benutzer Zugriff hat.
