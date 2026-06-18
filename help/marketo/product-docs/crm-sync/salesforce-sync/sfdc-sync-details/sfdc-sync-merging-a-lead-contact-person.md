---
unique-page-id: 7515133
description: Erfahren Sie, wie das Zusammenführen von Leads, Kontakten und Personen in Salesforce und Marketo funktioniert. Erfahren Sie mehr über Zusammenführungsregeln für Scores, Feldwerte und Aktivitätsprotokolle.
title: SFDC-Synchronisierung - Zusammenführen von Leads/Kontakten/Personen
exl-id: 0e755c80-27cd-4ba3-b540-d7918264c5f6
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/alPa6YMG0tgo08ruZAZlWhujV54iVcUMAAejXJbEQFw
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: 25bbf4409df3db38b849d936e2a90b48f859d089
workflow-type: tm+mt
source-wordcount: 267
ht-degree: 2%

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
* Wenn der „Verlierer-Datensatz“ (der verschwindet) einen Wert hatte und der Gewinner-Datensatz keinen hat (oder null ist), behalten wir den Verlierer-Datensatz bei. Mit anderen Worten: „Ein Wert ist besser als kein Wert.“
* Alle Aktivitätsprotokollelemente werden zusammengeführt.

>[!NOTE]
>
>Das Verhalten von booleschen Feldern bei einer API-Zusammenführung hat sich in der Version vom 26. März geändert. Jetzt wird ein Wert „False“ korrekt als Wert für dieses Feld behandelt. Nur ein Nullwert wird bei der Auswertung widersprüchlicher Felder als „leer“ behandelt. Siehe [diesen Community-Beitrag](https://experienceleaguecommunities.adobe.com/adobe-marketo-engage-27/api-merge-functionality-for-boolean-fields-251219?profile.language=de){target="_blank"} für weitere Details.

>[!MORELIKETHIS]
>
>Detaillierte Einblicke in weitere Informationen zu [Zusammenführen von Personen in Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md).
