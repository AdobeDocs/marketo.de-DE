---
unique-page-id: 2953457
description: SFDC-Synchronisierung - Kontaktsynchronisierung - Marketo-Dokumente - Produktdokumentation
title: SFDC-Synchronisierung - Kontaktsynchronisierung
exl-id: 537bbc95-9233-4454-892e-81f962cf729d
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# SFDC-Synchronisierung: Kontaktsynchronisierung {#sfdc-sync-contact-sync}

Wussten Sie, dass Marketo Engage Ihre gesamte Datenbank mit Salesforce synchronisiert? Er synchronisiert, wartet dann 5 Minuten und synchronisiert dann erneut, den ganzen Tag, jeden Tag. Im Folgenden finden Sie einige Informationen darüber, wie Marketo speziell mit Salesforce-Kontakten umgeht.

## Synchronisationsrichtung {#sync-direction}

Die Kontaktsynchronisation erfolgt bidirektional. Wenn Sie Änderungen an einem Kontakt in Salesforce oder Marketo vornehmen, werden Ihre Aktualisierungen auf beiden Systemen angezeigt.

## Was passiert, wenn Änderungen in beiden Systemen gleichzeitig vorgenommen werden? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Wir sind nett und lassen Salesforce gewinnen. Es kommt selten vor, dass diese Art von Datenkollision auftritt.

## Kann ich eine Person in Marketo in einen Kontakt konvertieren? {#can-i-convert-a-person-into-a-contact-in-marketo}

Ja, die Flussaktion **[Person konvertieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"}** verwenden.

>[!CAUTION]
>
>Die Konvertierung einer Person in Marketo führt zu einem neuen Konto und einer neuen Opportunity in Salesforce. Wenn doppelte Konten nicht gewünscht werden, konvertieren Sie sie mithilfe von Salesforce.

## Kann ich die Synchronisierung eines Kontakts manuell erzwingen? {#can-i-manually-force-a-sync-of-a-contact}

Ja, die Flussaktion **[Person mit SFDC synchronisieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}** wird in Echtzeit synchronisiert.

## Wird jedes Standardfeld mit Marketo synchronisiert? {#does-every-single-standard-field-sync-to-marketo}

Nein, nicht alle Standardfelder sind nützlich. Alle benutzerdefinierten Felder können Teil der Synchronisierung sein.

>[!NOTE]
>
>Marketo synchronisiert nur die Felder, auf die Ihr Marketo-Synchronisierungsbenutzer Zugriff hat.

## Hält Marketo die Salesforce-Validierungsregeln ein? {#will-marketo-respect-the-salesforce-validation-rules}

Ja, wenn ein Konflikt auftritt, wird das Ergebnis im Aktivitätsprotokoll des Leads protokolliert.
