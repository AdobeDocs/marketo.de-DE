---
unique-page-id: 7514918
description: Informationen zum Abmelden - Marketing Docs - Produktdokumentation
title: Abmelden
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# Abmelden {#understanding-unsubscribe}

Es gibt in Marketo tatsächlich mehrere verschiedene Typen von integrierten Abmeldeabonnements. Sie werden alle durch Felder im Personenobjekt dargestellt, genau wie der Vorname.

>[!NOTE]
>
>Marketo ist dabei, Begriffe wie Blacklist und Whitelist in Blockierungsliste und Zulassungsliste in unserem Produkt zu ändern. Während dieser Aktualisierung werden möglicherweise die alten Begriffe in unseren Screenshots zur Benutzeroberfläche und Dokumentation sowie die neuen Begriffe in unserem Dokumentationstext angezeigt. Wir entschuldigen uns für jede Verwirrung.

Alle diese Felder sind in Ihrem Marketo-Abonnement integriert. Sie sind alle booleschen (Kontrollkästchen) Typ. Sie können in Forms oder [Change Data Value](../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) Flow-Schritten verwendet werden.

## Nicht abonniert {#unsubscribed}

Dies wird auf der Standardseite zum Abmelden verwendet. Wenn eine Person dieses Kontrollkästchen aktiviert oder in einer E-Mail auf den Link zum Abmelden klickt, erhalten sie keine Marketing-E-Mails mehr. Sie erhalten jedoch [operative E-Mails](../../../product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md).

## Marketing ausgesetzt {#marketing-suspended}

Dieses Feld wird vom Benutzer für die Platzierung von Personen auf eine temporäre Abmeldung festgelegt. Personen können diesen Status nur dann erreichen, wenn sie manuell geändert werden oder ein Schritt zum Ändern des Datenwertflusses verwendet wird.

## E-Mail ausgesetzt {#email-suspended}

Dieser Status blockiert eine Person 24 Stunden nach dem Auftreten eines Hartabstoßes von Mailings. Nach 24 Stunden wird die Person wieder mailbar.

>[!NOTE]
>
>E-Mail Ausgesetzt bleibt auch nach Ablauf des 24-Stunden-Zeitraums überprüft, sodass Sie auf Personen verweisen können, die historisch als solche gekennzeichnet wurden. Um festzustellen, ob die Person per E-Mail versandbar ist, berechnen Sie einfach 24 Stunden nach dem Zeitpunkt der E-Mail-Aussetzung.

## Auf die Blockierungsliste gesetzt {#blocklisted}

[Benutze das für Leute wie Konkurrent](http://docs.marketo.com/x/uwOQ). Jeder, der **keine** E-Mails empfangen möchte - operativ, Marketing usw. Sie bekommen nichts!

![](assets/image2015-5-18-12-3a6-3a40.png)

