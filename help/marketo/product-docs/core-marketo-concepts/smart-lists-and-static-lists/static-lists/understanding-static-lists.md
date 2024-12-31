---
unique-page-id: 2949891
description: Grundlegendes zu statischen Listen - Marketo-Dokumente - Produktdokumentation
title: Verstehen von statischen Listen
exl-id: c37c1496-cf19-4e44-aaec-77b10669b9bf
feature: Static Lists
source-git-commit: 208ba59e3a5cb8e613e887b4c89e51cec4b3f897
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 2%

---

# Verstehen von statischen Listen {#understanding-static-lists}

Statische Listen sind eine der einfachsten und nützlichsten Funktionen von Marketo. Es handelt sich lediglich um eine Liste mit Namen aus Ihrer Datenbank. Sie werden viele Gründe finden, sie zu verwenden.

>[!NOTE]
>
>Eine einzelne Person in der Datenbank kann sich in vielen verschiedenen statischen Listen befinden.

Der Unterschied zwischen einer statischen und einer Smart List ist wichtig.

| Typ | Logik |
|---|---|
| Smart List | Basierend auf **definierten Regeln** |
| Statische Liste | Basierend auf **Hinzufügen/Entfernen jeder Person** |

>[!CAUTION]
>
>Einer der häufigsten Fehler ist der Gedanke, dass man eine Person aus einer Liste entfernen kann, indem man einfach „die Person löscht“. **Das ist falsch**. Wenn Sie die Person löschen, wird sie aus **der gesamten Datenbank** und nicht nur aus der Liste gelöscht.

## Möglichkeiten zum Hinzufügen/Entfernen von Personen aus einer Liste {#ways-to-add-remove-people-from-a-list}

1. Schritt des Flusses in Smart Campaign ([Zu Liste hinzufügen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-to-list.md){target="_blank"}, [Aus Liste entfernen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-list.md){target="_blank"})

1. [Schritt „Einzelner Aktionsfluss“](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/run-a-single-flow-step-from-a-smart-list.md){target="_blank"}
1. Personen in eine Liste im Baum ziehen
1. [Listen-Import](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md){target="_blank"}

## Einige Verwendungen einer statischen Liste {#some-uses-of-a-static-list}

* Eine Liste, die vorausgewählt wurde, um eine Marketing-Nachricht zu erhalten.
* Eine Liste der „Konkurrenten“, die Sie zum Senden bösartiger Nachrichten zur Gegenspionage verwenden.
* Eine temporäre Liste von Personen in einem bestimmten Status, die von Smart-Kampagnen entfernt werden, wenn sie diesen Status verlassen.

Genießen Sie die Kraft der LIST!

>[!MORELIKETHIS]
>
>[Erstellen einer statischen Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md){target="_blank"}
