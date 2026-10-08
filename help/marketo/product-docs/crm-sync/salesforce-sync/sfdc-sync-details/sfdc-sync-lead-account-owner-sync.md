---
unique-page-id: 2953463
description: Erfahren Sie, wie die Felder für Lead- und Kontoinhaber von Salesforce mit Marketo synchronisiert werden. Ändern Sie den Lead-Inhaber in Marketo und verwenden Sie die Daten des Verantwortlichen in Flussaktionen und Smart Lists.
title: SFDC-Synchronisierung - Synchronisierung von Lead/Kontoinhaber
exl-id: b9effcc2-f426-4390-aef1-42f4e525b182
feature: Salesforce Integration
TQID: 'https://experienceleague.adobe.com/hw4ZXOFSDBvVm45z84aQkxgKU17O-8h1NhukpGCNsos'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: edcca97f-2314-445f-9a79-3ac30a2a9c27
    internal-label: Salesforce integration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 15%
---
# SFDC-Synchronisierung: Synchronisierung von Lead-/Account-Inhabern {#sfdc-sync-lead-account-owner-sync}

Diese synchronisieren technisch die Tabelle „Benutzer“ in [!DNL Salesforce]. Wir bezeichnen sie jedoch als Lead-/Kontoinhaberfelder.

## Welche Felder werden mit Marketo Engage synchronisiert? {#which-fields-will-sync-to-marketo-engage}

Für jede mit Marketo synchronisierte Person synchronisieren wir auch die folgenden Besitzerfelder:

* Vorname des Verkaufsinhabers
* Nachname des Verkaufsinhabers
* Titel des Vertriebsinhabers
* Telefonnummer des Verkaufsinhabers
* E-Mail-Adresse des Verkaufsinhabers

Für jeden Kontakt synchronisieren wir die oben genannten fünf Felder für den Lead-Inhaber sowie diese Felder für den Kontoinhaber:

* Vorname des Account-Inhabers
* Nachname des Account-Inhabers
* E-Mail-Adresse des Account-Inhabers

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

