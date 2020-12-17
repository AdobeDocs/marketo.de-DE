---
unique-page-id: 2953457
description: SFDC-Synchronisierung - Kontaktsynchronisierung - Marketing-Dokumente - Produktdokumentation
title: SFDC-Synchronisierung - Kontaktsynchronisierung
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '235'
ht-degree: 0%

---


# SFDC-Synchronisierung: Kontaktsynchronisierung {#sfdc-sync-contact-sync}

Wussten Sie, dass Marketo Ihre gesamte Datenbank mit Salesforce synchronisiert? Es synchronisiert, wartet dann 5 Minuten und synchronisiert dann den ganzen Tag, jeden Tag. Hier sind einige Details darüber, wie Marketo Salesforce-Kontakte spezifisch behandelt.

## Sync Direction {#sync-direction}

Die Kontaktsynchronisierung erfolgt in beide Richtungen. Wenn Sie Änderungen an einem Kontakt in Salesforce oder Marketo vornehmen, werden Ihre Updates in beiden Systemen angezeigt.

## Was ist, wenn beide Systeme gleichzeitig geändert werden? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Wir sind nett und lassen Salesforce gewinnen. Es ist selten, dass diese Art von Datenkollision auftritt.

## Kann ich eine Person in einen Kontakt in Marketo umwandeln? {#can-i-convert-a-person-into-a-contact-in-marketo}

Ja, verwenden Sie die Aktion &quot;* [Person konvertieren](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md)**&quot;.

>[!CAUTION]
>
>Die Umwandlung einer Person in Marketo wird zu einem neuen Konto und Chancen in Salesforce führen. Wenn Sie keine Duplikat-Konten wünschen, verwenden Sie Salesforce zur Konvertierung.

## Kann ich eine Synchronisierung eines Kontakts manuell erzwingen? {#can-i-manually-force-a-sync-of-a-contact}

Ja, verwenden Sie die Aktion ** [Synchronisierte Person mit SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) **Textfluss und sie wird in Echtzeit synchronisiert.

## Synchronisiert jedes einzelne Standardfeld mit Marketo? {#does-every-single-standard-field-sync-to-marketo}

Nein, nicht alle Standardfelder sind nützlich. Alle benutzerdefinierten Felder können Teil der Synchronisierung sein.

>[!NOTE]
>
>Marketo synchronisiert nur die Felder, auf die Ihr Marketo Sync-Benutzer Zugriff hat.

## Wird Marketo die Salesforce-Validierungsregeln einhalten? {#will-marketo-respect-the-salesforce-validation-rules}

Ja, wenn ein Konflikt vorliegt, wird das Ergebnis im Protokoll der Interessenten-Aktivität protokolliert.
