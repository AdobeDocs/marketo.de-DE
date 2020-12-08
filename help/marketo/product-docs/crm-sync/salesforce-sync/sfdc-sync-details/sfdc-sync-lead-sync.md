---
unique-page-id: 2953455
description: SFDC-Synchronisierung - Lead-Synchronisierung - Marketing-Dokumente - Produktdokumentation
title: SFDC-Synchronisierung - Lead-Synchronisierung
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---


# SFDC-Synchronisierung: Interessentenabgleich {#sfdc-sync-lead-sync}

>[!NOTE]
>
>**FYI**
>
>Marketo standardisiert nun die Sprache für alle Abonnements, sodass Sie möglicherweise Interessenten in Ihrem Abonnement und Personen/Personen in docs.marketo.com sehen können. Diese Begriffe bedeuten dasselbe. Es hat keine Auswirkungen auf die Artikelanweisungen. Es gibt auch noch einige andere Änderungen. [Weitere Informationen](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Wussten Sie, dass Marketo aus Ihrer Salesforce-Datenbank synchronisiert wird? Es synchronisiert, wartet 5 Minuten und synchronisiert dann erneut. Den ganzen Tag, jeden Tag. Hier sind einige Details darüber, wie Marketo Salesforce Leads speziell behandelt.

## Richtung synchronisieren {#sync-direction}

Die Synchronisierung von Interessenten (Person) und Kontakten erfolgt bidirektional. Wenn Sie Änderungen an einem Datensatz in Salesforce oder Marketo vornehmen, werden Ihre Aktualisierungen auf beiden Systemen angezeigt.

## Was ist, wenn beide Systeme gleichzeitig geändert werden? {#what-if-changes-are-made-in-both-systems-at-the-same-time}

Marketo gewinnt. Es ist selten, dass diese Art von Datenkollision auftritt.

## Kann ich mit Marketo einen Lead in Salesforce erstellen? {#can-i-create-a-lead-in-salesforce-using-marketo}

Ja, verwenden Sie die Aktion &quot; [Synchronisierte Person zu SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) -Fluss&quot;. Dadurch wird ein Interessent in Salesforce erstellt, wenn der Interessent nicht vorhanden ist.

## Kann ich manuell eine Synchronisierung einer Person in Marketo zu einem Lead in Salesforce erzwingen? {#can-i-manually-force-a-sync-of-a-person-in-marketo-to-a-lead-in-salesforce}

Ja, verwenden Sie die Aktion &quot; [Synchronisierte Person zu SFDC](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md) -Fluss&quot;und sie wird in Echtzeit synchronisiert.

## Synchronisiert jedes einzelne Standardfeld mit Marketo? {#does-every-single-standard-field-sync-to-marketo}

Nein, nicht alle Standardfelder sind nützlich. Alle benutzerdefinierten Felder können Teil der Synchronisierung sein.

>[!NOTE]
>
>Marketo synchronisiert nur die Felder, auf die Ihr Salesforce-Synchronisierungsbenutzer Zugriff hat.

## Wird Marketo die Salesforce-Validierungsregeln einhalten? {#will-marketo-respect-the-salesforce-validation-rules}

Ja. Die Synchronisierung schlägt fehl, wenn das Datenformat falsch ist oder die erforderlichen Feldinformationen fehlen. Marketo protokolliert das Ergebnis im Protokoll der Interessenten-Aktivität, wenn dies geschieht.
