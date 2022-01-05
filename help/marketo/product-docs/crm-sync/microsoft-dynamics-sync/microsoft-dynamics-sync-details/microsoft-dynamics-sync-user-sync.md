---
unique-page-id: 3571840
description: Microsoft Dynamics Sync - Benutzersynchronisierung - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync - Benutzersynchronisierung
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
source-git-commit: 17cacaa56a437a568bd0d2cc23020f3f880eaf52
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 0%

---

# Microsoft Dynamics Sync: Benutzersynchronisierung {#microsoft-dynamics-sync-user-sync}

Wussten Sie, dass Marketo Ihre gesamte Datenbank mit Dynamics synchronisiert? Es wird synchronisiert, dann 5 Minuten wartet und dann wieder synchronisiert, den ganzen Tag, jeden Tag. Im Folgenden finden Sie einige Details dazu, wie Marketo Dynamics-Konten spezifisch behandelt.

Für die Integration benötigen Sie einen dedizierten Microsoft Dynamics CRM-Benutzer. Wir nennen diesen Benutzer &quot;Sync User&quot;.

## Wie werden Benutzerdetails zwischen den beiden Systemen synchronisiert? {#how-are-user-details-kept-in-sync-between-the-two-systems}

Die Benutzersynchronisierung ist eine Möglichkeit - Dynamics zu Marketo. Wenn Sie in Dynamics Änderungen an einem Benutzer vornehmen, werden die Änderungen in Marketo übernommen.

## Kann ich einen Benutzer mit Marketo erstellen? {#can-i-create-an-user-using-marketo}

Anz. Marketo kann keine Benutzer in Dynamics erstellen.

## Welche Felder werden mit Marketo synchronisiert? {#which-fields-will-sync-to-marketo}

Sie können [Auswahl der zu synchronisierenden Felder](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-4-of-4-connect.md#select-fields-to-sync) während der Einrichtung. Marketo synchronisiert jedoch nur die Felder, auf die der Benutzer für die Synchronisierung mit Dynamics Zugriff hat.
