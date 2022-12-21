---
unique-page-id: 2949891
description: Statische Listen - Marketo-Dokumente - Produktdokumentation
title: Grundlegendes zu statischen Listen
exl-id: c37c1496-cf19-4e44-aaec-77b10669b9bf
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 3%

---

# Grundlegendes zu statischen Listen {#understanding-static-lists}

Statische Listen sind eine der einfachsten und nützlichsten Funktionen von Marketo. Es handelt sich lediglich um eine Liste von Namen aus Ihrer Datenbank. Es gibt viele Gründe, sie zu benutzen.

>[!NOTE]
>
>Eine einzelne Person in der Datenbank kann in vielen verschiedenen statischen Listen enthalten sein.

Der Unterschied zwischen einer statischen und einer intelligenten Liste ist für das Verständnis von entscheidender Bedeutung.

| Typ | Logik |
|---|---|
| Smart List | Basierend auf **definierte Regeln** |
| Statische Liste | Basierend auf **Hinzufügen/Entfernen jeder Person** |

>[!CAUTION]
>
>Einer der häufigsten Fehler besteht darin, zu denken, dass man eine Person aus einer Liste entfernen kann, indem man einfach &quot;die Person löscht&quot;. **Das ist falsch**. Wenn Sie die Person löschen, wird sie aus **die gesamte Datenbank**, nicht nur die Liste.

## Methoden zum Hinzufügen/Entfernen von Personen aus einer Liste {#ways-to-add-remove-people-from-a-list}

1. Schritt zum Fluss intelligenter Kampagnen ([Zu Liste hinzufügen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-to-list.md), [Aus Liste entfernen](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/remove-from-list.md))

1. [Schritt für einen Aktionsfluss](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/run-a-single-flow-step-from-a-smart-list.md)
1. Personen in eine Liste im Baum ziehen
1. [Listenimport](/help/marketo/getting-started/quick-wins/import-a-list-of-people.md)

## Einige Verwendungen einer statischen Liste {#some-uses-of-a-static-list}

* Eine Liste, die für den Empfang einer Marketing-Nachricht vorausgewählt wurde.
* Eine Liste mit &quot;Konkurrenten&quot;, mit der Sie Unheilmittel-Nachrichten versenden.
* Eine temporäre Liste von Personen in einem bestimmten Status, die dann von intelligenten Kampagnen entfernt werden, wenn sie diesen Status verlassen.

Genießen Sie die Kraft der LIST!

>[!MORELIKETHIS]
>
>[Erstellen einer statischen Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md)
