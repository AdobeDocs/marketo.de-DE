---
unique-page-id: 2953463
description: SFDC-Synchronisierung - Synchronisation von Lead-/Kontoinhabern - Marketo-Dokumente - Produktdokumentation
title: SFDC Sync - Synchronisierung von Lead-/Kontoinhabern
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 13%

---

# SFDC-Synchronisation: Synchronisation von Lead-/Kontoinhabern {#sfdc-sync-lead-account-owner-sync}

Diese synchronisieren technisch die &quot;Benutzer&quot;-Tabelle in Salesforce, werden jedoch als &quot;Lead-/Kontoeigentümer&quot;-Felder bezeichnet.

## Welche Felder werden mit Marketo synchronisiert? {#which-fields-will-sync-to-marketo}

Für jede mit Marketo synchronisierte Person werden auch die folgenden Eigentümerfelder synchronisiert:

* Vorname des Verkaufseigentümers
* Nachname des Verkaufseigentümers
* Name des Vertriebsmitarbeiters
* Telefonnummer des Verkaufseigentümers
* E-Mail-Adresse des Verkaufseigentümers

Für jeden Kontakt werden die oben genannten fünf Lead-Eigentümer-Felder sowie diese Kontoinhaberfelder synchronisiert:

* Vorname des Kontoeigentümers
* Nachname des Kontoeigentümers
* E-Mail-Adresse des Kontoeigentümers

## Kann ich den Lead-Inhaber in Marketo ändern? {#can-i-change-the-lead-owner-in-marketo}

Absolut: Verwenden Sie einfach die [Inhaber ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md) Flussaktion.

>[!NOTE]
>
>Sie können die Eigentümerinformationen nicht mit dem [Verwenden der Seite &quot;Personendetails&quot;](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

## Was kann ich mit diesen Daten machen? {#what-can-i-do-with-this-data}

Es gibt viele Gründe für die Verwendung dieser Daten, z. B.

* Senden einer personalisierten E-Mail mit der Unterschrift des Eigentümers des Verkaufs
* Filtern nach bestimmten Vertriebsmitarbeitern für Marketing- oder Analyse der Effektivität
* Zuweisungs- (und Neuzuweisungsregeln) in Marketo
* Verwenden Sie sie im [Inhaber ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md), [Person mit SFDC synchronisieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md), und [Aufgabe erstellen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) Flussaktionen

Marketo verfügt über eine fantastische Salesforce-Synchronisation. Niemand sonst macht es so gut!
