---
unique-page-id: 2953463
description: Erfahren Sie, wie die Felder für Lead- und Kontoinhaber von Salesforce mit Marketo synchronisiert werden. Ändern Sie den Lead-Inhaber in Marketo und verwenden Sie die Daten des Verantwortlichen in Flussaktionen und Smart Lists.
title: SFDC-Synchronisierung - Synchronisierung von Lead/Kontoinhaber
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
feature: Salesforce Integration
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 14%

---

# SFDC-Synchronisierung: Synchronisierung von Leads/Kontoinhaberinnen bzw. Kontoinhabern {#sfdc-sync-lead-account-owner-sync}

Diese synchronisieren technisch die Tabelle „Benutzer“ in [!DNL Salesforce]. Wir bezeichnen sie jedoch als Lead-/Kontoinhaberfelder.

## Welche Felder werden mit Marketo Engage synchronisiert? {#which-fields-will-sync-to-marketo-engage}

Für jede mit Marketo synchronisierte Person synchronisieren wir auch die folgenden Besitzerfelder:

* Vorname des Verkaufseigentümers
* Nachname des Verkaufseigentümers
* Titel des Vertriebsinhabers
* Telefonnummer des Verkaufseigentümers
* E-Mail-Adresse des Verkaufseigentümers

Für jeden Kontakt synchronisieren wir die oben genannten fünf Felder für den Lead-Inhaber sowie diese Felder für den Kontoinhaber:

* Vorname des Kontoeigentümers
* Nachname des Kontoeigentümers
* E-Mail Adresse des Kontoeigentümers

## Kann ich den Lead-Inhaber in Marketo ändern? {#can-i-change-the-lead-owner-in-marketo}

Absolut, verwenden Sie einfach die [Besitzer ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"} Flussaktion.

>[!NOTE]
>
>Sie können die Besitzerinformationen nicht über die Seite [Verwenden der Personendetailseite“ ](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/using-the-person-detail-page.md){target="_blank"}.

## Was kann ich mit diesen Daten tun? {#what-can-i-do-with-this-data}

Es gibt viele Gründe, diese Daten zu verwenden, z. B.

* Senden einer personalisierten E-Mail mit Unterschrift des Verkäufers
* Filtern Sie nach spezifischen Vertriebsmitarbeitern für die Marketing-Analyse oder sogar die Effektivitätsanalyse.
* Zuweisungsregeln (und Neuzuweisungsregeln) in Marketo
* Verwenden Sie sie in den [Besitzer ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/change-owner.md){target="_blank"}, [Person mit SFDC synchronisieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} und [Aufgabe erstellen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} Flussaktionen

Marketo verfügt über eine hervorragende [!DNL Salesforce]. Niemand sonst macht es so gut!
