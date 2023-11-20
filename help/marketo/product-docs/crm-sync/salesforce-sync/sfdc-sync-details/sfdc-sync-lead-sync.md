---
unique-page-id: 2953455
description: SFDC Sync - Lead Sync - Marketo Docs - Produktdokumentation
title: SFDC Sync - Lead Sync
exl-id: cf38e091-7344-4b95-b9e1-77eda751c4a9
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 0%

---

# SFDC Sync: Lead Sync {#sfdc-sync-lead-sync}

Wussten Sie Marketo Engage-Synchronisationen aus Ihrer Salesforce-Datenbank? Es wird synchronisiert, 5 Minuten wartet und dann erneut synchronisiert. Den ganzen Tag, jeden Tag. Im Folgenden finden Sie einige Details dazu, wie Marketo Salesforce-Leads spezifisch behandelt.

## Synchronisierungsrichtung {#sync-direction}

Die Synchronisation von Lead (Person) und Kontakt erfolgt bidirektional. Wenn Sie Änderungen an einem Datensatz in Salesforce oder Marketo vornehmen, werden Ihre Aktualisierungen in beiden Systemen übernommen.

## Was passiert, wenn beide Systeme gleichzeitig geändert werden? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo gewinnt. Es ist selten, dass diese Art von Datenkollision auftritt.

## Kann ich mit Marketo einen Lead in Salesforce erstellen? {#can-i-create-a-lead-in-salesforce-using-marketo}

Ja, verwenden Sie die [Person mit SFDC synchronisieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} Flussaktion. Dadurch wird ein Lead in Salesforce erstellt, wenn der Lead nicht vorhanden ist.

## Kann ich in Salesforce manuell die Synchronisierung einer Person in Marketo mit einem Lead erzwingen? {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

Ja, verwenden Sie die [Person mit SFDC synchronisieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} Flussaktion und sie wird in Echtzeit synchronisiert.

## Synchronisiert jedes Standardfeld mit Marketo? {#does-every-single-standard-field-sync-to-marketo}

Nein, nicht alle Standardfelder sind nützlich. Alle benutzerdefinierten Felder können Teil der Synchronisierung sein.

>[!NOTE]
>
>Marketo synchronisiert nur die Felder, auf die Ihr Salesforce-Synchronisierungsbenutzer Zugriff hat.

## Wird Marketo die Salesforce-Validierungsregeln einhalten? {#will-marketo-respect-the-salesforce-validation-rules}

Ja. Die Synchronisierung schlägt fehl, wenn das Datenformat falsch ist oder die erforderlichen Feldinformationen fehlen. In diesem Fall protokolliert Marketo das Ergebnis im Lead-Aktivitätsprotokoll.
