---
unique-page-id: 2953457
description: SFDC Sync - Kontaktsynchronisierung - Marketo-Dokumente - Produktdokumentation
title: SFDC Sync - Kontaktsynchronisierung
exl-id: 537bbc95-9233-4454-892e-81f962cf729d
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# SFDC Sync: Kontaktsynchronisierung {#sfdc-sync-contact-sync}

Wussten Sie, dass Marketo Engage Ihre gesamte Datenbank mit Salesforce synchronisiert? Es wird synchronisiert, dann 5 Minuten wartet und dann wieder synchronisiert, den ganzen Tag, jeden Tag. Im Folgenden finden Sie einige Details dazu, wie Marketo Salesforce-Kontakte spezifisch behandelt.

## Synchronisierungsrichtung {#sync-direction}

Die Synchronisation von Kontakten erfolgt bidirektional. Wenn Sie Änderungen an einem Kontakt in Salesforce oder Marketo vornehmen, spiegeln sich Ihre Aktualisierungen in beiden Systemen wider.

## Was passiert, wenn beide Systeme gleichzeitig geändert werden? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Wir sind nett und lassen Salesforce gewinnen. Es ist selten, dass diese Art von Datenkollision auftritt.

## Kann ich eine Person in einen Kontakt in Marketo umwandeln? {#can-i-convert-a-person-into-a-contact-in-marketo}

Ja, verwenden Sie die **[Person konvertieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"}** Flussaktion.

>[!CAUTION]
>
>Das Konvertieren einer Person in Marketo wird zu einem neuen Konto und einer neuen Möglichkeit in Salesforce führen. Wenn Sie keine doppelten Konten möchten, verwenden Sie Salesforce zur Konvertierung.

## Kann ich die Synchronisierung eines Kontakts manuell erzwingen? {#can-i-manually-force-a-sync-of-a-contact}

Ja, verwenden Sie die **[Person mit SFDC synchronisieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}** Flussaktion und sie wird in Echtzeit synchronisiert.

## Synchronisiert jedes Standardfeld mit Marketo? {#does-every-single-standard-field-sync-to-marketo}

Nein, nicht alle Standardfelder sind nützlich. Alle benutzerdefinierten Felder können Teil der Synchronisierung sein.

>[!NOTE]
>
>Marketo synchronisiert nur die Felder, auf die Ihr Marketo Sync User Zugriff hat.

## Wird Marketo die Salesforce-Validierungsregeln einhalten? {#will-marketo-respect-the-salesforce-validation-rules}

Ja, wenn ein Konflikt vorliegt, wird das Ergebnis im Interessenten-Aktivitätsprotokoll protokolliert.
