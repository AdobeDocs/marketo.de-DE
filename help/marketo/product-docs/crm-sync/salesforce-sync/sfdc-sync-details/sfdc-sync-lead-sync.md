---
unique-page-id: 2953455
description: SFDC-Synchronisierung - Lead-Synchronisierung - Marketo-Dokumente - Produktdokumentation
title: SFDC-Synchronisierung - Lead-Synchronisierung
exl-id: cf38e091-7344-4b95-b9e1-77eda751c4a9
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '230'
ht-degree: 0%

---

# SFDC-Synchronisierung: Lead-Synchronisierung {#sfdc-sync-lead-sync}

Wussten Sie Marketo-Synchronisationen aus Ihrer [!DNL Salesforce]? Er synchronisiert, wartet 5 Minuten und synchronisiert dann erneut. Den ganzen Tag, jeden Tag. Im Folgenden finden Sie einige Details dazu, wie Marketo speziell mit [!DNL Salesforce] Leads umgeht.

## Synchronisationsrichtung {#sync-direction}

Die Lead- (Personen-) und Kontaktsynchronisierung erfolgt bidirektional. Wenn Sie Änderungen an einem Datensatz in [!DNL Salesforce] oder Marketo vornehmen, werden die Aktualisierungen auf beiden Systemen angezeigt.

## Was passiert, wenn Änderungen in beiden Systemen gleichzeitig vorgenommen werden? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo gewinnt. Es kommt selten vor, dass diese Art von Datenkollision auftritt.

## Kann ich mit Marketo einen Lead in [!DNL Salesforce] erstellen? {#can-i-create-a-lead-in-salesforce-using-marketo}

Ja, die [Person mit SFDC synchronisieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) verwenden. Dadurch wird ein Lead in [!DNL Salesforce] erstellt, wenn der Lead nicht vorhanden ist.

## Kann ich die Synchronisierung einer Person in Marketo mit einem Lead in [!DNL Salesforce] manuell erzwingen? {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

Ja, die Flussaktion [Person mit SFDC synchronisieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} wird in Echtzeit synchronisiert.

## Wird jedes Standardfeld mit Marketo synchronisiert? {#does-every-single-standard-field-sync-to-marketo}

Nein, nicht alle Standardfelder sind nützlich. Alle benutzerdefinierten Felder können Teil der Synchronisierung sein.

>[!NOTE]
>
>Marketo synchronisiert nur die Felder, auf die der [!DNL Salesforce] Synchronisierungsbenutzer Zugriff hat.

## Wird Marketo die [!DNL Salesforce] Validierungsregeln einhalten? {#will-marketo-respect-the-salesforce-validation-rules}

Ja. Die Synchronisierung schlägt fehl, wenn das Datenformat falsch ist oder erforderliche Feldinformationen fehlen. Marketo protokolliert in diesem Fall das Ergebnis im Aktivitätsprotokoll der Leads.
