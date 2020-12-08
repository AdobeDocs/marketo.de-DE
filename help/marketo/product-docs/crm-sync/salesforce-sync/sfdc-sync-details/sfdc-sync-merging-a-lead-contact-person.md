---
unique-page-id: 7515133
description: SFDC-Synchronisierung - Zusammenführen eines Interessenten/Kontakts/einer Person - Marketing Docs - Produktdokumentation
title: SFDC-Synchronisierung - Zusammenführen eines Interessenten/Kontakts/einer Person
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---


# SFDC-Synchronisierung: Zusammenführen eines Interessenten/Kontakts/einer Person {#sfdc-sync-merging-a-lead-contact-person}

>[!NOTE]
>
>**FYI**
>
>Marketo standardisiert nun die Sprache für alle Abonnements, sodass Sie möglicherweise Interessenten in Ihrem Abonnement und Personen/Personen in docs.marketo.com sehen können. Diese Begriffe bedeuten dasselbe. Es hat keine Auswirkungen auf die Artikelanweisungen. Es gibt auch noch einige andere Änderungen. [Weitere Informationen](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology).

Manchmal ist es am besten, nur die Regeln Liste. Gehen wir weiter:

* Wenn Sie zwei Interessenten in **Salesforce** zusammenführen, teilt die normale Synchronisierung Marketo mit und die Interessenten werden automatisch als Personen in Marketo zusammengeführt.
* Die Zusammenführung von zwei Personen in **Marketo** führt in der Tat zum selben Prozess wie die Zusammenführung als Interessenten in Salesforce. Es funktioniert immer noch automatisch.
* Das Zusammenführen eines **Interessenten (einer Person) zu einem Kontakt** funktioniert auf dieselbe Weise. Am Ende haben Sie einen einzigen Kontakt auf beiden Seiten.
* Beim Zusammenführen wird der Standardwert summiert.

>[!NOTE]
>
>**Beispiel**
>
>Die Zusammenführung von 3 Interessenten (Personen) mit 10 Punkten pro, ergibt ein Ergebnis von 1 Interessent (Person) mit einem Ergebnis von 30.

* Konfliktende Feldwerte werden aus dem Gewinn-Datensatz genommen. (Datensatz = resultierender Interessent oder Kontakt)
* Wenn der &quot;verlorene Rekord&quot;(der verschwindet) einen Wert hatte und der Gewinn keinen hat, werden wir den verlorenen Rekord behalten. Mit anderen Worten: &quot;Ein Wert ist besser als kein Wert.&quot;
* Alle Protokollelemente der Aktivität werden zusammengeführt.

>[!NOTE]
>
>**Tieftauchen**
>
>Tief tauchen für weitere Informationen über die [Zusammenführung von Menschen in Marketo](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md).

