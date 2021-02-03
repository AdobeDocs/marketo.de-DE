---
unique-page-id: 2953459
description: SFDC-Synchronisierung - Kontosynchronisierung - Marketing Docs - Produktdokumentation
title: SFDC-Synchronisierung - Kontosynchronisierung
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 0%

---


# SFDC-Synchronisierung: Kontosynchronisierung {#sfdc-sync-account-sync}

Marketo synchronisiert auch Ihre Kontoinformationen mit Salesforce. Hier sind einige spezielle Dinge, die Sie wissen sollten!

## Auf welche Weise werden die Informationen synchronisiert? {#which-way-does-the-information-sync}

Nur eine Möglichkeit: von SFDC nach Marketo.

## Wie funktionieren die Updates? {#how-do-the-updates-work}

Wenn Sie ein Feld für ein Konto für einen Kontakt in Marketo aktualisieren, ändert es die Werte aller Kontakte, die zu diesem Konto in Marketo gehören. Es wird nicht mit dem SFDC synchronisiert. Bei der nächsten Aktualisierung dieses Kontos im SFDC werden jedoch alle Kontoinformationen in Marketo durch die Änderungen außer Kraft gesetzt.

## Kann ein Kontakt zu mehreren Konten gehören?  {#can-a-contact-belong-to-multiple-accounts}

Anzahl Ein Konto kann viele Kontakte haben, ein Kontakt kann nur ein Konto haben.

## Kann ich aus Marketo Konten erstellen? {#can-i-create-accounts-from-marketo}

Meistens, nein. Wenn Sie jedoch den Schritt [Person](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md) konvertieren für eine Person verwenden, wird ein neuer Kontakt, ein neues Konto und eine neue Chance erstellt.

>[!CAUTION]
>
>Dieser Flussschritt hat einen sehr begrenzten Anwendungsfall. Wenn Sie sich nicht sicher sind, sollten Sie es wahrscheinlich nicht benutzen.

## Führt eine Änderung in einem Kontofeld in Salesforce zu einem Änderungs-Datenwertprotokoll für jede Aktivität?  {#does-a-change-in-an-account-field-in-salesforce-result-in-a-change-data-value-activity-log-for-each-contact}

Meistens ja. Wenn jedoch ein Konto mehr als 5.000 Kontakte hat und sich ein Feld auf diesem Konto im SFDC ändert, wird die Änderung synchronisiert, aber die Aktivität für die 5.000+ Kontakte wird nicht protokolliert.
