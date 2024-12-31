---
unique-page-id: 3571840
description: Microsoft Dynamics-Synchronisierung - Benutzersynchronisierung - Marketo-Dokumente - Produktdokumentation
title: Microsoft Dynamics-Synchronisierung - Benutzersynchronisierung
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 0%

---

# Microsoft Dynamics-Synchronisierung: Benutzersynchronisierung {#microsoft-dynamics-sync-user-sync}

Wussten Sie, dass Marketo Engage Ihre gesamte Datenbank mit Dynamics synchronisiert? Er synchronisiert, wartet dann 5 Minuten und synchronisiert dann erneut, den ganzen Tag, jeden Tag. Im Folgenden finden Sie einige Details dazu, wie Marketo Dynamics-Konten spezifisch behandelt.

Für die Integration benötigen Sie einen dedizierten Microsoft Dynamics CRM-Benutzer. Dieser Benutzer wird als Synchronisierungsbenutzer bezeichnet.

## Wie werden die Benutzerdetails zwischen den beiden Systemen synchron gehalten? {#how-are-user-details-kept-in-sync-between-the-two-systems}

Die Benutzersynchronisierung erfolgt in eine Richtung - Dynamics zu Marketo. Wenn Sie in Dynamics Änderungen an einem Benutzer vornehmen, werden die Änderungen in Marketo übernommen.

## Kann ich Benutzende mit Marketo erstellen? {#can-i-create-an-user-using-marketo}

Nein. Marketo kann keine Benutzer in Dynamics erstellen.

## Welche Felder werden mit Marketo synchronisiert? {#which-fields-will-sync-to-marketo}

Sie können [ Setup Felder auswählen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync){target="_blank"} die synchronisiert werden sollen. Marketo synchronisiert jedoch nur die Felder, auf die der Dynamics-Synchronisierungsbenutzer Zugriff hat.
