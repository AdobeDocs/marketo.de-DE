---
description: Gründe für Protokollaufrufe und Ergebnisse von Aufrufen an Salesforce - Marketo Docs - Produktdokumentation
title: Gründe für Protokollaufrufe und Ergebnisse von Aufrufen an Salesforce
hide: true
hidefromtoc: true
source-git-commit: 1dd4a4f6bfac0b101f85f3776396aeef1a1f7182
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# Gründe für Protokollaufrufe und Ergebnisse von Aufrufen an Salesforce {#log-call-reasons-and-call-outcomes-to-salesforce}

Wenn Sie Aufrufergebnisse protokollieren und Salesforce aus Berichts- oder Sichtbarkeitsgründen aufrufen möchten, können Sie für jede Aktivität ein eigenes Aktivitätsfeld erstellen. Jedes Feld muss einen bestimmten API-Namen verwenden.

* API-Name für Aufrufergebnisse: mktosales_call_result
* API-Name der Aufrufgründe: mktosales_call_reason

Um diese Felder zu nutzen, müssen Sie zunächst das Feld als ein benutzerdefiniertes Aktivitätsfeld erstellen. Damit sie für Benutzer sichtbar ist, müssen Sie sie dem Seitenlayout der Aufgabenobjekte hinzufügen.

## Benutzerdefiniertes Aktivitätsfeld in Salesforce Classic erstellen  {#create-custom-activity-field-in-salesforce-classic}

1. Gehen Sie in Salesforce zu Einrichtung.

PICC

1. Geben Sie &quot;Aktivitäten&quot;in das Feld &quot;Schnellsuche&quot;ein.

PICC

1. Klicken **Benutzerdefinierte Aktivitätsfelder**.

PICC

1. Klicken **Neu**.

PICC

## Benutzerdefiniertes Aktivitätsfeld in Salesforce-Blitzen erstellen {#create-custom-activity-field-in-salesforce-lightning}

1. Klicken Sie in Salesforce auf das Zahnradsymbol oben rechts.

PICC

1. Klicken **Einrichtung**.

PICC

1. Klicken **Object Manager**.

PICC

1. Geben Sie in das Feld &quot;Schnellsuche&quot;die Aktivität ein und klicken Sie auf die Bezeichnung Aktivität , um die Objekteinrichtung zu öffnen.

PICC

1. Klicken Sie links auf **Felder und Beziehungen**.

PICC

1. Klicken **Neu**.

PICC

## Fügen Sie benutzerdefinierte Aktivitätsfelder zum Aufgabenseitenlayout in Salesforce Classic hinzu. {#add-custom-activity-field-to-task-page-layout-in-salesforce-classic}

SCHRITTE

## Fügen Sie benutzerdefiniertes Aktivitätsfeld zum Aufgabenseitenlayout in Salesforce-Blitzen hinzu {#add-custom-activity-field-to-task-page-layout-in-salesforce-lightning}

SCHRITTE

>[!MORELIKETHIS]
>
>[Installieren Sie die Ereignisfelder für &quot;Sales Connect&quot; in den Aktivitätsverlauf.](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/install-sales-connect-event-fields-on-activity-history.md)
