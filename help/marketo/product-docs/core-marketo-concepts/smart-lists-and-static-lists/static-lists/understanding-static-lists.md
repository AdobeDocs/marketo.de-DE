---
unique-page-id: 2949891
description: Erfahren Sie mehr über statische Listen in Marketo für feste Personengruppen. Verwenden Sie statische Listen, wenn die Mitgliedschaft manuell verwaltet wird.
title: Grundlegendes zu statischen Listen
exl-id: c37c1496-cf19-4e44-aaec-77b10669b9bf
feature: Static Lists
TQID: https://experienceleague.adobe.com/rRi3-6ZggKswYYLTZjUr5EBDNoMRirDc1KJgHbbDqP4
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: c5f60233-d5ea-4453-a799-0ad258b4d399id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
subfeature_v2: id: ad89fb33-8541-4339-afe7-bb13d1633714
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 222
ht-degree: 5%

---

# Grundlegendes zu statischen Listen {#understanding-static-lists}

Statische Listen sind eine der einfachsten und nützlichsten Funktionen von Marketo. Es handelt sich um eine Liste mit Namen aus Ihrer Datenbank. Sie werden viele Gründe finden, sie zu verwenden.

>[!NOTE]
>
>Eine einzelne Person in der Datenbank kann sich in vielen verschiedenen statischen Listen befinden.

Der Unterschied zwischen einer statischen und einer Smart List ist wichtig.

| Typ | Logik |
|---|---|
| Intelligente Liste | Basierend auf **definierten Regeln** |
| Statische Liste | Basierend auf **Hinzufügen/Entfernen jeder Person** |

>[!CAUTION]
>
>Einer der häufigsten Fehler ist der Gedanke, dass man eine Person aus einer Liste entfernen kann, indem man „die Person löscht“. **Das ist falsch**. Wenn Sie die Person löschen, wird sie aus **der gesamten Datenbank** und nicht nur aus der Liste gelöscht.

## Möglichkeiten zum Hinzufügen oder Entfernen von Personen aus einer Liste {#ways-to-add-remove-people-from-a-list}

1. Schritt des Flusses in Smart Campaign ([Zu Liste hinzufügen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-to-list.md){target="_blank"}, [Aus Liste entfernen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-list.md){target="_blank"})

1. [Schritt des Flusses mit einer Aktion](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/run-a-single-flow-step-from-a-smart-list.md){target="_blank"}
1. Personen in eine Liste im Baum ziehen
1. [Listen-Import](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md){target="_blank"}

## Einige Verwendungen einer statischen Liste {#some-uses-of-a-static-list}

* Eine Liste, die vorausgewählt wurde, um eine Marketing-Nachricht zu erhalten.
* Eine Liste der „Konkurrenten“, die Sie zum Senden bösartiger Nachrichten zur Gegenspionage verwenden.
* Eine temporäre Liste von Personen in einem bestimmten Status, die von Smart-Kampagnen entfernt werden, wenn sie diesen Status verlassen.

>[!MORELIKETHIS]
>
>[Erstellen einer statischen Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md){target="_blank"}
