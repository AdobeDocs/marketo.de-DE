---
unique-page-id: 1147322
description: Grundlegendes zu anonymen Aktivitäten und Personen - Marketo-Dokumente - Produktdokumentation
title: Anonyme Aktivitäten und Personen
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
feature: Smart Lists
source-git-commit: 208ba59e3a5cb8e613e887b4c89e51cec4b3f897
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# Anonyme Aktivitäten und Personen {#understanding-anonymous-activity-and-people}

Wenn ein Besucher zum ersten Mal eine Marketo-Landingpage (oder eine Seite auf Ihrer Website mit dem [Munchkin-Trackingcode](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}) besucht, erstellt Marketo eine *anonyme Aktivität* und verwendet ein Browser-Cookie, um sie zu verfolgen. Sobald sie identifiziert wurde, wird sie zu einer Person und der mit ihrem Browser-Cookie verknüpfte Verlauf wird in zusammengeführt.

>[!IMPORTANT]
>
>Durch Aktivierung der Beta-Funktion **Munchkin V2 Anonyme Wiedergabe-Aktivität auf Bekanntem** wird sichergestellt, dass Kampagnen, die durch anonyme Lead-Promotion ausgelöst werden, immer wiedergegeben werden, nachdem der anonyme Lead erfolgreich mit dem bekannten Datensatz zusammengeführt wurde. Daher werden benutzerdefinierte Felder, die in wiedergegebenen Kampagnen durch die Schritte Datenwert ändern geändert wurden, im bekannten Datensatz beibehalten.

**Eine anonyme** -Aktivität wird erstellt, wenn ein Benutzer:

* Besucht Ihre Marketo-Landingpage zum ersten Mal.
* Besucht eine Seite Ihrer Site mit dem [Munchkin-Tracking](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}.
* Klicken Sie auf den Link [Als Webseite anzeigen](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"} in einer Marketo-E-Mail.

>[!NOTE]
>
>Im Gegensatz zu anderen Links in Marketo-E-Mails wird [Als Webseite anzeigen](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"} nicht als E-Mail-Klick verfolgt.

Eine anonyme Aktivität wird zu einer neuen oder vorhandenen Person zusammengeführt, wenn jemand:

* Klickt auf einen [Link in einer Marketo-E-Mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"}.
* Fügt ein Marketo [Form](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md){target="_blank"} aus.
* Verwendet die API [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md){target="_blank"} oder [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} von Marketo (für Entwickler), um eine anonyme Person einem bekannten Datensatz zuzuordnen.

Ein Name in der Datenbank kann mit vielen Cookies verknüpft sein, da Benutzer oft verschiedene Geräte und Browser verwenden, um Ihre Site zu besuchen.

>[!NOTE]
>
>Wenn anonyme Datensätze zu einem neuen oder vorhandenen Personendatensatz zusammengeführt werden, werden benutzerdefinierte Feldwerte *nicht* übertragen.
