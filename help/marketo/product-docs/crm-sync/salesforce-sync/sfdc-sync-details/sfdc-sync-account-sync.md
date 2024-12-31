---
unique-page-id: 2953459
description: SFDC-Synchronisierung - Kontosynchronisierung - Marketo-Dokumente - Produktdokumentation
title: SFDC-Synchronisierung - Kontosynchronisierung
exl-id: 94f7a9e5-86ea-4bb4-9d78-96a09c61321d
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 0%

---

# SFDC-Synchronisierung: Kontosynchronisierung {#sfdc-sync-account-sync}

Marketo Engage synchronisiert auch Ihre Kontoinformationen mit Salesforce. Hier sind einige spezifische Dinge, die Sie wissen sollten!

## Auf welche Weise werden die Informationen synchronisiert? {#which-way-does-the-information-sync}

Nur eine Möglichkeit: von SFDC nach Marketo.

## Wie funktionieren die Aktualisierungen? {#how-do-the-updates-work}

Wenn Sie ein Kontofeld für einen Kontakt in Marketo aktualisieren, werden die Werte aller Kontakte geändert, die zu diesem Konto in Marketo gehören. Es wird nicht mit SFDC synchronisiert. Wenn dieses Konto jedoch das nächste Mal in SFDC aktualisiert wird, überschreiben die Änderungen alle Kontoinformationen in Marketo.

## Kann ein Kontakt mehreren Konten angehören?  {#can-a-contact-belong-to-multiple-accounts}

Nein. Ein Konto kann viele Kontakte haben, ein Kontakt kann nur ein Konto haben.

## Kann ich über Marketo Konten erstellen? {#can-i-create-accounts-from-marketo}

Meistens nicht. Wenn Sie jedoch den Flussschritt [Person ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"}) für eine Person verwenden, wird ein neuer Kontakt, ein neues Konto und eine neue Opportunity erstellt.

>[!CAUTION]
>
>Dieser Flussschritt hat einen sehr eingeschränkten Anwendungsfall. Wenn Sie sich nicht sicher sind, sollten Sie es wahrscheinlich nicht verwenden.

## Führt eine Änderung an einem Kontofeld in Salesforce zu einem Aktivitätsprotokoll „Datenwert ändern“ für jeden Kontakt?  {#does-a-change-in-an-account-field-in-salesforce-result-in-a-change-data-value-activity-log-for-each-contact}

Meistens ja. Wenn ein Konto jedoch mehr als 5.000 Kontakte hat und sich ein Feld in diesem Konto in SFDC ändert, synchronisieren wir die Änderung, protokollieren jedoch nicht die Aktivität für die über 5.000 Kontakte.
