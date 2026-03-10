---
unique-page-id: 3571840
description: Erfahren Sie, wie Benutzerdaten von Microsoft Dynamics mit Marketo synchronisiert werden. Erfahren Sie, welche Besitzerfelder synchronisiert werden und wie Sie sie in Smart Lists und Flussaktionen verwenden.
title: Microsoft [!DNL Dynamics] Sync -Benutzersynchronisierung
exl-id: d642d4d2-2beb-42c6-a6b2-3da5df1cd9c8
feature: Microsoft Dynamics
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---

# Microsoft [!DNL Dynamics] Sync.: Benutzersynchronisierung {#microsoft-dynamics-sync-user-sync}

Wussten Sie, dass Marketo Ihre gesamte Datenbank mit [!DNL Dynamics] synchronisiert? Er synchronisiert, wartet dann 5 Minuten und synchronisiert dann erneut, den ganzen Tag, jeden Tag. Im Folgenden finden Sie einige Details dazu, wie Marketo [!DNL Dynamics]-Konten spezifisch behandelt.

Für die Integration benötigen Sie einen dedizierten Microsoft [!DNL Dynamics] CRM-Benutzer. Dieser Benutzer wird als Synchronisierungsbenutzer bezeichnet.

## Wie werden die Benutzerdetails zwischen den beiden Systemen synchron gehalten? {#how-are-user-details-kept-in-sync-between-the-two-systems}

Die Benutzersynchronisierung erfolgt in eine Richtung - [!DNL Dynamics] zu Marketo. Wenn Sie in [!DNL Dynamics] Änderungen an einer Benutzerin oder einem Benutzer vornehmen, werden diese Änderungen in Marketo übernommen.

## Kann ich Benutzende mit Marketo erstellen? {#can-i-create-an-user-using-marketo}

Nein. Marketo kann keine Benutzenden in [!DNL Dynamics] erstellen.

## Welche Felder werden mit Marketo synchronisiert? {#which-fields-will-sync-to-marketo}

Sie können [&#x200B; Setup Felder auswählen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-4-of-4-connect.md#select-fields-to-sync) die synchronisiert werden sollen. Marketo synchronisiert jedoch nur die Felder, auf die der [!DNL Dynamics] Synchronisierungsbenutzer Zugriff hat.
