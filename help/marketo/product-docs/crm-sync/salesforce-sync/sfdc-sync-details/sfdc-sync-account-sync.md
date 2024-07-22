---
unique-page-id: 2953459
description: SFDC Sync - Kontosynchronisierung - Marketo-Dokumente - Produktdokumentation
title: SFDC Sync - Kontosynchronisierung
exl-id: 94f7a9e5-86ea-4bb4-9d78-96a09c61321d
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 0%

---

# SFDC Sync: Kontosynchronisierung {#sfdc-sync-account-sync}

Marketo Engage synchronisiert Ihre Kontoinformationen auch mit Salesforce. Hier sind einige spezielle Dinge, die Sie wissen sollten!

## Wie werden die Informationen synchronisiert? {#which-way-does-the-information-sync}

Nur eine Möglichkeit: von SFDC nach Marketo.

## Wie funktionieren die Aktualisierungen? {#how-do-the-updates-work}

Wenn Sie ein Feld &quot;Konto&quot;für einen Kontakt in Marketo aktualisieren, werden die Werte aller Kontakte geändert, die zu diesem Konto in Marketo gehören. Es wird nicht mit SFDC synchronisiert. Wenn dieses Konto jedoch das nächste Mal im SFDC aktualisiert wird, werden alle Kontoinformationen in Marketo durch die Änderungen überschrieben.

## Kann ein Kontakt mehreren Konten angehören?  {#can-a-contact-belong-to-multiple-accounts}

Anz. Ein Konto kann viele Kontakte haben, ein Kontakt kann nur ein Konto haben.

## Kann ich Konten aus Marketo erstellen? {#can-i-create-accounts-from-marketo}

Meistens nein. Wenn Sie jedoch den Schritt [Person konvertieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"} für eine Person verwenden, werden ein neuer Kontakt, ein neues Konto und eine neue Chance erstellt.

>[!CAUTION]
>
>Dieser Flussschritt hat einen sehr begrenzten Anwendungsfall. Wenn du dir nicht sicher bist, solltest du es wahrscheinlich nicht benutzen.

## Führt eine Änderung in einem Feld &quot;Konto&quot;in Salesforce zu einem Aktivitätsprotokoll &quot;Datenwert ändern&quot;für jeden Kontakt?  {#does-a-change-in-an-account-field-in-salesforce-result-in-a-change-data-value-activity-log-for-each-contact}

Meistens ja. Wenn jedoch ein Konto mehr als 5.000 Kontakte hat und sich ein Feld auf diesem Konto in SFDC ändert, synchronisieren wir die Änderung, protokollieren aber die Aktivität nicht für mehr als 5.000 Kontakte.
