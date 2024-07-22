---
unique-page-id: 7514918
description: Grundlegendes zur Abmeldung - Marketo-Dokumente - Produktdokumentation
title: Grundlegendes zur Abmeldung
exl-id: 30866dc0-cdac-4e73-8dbf-d4b509012269
feature: Deliverability
source-git-commit: 4bae0126d6b36720e170bea7b6b973508c855633
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 2%

---

# Grundlegendes zur Abmeldung {#understanding-unsubscribe}

In Marketo gibt es mehrere Arten von integrierten Abmeldungen. Sie werden alle durch Felder im Personen-Objekt repräsentiert, genau wie Vorname.

Alle diese Felder sind in Ihrem Marketo-Abonnement integriert. Sie sind alle boolesch (Kontrollkästchen). Sie können in den Workflow-Schritten Forms oder [Datenwert ändern](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) verwendet werden.

## Abbestellt {#unsubscribed}

Dies wird auf der Standard-Abmeldeseite verwendet. Wenn eine Person dieses Kontrollkästchen aktiviert oder in einer E-Mail auf den Abmelde-Link klickt, erhält sie keine Marketing-E-Mails mehr. Sie erhalten jedoch [operative E-Mails](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

## Marketing eingestellt {#marketing-suspended}

Dieses Feld wird vom Benutzer festgelegt, um Personen bei einer temporären Abmeldung zu melden. Personen können diesen Status nur erreichen, wenn sie manuell geändert oder ein Schritt zum Ändern des Datenwertflusses verwendet wird.

## E-Mail angehalten {#email-suspended}

Dieser Status blockiert Personen 24 Stunden lang, nachdem ein Hardbounce aufgetreten ist, an Mailings. Nach 24 Stunden wird die Person wieder mailbar.

>[!NOTE]
>
>E-Mail ausgesetzt bleibt auch nach Ablauf des 24-Stunden-Zeitraums aktiviert, sodass Sie sich auf Personen beziehen können, die historisch als solche gekennzeichnet wurden. Um festzustellen, ob die Person Mailbar ist, berechnen Sie einfach 24 Stunden nach dem Zeitpunkt der E-Mail-Aussetzung.

## Auf der Sperrliste {#blocklisted}

[Verwenden Sie dies für Personen wie Konkurrenten](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md). Jeder, der **no** -E-Mails erhält - operative, Marketing usw. Sie bekommen nichts!

![](assets/image2015-5-18-12-3a6-3a40.png)
