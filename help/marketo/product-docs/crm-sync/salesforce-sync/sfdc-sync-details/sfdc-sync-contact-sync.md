---
unique-page-id: 2953457
description: SFDC-Synchronisierung - Kontaktsynchronisierung - Marketo-Dokumente - Produktdokumentation
title: SFDC-Synchronisierung - Kontaktsynchronisierung
exl-id: 537bbc95-9233-4454-892e-81f962cf729d
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 1%

---

# SFDC-Synchronisierung: Kontaktsynchronisierung {#sfdc-sync-contact-sync}

Wussten Sie, dass Marketo Ihre gesamte Datenbank mit [!DNL Salesforce] synchronisiert? Er synchronisiert, wartet dann 5 Minuten und synchronisiert dann erneut, den ganzen Tag, jeden Tag. Im Folgenden finden Sie einige Details dazu, wie Marketo [!DNL Salesforce] Kontakte spezifisch behandelt.

## Synchronisationsrichtung {#sync-direction}

Die Kontaktsynchronisation erfolgt bidirektional. Wenn Sie Änderungen an einem Kontakt in [!DNL Salesforce] oder Marketo vornehmen, werden Ihre Aktualisierungen auf beiden Systemen angezeigt.

## Was passiert, wenn Änderungen in beiden Systemen gleichzeitig vorgenommen werden? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Wir sind nett und lassen [!DNL Salesforce] gewinnen. Es kommt selten vor, dass diese Art von Datenkollision auftritt.

## Kann ich eine Person in Marketo in einen Kontakt konvertieren? {#can-i-convert-a-person-into-a-contact-in-marketo}

Ja, die Flussaktion **[Person konvertieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/convert-person.md){target="_blank"}** verwenden.

>[!CAUTION]
>
>Die Konvertierung einer Person in Marketo führt zu einem neuen Konto und einer neuen Opportunity in [!DNL Salesforce]. Wenn doppelte Konten nicht gewünscht werden, konvertieren Sie mithilfe von [!DNL Salesforce].

## Kann ich die Synchronisierung eines Kontakts manuell erzwingen? {#can-i-manually-force-a-sync-of-a-contact}

Ja, die Flussaktion **[Person mit SFDC synchronisieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"}** wird in Echtzeit synchronisiert.

## Wird jedes Standardfeld mit Marketo synchronisiert? {#does-every-single-standard-field-sync-to-marketo}

Nein, nicht alle Standardfelder sind nützlich. Alle benutzerdefinierten Felder können Teil der Synchronisierung sein.

>[!NOTE]
>
>Marketo synchronisiert nur die Felder, auf die Ihr Marketo-Synchronisierungsbenutzer Zugriff hat.

## Wird Marketo die [!DNL Salesforce] Validierungsregeln einhalten? {#will-marketo-respect-the-salesforce-validation-rules}

Ja, wenn ein Konflikt auftritt, wird das Ergebnis im Aktivitätsprotokoll des Leads protokolliert.
