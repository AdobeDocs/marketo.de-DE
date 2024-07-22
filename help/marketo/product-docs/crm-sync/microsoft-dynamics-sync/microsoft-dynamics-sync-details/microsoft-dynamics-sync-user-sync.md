---
unique-page-id: 3571840
description: Microsoft Dynamics Sync - Benutzersynchronisierung - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync - Benutzersynchronisierung
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 0%

---

# Microsoft Dynamics Sync: Benutzersynchronisierung {#microsoft-dynamics-sync-user-sync}

Wussten Sie, dass Marketo Engage Ihre gesamte Datenbank mit Dynamics synchronisiert? Es wird synchronisiert, dann 5 Minuten wartet und dann wieder synchronisiert, den ganzen Tag, jeden Tag. Im Folgenden finden Sie einige Details dazu, wie Marketo Dynamics-Konten spezifisch behandelt.

Für die Integration benötigen Sie einen dedizierten Microsoft Dynamics CRM-Benutzer. Wir nennen diesen Benutzer &quot;Sync User&quot;.

## Wie werden Benutzerdetails zwischen den beiden Systemen synchronisiert? {#how-are-user-details-kept-in-sync-between-the-two-systems}

Die Benutzersynchronisierung ist eine Möglichkeit - Dynamics zu Marketo. Wenn Sie in Dynamics Änderungen an einem Benutzer vornehmen, werden die Änderungen in Marketo übernommen.

## Kann ich einen Benutzer mit Marketo erstellen? {#can-i-create-an-user-using-marketo}

Anz. Marketo kann keine Benutzer in Dynamics erstellen.

## Welche Felder werden mit Marketo synchronisiert? {#which-fields-will-sync-to-marketo}

Sie können [ Felder auswählen, die während der Einrichtung synchronisiert werden sollen. ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} Marketo synchronisiert jedoch nur die Felder, auf die der Benutzer für die Synchronisierung mit Dynamics Zugriff hat.
