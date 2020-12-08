---
unique-page-id: 2953463
description: SFDC-Synchronisierung - Lead-/Kontoinhaber-Synchronisierung - Marketing-Dokumente - Produktdokumentation
title: SFDC-Synchronisierung - Synchronisierung von Interessenten/Kontoinhabern
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---


# SFDC-Synchronisierung: Synchronisierung von Interessenten-/Kontoinhabern {#sfdc-sync-lead-account-owner-sync}

Diese synchronisieren die &quot;Benutzer&quot;-Tabelle in Salesforce, wir werden sie jedoch als Interessenten-/Kontoinhaber-Felder bezeichnen.

## Welche Felder werden mit Marketo synchronisiert? {#which-fields-will-sync-to-marketo}

Für jede mit Marketo synchronisierte Person werden auch die folgenden Besitzerfelder synchronisiert:

* Vorname des Verkäufers
* Nachname des Verkäufers
* Name des Verkäufers
* Telefonnummer des Verkäufers
* E-Mail-Adresse des Verkäufers

Für jeden Kontakt werden die oben genannten fünf Felder mit Interessenteninhabern sowie die folgenden Felder mit Kontoinhabern synchronisiert:

* Vorname des Kontoinhabers
* Nachname des Kontoinhabers
* E-Mail-Adresse des Kontoinhabers

## Kann ich den Interessentenbesitzer in Marketo wechseln? {#can-i-change-the-lead-owner-in-marketo}

Verwenden Sie auf jeden Fall die Flussaktion &quot;Besitzer [ändern](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md) &quot;.

>[!NOTE]
>
>Sie können die Inhaberinformationen nicht auf der Seite &quot; [Personendetails verwenden&quot;ändern](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md).

## Was kann ich mit diesen Daten machen? {#what-can-i-do-with-this-data}

Es gibt viele Gründe, diese Daten zu verwenden, z. B.

* Senden Sie eine personalisierte E-Mail mit Unterschrift des Verkäufers
* Filtern Sie nach bestimmten Vertriebsmitteilungen, um die Effektivität zu analysieren oder zu analysieren.
* Zuweisungsregeln (und Neuzuweisungsregeln) in Marketo
* Verwenden Sie sie in den [Aktionen &quot;Eigentümer](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md)ändern&quot;, &quot; [Person zu SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md)synchronisieren&quot;und &quot;Aufgabe [](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) erstellen&quot;

Marketo hat eine fantastische Salesforce-Synchronisierung. Das macht sonst niemand so gut!
