---
unique-page-id: 3571840
description: Microsoft Dynamics Sync - User Sync - Marketo Docs - Produktdokumentation
title: Microsoft Dynamics Sync - User Sync
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Benutzersynchronisierung {#microsoft-dynamics-sync-user-sync}

Wussten Sie, dass Marketo Ihre gesamte Datenbank mit Dynamics synchronisiert? Es synchronisiert, wartet dann 5 Minuten und synchronisiert dann den ganzen Tag, jeden Tag. Hier sind einige Details darüber, wie Marketo Dynamics Accounts speziell behandelt.

Für die Integration benötigen Sie einen eigenen Microsoft Dynamics CRM-Benutzer. Wir nennen diesen Benutzer den Synchronisierungsbenutzer.

## Wie werden die Benutzerdetails zwischen den beiden Systemen synchronisiert? {#how-are-user-details-kept-in-sync-between-the-two-systems}

Die Benutzersynchronisierung ist eine Möglichkeit - Dynamik zu Marketo. Wenn Sie Änderungen an einem Benutzer in Dynamics vornehmen, werden die Änderungen in Marketo übernommen.

## Kann ich einen Benutzer mit Marketo erstellen? {#can-i-create-an-user-using-marketo}

Anzahl Marketo kann keine Benutzer in Dynamics erstellen.

## Welche Felder werden mit Marketo synchronisiert? {#which-fields-will-sync-to-marketo}

Sie können Felder [auswählen, die während der Einrichtung synchronisiert](https://docs.marketo.com/pages/viewpage.action?pageId=3571830#Step3of3:ConnectMicrosoftDynamicswithMarketo(Online)-SelectFieldstoSync) werden sollen. Marketo synchronisiert jedoch nur die Felder, auf die Ihr Dynamics Sync-Benutzer Zugriff hat.
