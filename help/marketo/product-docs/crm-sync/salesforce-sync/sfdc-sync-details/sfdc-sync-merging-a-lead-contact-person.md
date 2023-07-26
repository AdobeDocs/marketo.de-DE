---
unique-page-id: 7515133
description: SFDC-Synchronisierung - Zusammenführen von Lead/Kontakt/Person - Marketo-Dokumente - Produktdokumentation
title: SFDC-Synchronisation - Zusammenführen von Lead/Kontakt/Person
exl-id: 0e755c80-27cd-4ba3-b540-d7918264c5f6
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 0%

---

# SFDC-Synchronisation: Zusammenführen von Lead/Kontakt/Person {#sfdc-sync-merging-a-lead-contact-person}

Manchmal ist es am besten, nur die Regeln aufzulisten. Gehen wir hier:

* Wenn Sie zwei Leads zusammenführen in **Salesforce**, gibt die normale Synchronisierung an, dass Marketo und die Leads automatisch als Personen in Marketo zusammengeführt werden.
* Zusammenführen von zwei Personen in **Marketo** führt denselben Prozess aus wie das Zusammenführen als Leads in Salesforce. Es funktioniert weiterhin automatisch.
* Zusammenführen einer **Kontakt** funktioniert genauso. Am Ende haben Sie einen einzigen Kontakt auf beiden Seiten.
* Beim Zusammenführen wird der Standardwert summiert.

>[!NOTE]
>
>Die Zusammenführung von 3 Leads (Personen) mit einem Wert von jeweils 10 ergibt ein Ergebnis von 1 Lead (Person) mit einem Wert von 30.

* Konfliktfeldwerte werden aus dem &quot;Siegerdatensatz&quot;übernommen. (Datensatz = resultierender Lead oder Kontakt)
* Wenn der &quot;verlorene Datensatz&quot;(der verschwindet) einen Wert hat und der Gewinnerrekord keinen hat, behalten wir den verlorenen Rekord. Mit anderen Worten: &quot;Ein Wert ist besser als kein Wert.&quot;
* Alle Aktivitätsprotokollelemente werden zusammengeführt.

>[!NOTE]
>
>Weitere Informationen zu [Zusammenführen von Personen in Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md).
