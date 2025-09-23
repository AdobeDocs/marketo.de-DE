---
unique-page-id: 7515133
description: SFDC-Synchronisierung - Zusammenführen von Leads/Kontakten/Personen - Marketo-Dokumente - Produktdokumentation
title: SFDC-Synchronisierung - Zusammenführen von Leads/Kontakten/Personen
exl-id: 0e755c80-27cd-4ba3-b540-d7918264c5f6
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 3%

---

# SFDC-Synchronisierung: Zusammenführen von Lead/Kontakt/Person {#sfdc-sync-merging-a-lead-contact-person}

Manchmal ist es am besten, nur die Regeln aufzulisten. Los geht&#39;s:

* Wenn Sie zwei Leads in **[!DNL Salesforce]** zusammenführen, teilt die normale Synchronisierung Marketo mit, dass die Leads automatisch als Personen in Marketo zusammengeführt werden.
* Beim Zusammenführen von zwei Personen in **Marketo** wird derselbe Prozess aufgerufen wie beim Zusammenführen als Leads in [!DNL Salesforce]. Es funktioniert weiterhin automatisch.
* Das Zusammenführen **Leads (Personen) in einem Kontakt** funktioniert genauso. Am Ende haben Sie auf beiden Seiten einen einzigen Kontakt.
* Beim Zusammenführen wird die Standardpunktzahl summiert.

>[!NOTE]
>
>Die Zusammenführung von 3 Leads (Personen) mit Werten von jeweils 10 ergibt ein Ergebnis von 1 Lead (Person) mit einem Score von 30.

* Widersprüchliche Feldwerte werden dem „erfolgreichsten Datensatz“ entnommen. (Datensatz = der resultierende Lead oder Kontakt)
* Wenn der „Verlierer-Rekord“ (der, der verschwindet) einen Wert hatte und der Gewinner-Rekord keinen hat, werden wir den Verlierer-Rekord beibehalten. Mit anderen Worten: „Ein Wert ist besser als kein Wert.“
* Alle Aktivitätsprotokollelemente werden zusammengeführt.

>[!NOTE]
>
>Detaillierte Einblicke in weitere Informationen zu [Zusammenführen von Personen in Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target="_blank"}.
