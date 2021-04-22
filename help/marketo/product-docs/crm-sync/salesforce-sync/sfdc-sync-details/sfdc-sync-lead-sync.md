---
unique-page-id: 2953455
description: SFDC-Synchronisierung - Lead-Synchronisierung - Marketo Docs - Produktdokumentation
title: SFDC-Synchronisierung - Lead-Synchronisierung
exl-id: cf38e091-7344-4b95-b9e1-77eda751c4a9
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# SFDC-Synchronisierung: Interessentensynchronisierung {#sfdc-sync-lead-sync}

Wussten Sie, dass Marketo-Synchronisierungen aus Ihrer Salesforce-Datenbank stammen? Es synchronisiert, wartet 5 Minuten und synchronisiert dann erneut. Den ganzen Tag, jeden Tag. Hier sind einige Details darüber, wie Marketo Salesforce Leads speziell behandelt.

## Sync Direction {#sync-direction}

Die Synchronisierung von Interessenten (Person) und Kontakten erfolgt bidirektional. Wenn Sie Änderungen an einem Datensatz in Salesforce oder Marketo vornehmen, werden Ihre Aktualisierungen in beiden Systemen übernommen.

## Was ist, wenn beide Systeme gleichzeitig geändert werden? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo gewinnt. Es ist selten, dass diese Art von Datenkollision auftritt.

## Kann ich mit Marketo einen Lead in Salesforce erstellen? {#can-i-create-a-lead-in-salesforce-using-marketo}

Ja, verwenden Sie die Aktion [Person zu SFDC synchronisieren](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md). Dadurch wird ein Interessent in Salesforce erstellt, wenn der Interessent nicht vorhanden ist.

## Kann ich manuell eine Synchronisierung eines Benutzers in Marketo zu einem Interessenten in Salesforce erzwingen? {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

Ja, verwenden Sie die Aktion [Synchronisierte Person mit SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) und sie wird in Echtzeit synchronisiert.

## Synchronisiert jedes einzelne Standardfeld mit Marketo? {#does-every-single-standard-field-sync-to-marketo}

Nein, nicht alle Standardfelder sind nützlich. Alle benutzerdefinierten Felder können Teil der Synchronisierung sein.

>[!NOTE]
>
>Marketo synchronisiert nur die Felder, auf die Ihr Salesforce-Synchronisierungsbenutzer Zugriff hat.

## Wird Marketo die Salesforce-Validierungsregeln einhalten? {#will-marketo-respect-the-salesforce-validation-rules}

Ja. Die Synchronisierung schlägt fehl, wenn das Datenformat falsch ist oder die erforderlichen Feldinformationen fehlen. Marketo protokolliert das Ergebnis im Protokoll der Interessenten-Aktivität, wenn dies der Fall ist.
