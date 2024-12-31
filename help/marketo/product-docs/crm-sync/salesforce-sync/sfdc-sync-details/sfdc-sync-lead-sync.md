---
unique-page-id: 2953455
description: SFDC-Synchronisierung - Lead-Synchronisierung - Marketo-Dokumente - Produktdokumentation
title: SFDC-Synchronisierung - Lead-Synchronisierung
exl-id: cf38e091-7344-4b95-b9e1-77eda751c4a9
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 0%

---

# SFDC-Synchronisierung: Lead-Synchronisierung {#sfdc-sync-lead-sync}

Wussten Sie Marketo Engage-Synchronisationen aus Ihrer Salesforce-Datenbank? Er synchronisiert, wartet 5 Minuten und synchronisiert dann erneut. Den ganzen Tag, jeden Tag. Im Folgenden finden Sie einige Details dazu, wie Marketo speziell mit Salesforce-Leads umgeht.

## Synchronisationsrichtung {#sync-direction}

Die Lead- (Personen-) und Kontaktsynchronisierung erfolgt bidirektional. Wenn Sie Änderungen an einem Datensatz in Salesforce oder Marketo vornehmen, werden die Aktualisierungen auf beiden Systemen angezeigt.

## Was passiert, wenn Änderungen in beiden Systemen gleichzeitig vorgenommen werden? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo gewinnt. Es kommt selten vor, dass diese Art von Datenkollision auftritt.

## Kann ich mit Marketo einen Lead in Salesforce erstellen? {#can-i-create-a-lead-in-salesforce-using-marketo}

Ja, die [Person mit SFDC synchronisieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} verwenden. Dadurch wird ein Lead in Salesforce erstellt, wenn der Lead nicht vorhanden ist.

## Kann ich die Synchronisierung einer Person in Marketo mit einem Lead in Salesforce manuell erzwingen? {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

Ja, die Flussaktion [Person mit SFDC synchronisieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} wird in Echtzeit synchronisiert.

## Wird jedes Standardfeld mit Marketo synchronisiert? {#does-every-single-standard-field-sync-to-marketo}

Nein, nicht alle Standardfelder sind nützlich. Alle benutzerdefinierten Felder können Teil der Synchronisierung sein.

>[!NOTE]
>
>Marketo synchronisiert nur die Felder, auf die der Salesforce-Synchronisierungsbenutzer Zugriff hat.

## Hält Marketo die Salesforce-Validierungsregeln ein? {#will-marketo-respect-the-salesforce-validation-rules}

Ja. Die Synchronisierung schlägt fehl, wenn das Datenformat falsch ist oder erforderliche Feldinformationen fehlen. Marketo protokolliert in diesem Fall das Ergebnis im Aktivitätsprotokoll der Leads.
