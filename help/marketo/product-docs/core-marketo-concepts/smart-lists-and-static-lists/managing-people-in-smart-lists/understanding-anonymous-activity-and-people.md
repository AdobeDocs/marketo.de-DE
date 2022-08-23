---
unique-page-id: 1147322
description: Grundlegendes zu anonymen Aktivitäten und Personen - Marketo-Dokumente - Produktdokumentation
title: Grundlegendes zu anonymen Aktivitäten und Personen
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
source-git-commit: cc66f4ff2e3e0e6ddfabab91215e3ad31f3b9226
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# Grundlegendes zu anonymen Aktivitäten und Personen {#understanding-anonymous-activity-and-people}

Wenn ein Besucher zum ersten Mal eine Marketo-Landingpage (oder eine Seite auf Ihrer Website mit der Variablen [Munchkin-Trackingcode](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md), erstellt Marketo eine _anonyme Aktivität_ und verwendet ein Browser-Cookie, um es zu verfolgen. Sobald sie identifiziert wurde, wird sie zu einer Person und der mit ihrem Browser-Cookie verknüpfte Verlauf wird in zusammengeführt.

>[!IMPORTANT]
>
>Beta-Funktion aktivieren **Munchkin V2 Anonyme Wiederholungsaktivität auf Bekanntem** stellt sicher, dass Kampagnen, die von einer anonymen Lead-Promotion ausgelöst werden, immer wiedergegeben werden, nachdem der anonyme Lead erfolgreich mit dem bekannten Datensatz zusammengeführt wurde. Daher werden benutzerdefinierte Felder, die in wiedergegebenen Kampagnen durch die Schritte Datenwert ändern geändert wurden, im bekannten Datensatz beibehalten.

**Anonym** -Aktivität erstellt, wenn jemand:

* Besucht Ihre Marketo-Landingpage zum ersten Mal.
* Besucht eine Seite Ihrer Site, die [Munchkin-Tracking](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
* Klicks auf die [Als Webseite anzeigen](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) in einer Marketo-E-Mail.

>[!NOTE]
>
>Im Gegensatz zu anderen Links in Marketo-E-Mails [Als Webseite anzeigen](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) wird nicht als E-Mail-Klick verfolgt.

Eine anonyme Aktivität wird zu einer neuen oder vorhandenen Person zusammengeführt, wenn eine Person:

* Klicks a [Link in einer Marketo-E-Mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).
* Ausfüllen eines Marketo [Formular](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md).
* Verwendet Marketo [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md) oder [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) API (für Entwickler) zum Verknüpfen einer anonymen Person mit einem bekannten Datensatz.

Ein Name in der Datenbank kann mit vielen Cookies verknüpft sein, da Benutzer oft verschiedene Geräte und Browser verwenden, um Ihre Site zu besuchen.

>[!NOTE]
>
>Wenn anonyme Datensätze zu einem neuen oder vorhandenen Personendatensatz zusammengeführt werden, werden benutzerdefinierte Feldwerte **not** Übertragung.
