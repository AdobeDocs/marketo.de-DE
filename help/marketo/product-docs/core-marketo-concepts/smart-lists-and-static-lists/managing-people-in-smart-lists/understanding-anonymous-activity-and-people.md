---
unique-page-id: 1147322
description: Verstehen der anonymen Aktivität und der Menschen - Marketing-Dokumente - Produktdokumentation
title: Verstehen der anonymen Aktivität und der Personen
translation-type: tm+mt
source-git-commit: 07f713ece9832b7696451001f61c6a3b45b4a94a
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 0%

---


# Verstehen der anonymen Aktivität und der Personen {#understanding-anonymous-activity-and-people}

Wenn jemand zum ersten Mal eine Marketing-Landingpage besucht (oder eine Seite auf Ihrer Website, die über den [Munchkin-Rückverfolgungscode](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) verfügt), erstellt Marketo eine _anonyme Aktivität_ und verwendet zur Verfolgung einen Browsercookie. Sobald es identifiziert wurde, wird es zu einer Person und der mit ihrem Browser-Cookie verknüpfte Verlauf wird zusammengeführt.

**Eine** Anonymousaktivität wird erstellt, wenn jemand:

* Besucht zum ersten Mal Ihre Marketing-Landingpage.
* Besucht eine Seite auf Ihrer Site, die über [Munchkin-Verfolgung](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) verfügt.
* Klicken Sie auf den Link [Ansicht als Webseite](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) in einer Marketing-E-Mail.

>[!NOTE]
>
>Im Gegensatz zu anderen Links in Marketing-E-Mails wird [Ansicht als Webseite](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) nicht als E-Mail-Klick verfolgt.

Eine anonyme Aktivität wird zu einer neuen oder vorhandenen Person zusammengeführt, wenn eine Person:

* Klicken Sie auf einen [Link in einer Marketing-E-Mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).
* Füllt ein Marker [Formular](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md) aus.
* Verwendet die API [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md) oder [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) (für Entwickler) von Marketo, um eine anonyme Person mit einem bekannten Datensatz zu verknüpfen.

Ein Name in der Datenbank kann mit vielen Cookies verknüpft sein, da Benutzer Ihre Site oft mit verschiedenen Geräten und Browsern besuchen.

>[!NOTE]
>
>Wenn anonyme Datensätze in einen neuen oder vorhandenen Personensatz zusammengeführt werden, werden benutzerdefinierte Feldwerte **nicht** übertragen.
