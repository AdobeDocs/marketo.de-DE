---
unique-page-id: 2953455
description: Erfahren Sie, wie die Lead-Synchronisierung zwischen Salesforce und Marketo funktioniert. Bidirektionale Synchronisierung verstehen, Leads aus Marketo erstellen und Validierungsregeln einhalten.
title: SFDC-Synchronisierung - Lead-Synchronisierung
exl-id: cf38e091-7344-4b95-b9e1-77eda751c4a9
feature: Salesforce Integration
TQID: 'https://experienceleague.adobe.com/zqztwtX4Xe08Df-v1aTxhRi-cB2CZALctr3kaFNrT7s'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
    internal-label: Database
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: edcca97f-2314-445f-9a79-3ac30a2a9c27
    internal-label: Salesforce integration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 2%
---
# SFDC Sync: Lead Sync {#sfdc-sync-lead-sync}

Marketo synchronisiert aus Ihrer [!DNL Salesforce]. Er synchronisiert, wartet 5 Minuten und synchronisiert dann erneut. Den ganzen Tag, jeden Tag. Im Folgenden finden Sie einige Details dazu, wie Marketo speziell mit [!DNL Salesforce] Leads umgeht.

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
