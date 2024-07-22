---
unique-page-id: 7515133
description: SFDC-Synchronisierung - Zusammenführen von Lead/Kontakt/Person - Marketo-Dokumente - Produktdokumentation
title: SFDC-Synchronisation - Zusammenführen von Lead/Kontakt/Person
exl-id: 0e755c80-27cd-4ba3-b540-d7918264c5f6
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---

# SFDC-Synchronisation: Zusammenführen von Lead/Kontakt/Person {#sfdc-sync-merging-a-lead-contact-person}

Manchmal ist es am besten, nur die Regeln aufzulisten. Gehen wir hier:

* Wenn Sie zwei Leads in **Salesforce** zusammenführen, teilt die normale Synchronisierung Marketo Engage mit und die Leads werden automatisch als Personen in Marketo zusammengeführt.
* Die Zusammenführung von zwei Personen in **Marketo** führt denselben Prozess auf wie die Zusammenführung als Leads in Salesforce. Es funktioniert weiterhin automatisch.
* Das Zusammenführen eines **Leads (einer Person) mit einem Kontakt** funktioniert auf die gleiche Weise. Am Ende haben Sie einen einzigen Kontakt auf beiden Seiten.
* Beim Zusammenführen wird der Standardwert summiert.

>[!NOTE]
>
>Die Zusammenführung von 3 Leads (Personen) mit einem Wert von jeweils 10 ergibt ein Ergebnis von 1 Lead (Person) mit einem Wert von 30.

* Konfliktfeldwerte werden aus dem &quot;Siegerdatensatz&quot;übernommen. (Datensatz = resultierender Lead oder Kontakt)
* Wenn der &quot;verlorene Datensatz&quot;(der verschwindet) einen Wert hat und der Gewinnerrekord keinen hat, behalten wir den verlorenen Rekord. Mit anderen Worten: &quot;Ein Wert ist besser als kein Wert.&quot;
* Alle Aktivitätsprotokollelemente werden zusammengeführt.

>[!NOTE]
>
>Tief tauchen für weitere Informationen zum [Zusammenführen von Personen in Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md){target="_blank"}.
