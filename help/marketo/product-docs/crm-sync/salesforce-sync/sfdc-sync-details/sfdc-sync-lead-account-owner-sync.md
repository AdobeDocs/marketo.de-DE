---
unique-page-id: 2953463
description: SFDC-Synchronisierung - Lead-/Kontoinhaber-Synchronisierung - Marketo Dokumente - Produktdokumentation
title: SFDC-Synchronisierung - Synchronisierung von Interessenten/Kontoinhabern
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 13%

---

# SFDC-Synchronisierung: Interessenten-/Kontoinhaber-Synchronisierung {#sfdc-sync-lead-account-owner-sync}

Diese synchronisieren die &quot;Benutzer&quot;-Tabelle in Salesforce, wir werden sie jedoch als Interessenten-/Kontoinhaber-Felder bezeichnen.

## Welche Felder werden mit Marketo synchronisiert? {#which-fields-will-sync-to-marketo}

Für jede mit Marketo synchronisierte Person werden auch die folgenden Besitzerfelder synchronisiert:

* Vorname des Vertriebseigentümers
* Nachname des Vertriebseigentümers
* Name des Verkäufers
* Telefonnummer des Vertriebseigentümers
* E-Mail-Adresse des Vertriebseigentümers

Für jeden Kontakt werden die oben genannten fünf Felder mit Interessenteninhabern sowie die folgenden Felder mit Kontoinhabern synchronisiert:

* Vorname des Kontoeigentümers
* Nachname des Kontoeigentümers
* E-Mail Adresse des Kontoeigentümers

## Kann ich den Interessentenbesitzer in Marketo wechseln? {#can-i-change-the-lead-owner-in-marketo}

Verwenden Sie unbedingt die Flussaktion [Eigentümer ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md).

>[!NOTE]
>
>Sie können die Inhaberinformationen nicht mit der [Seite mit Personendetails](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md) ändern.

## Was kann ich mit diesen Daten machen? {#what-can-i-do-with-this-data}

Es gibt viele Gründe, diese Daten zu verwenden, z. B.

* Senden Sie eine personalisierte E-Mail mit Unterschrift des Verkäufers
* Filtern Sie nach bestimmten Vertriebsmitteilungen, um die Effektivität zu analysieren oder zu analysieren.
* Zuweisungsregeln (und Neuzuweisungsregeln) in Marketo
* Verwenden Sie sie in den Aktionen [Eigentümer ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md), [Person zu SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) synchronisieren und [Aufgabe erstellen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md)

Marketo hat eine fantastische Salesforce-Synchronisierung. Das macht sonst niemand so gut!
