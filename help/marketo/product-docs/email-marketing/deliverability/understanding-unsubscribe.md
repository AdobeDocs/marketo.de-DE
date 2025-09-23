---
unique-page-id: 7514918
description: Grundlagen zur Abmeldung - Marketo-Dokumente - Produktdokumentation
title: Grundlegendes zur Abmeldung
exl-id: 30866dc0-cdac-4e73-8dbf-d4b509012269
feature: Deliverability
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 4%

---

# Grundlegendes zur Abmeldung {#understanding-unsubscribe}

Es gibt mehrere verschiedene Arten von integrierten Abmeldungen in Marketo. Sie werden alle durch Felder auf dem Objekt Person dargestellt, genau wie der Vorname.

Alle diese Felder sind in Ihrem Marketo-Abonnement integriert. Sie sind alle boolesch (Kontrollkästchen). Sie können in Forms- oder [Datenwert ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)-Flussschritten verwendet werden.

## Abbestellt {#unsubscribed}

Dies wird auf der standardmäßigen Abmeldeseite verwendet. Wenn eine Person dieses Kontrollkästchen aktiviert oder in einer E-Mail auf den Abmelde-Link klickt, erhält sie keine Marketing-E-Mails mehr. Sie erhalten jedoch [operative E-Mails](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

## Marketing eingestellt {#marketing-suspended}

Dieses Feld wird vom Benutzer festgelegt, um Personen in ein temporäres Abo zu stellen. Personen können diesen Status nur erreichen, wenn sie manuell geändert werden oder ein Schritt zum Ändern des Datenwerts verwendet wird.

## E-Mail angehalten {#email-suspended}

Dieser Status blockiert eine Person für 24 Stunden nach einem Hardbounce am Versenden von E-Mails. Nach 24 Stunden wird die Person wieder versandfähig.

>[!NOTE]
>
>Ausgesetzte E-Mails bleiben auch nach Ablauf des 24-Stunden-Zeitraums aktiviert, sodass Sie sich auf Personen beziehen können, die zuvor als solche gekennzeichnet wurden. Um festzustellen, ob die Person per E-Mail erreichbar ist, berechnen Sie einfach 24 Stunden nach dem Zeitpunkt der E-Mail-Aussetzung.

## Auf der Sperrliste {#blocklisted}

[Nutzen Sie dies für Leute wie Konkurrenten](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md). Jeder, den Sie **keine** E-Mails erhalten möchten - betrieblich, Marketing usw. Sie bekommen nichts!

![](assets/image2015-5-18-12-3a6-3a40.png)
