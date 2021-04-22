---
unique-page-id: 1147322
description: Anonyme Aktivität und Personen - Marketo Docs - Produktdokumentation
title: Verstehen der anonymen Aktivität und der Personen
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 0%

---

# Verstehen der anonymen Aktivität und der Personen {#understanding-anonymous-activity-and-people}

Wenn jemand zum ersten Mal eine Marketo-Landingpage besucht (oder eine Seite auf Ihrer Website, die über den [Munchkin-Rückverfolgungscode](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) verfügt), erstellt Marketo eine _anonyme Aktivität_ und verwendet ein Browsercookie, um sie zu verfolgen. Sobald es identifiziert wurde, wird es zu einer Person und der mit ihrem Browser-Cookie verknüpfte Verlauf wird zusammengeführt.

**Eine** Anonymousaktivität wird erstellt, wenn jemand:

* Besucht Ihre Marketo-Landingpage zum ersten Mal.
* Besucht eine Seite auf Ihrer Site, die über [Munchkin-Verfolgung](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) verfügt.
* Klicken Sie in einer Marketo-E-Mail auf den Link [Ansicht als Webseite](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md).

>[!NOTE]
>
>Im Gegensatz zu anderen Links in Marketo-E-Mails wird [Ansicht als Webseite](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) nicht als E-Mail-Klick verfolgt.

Eine anonyme Aktivität wird zu einer neuen oder vorhandenen Person zusammengeführt, wenn eine Person:

* Klicken Sie auf einen [Link in einer Marketo-E-Mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).
* Füllt ein Marketo [Formular](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md) aus.
* Verwendet Marketos API [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md) oder [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) (für Entwickler), um eine anonyme Person mit einem bekannten Datensatz zu verknüpfen.

Ein Name in der Datenbank kann mit vielen Cookies verknüpft sein, da Benutzer Ihre Site oft mit verschiedenen Geräten und Browsern besuchen.

>[!NOTE]
>
>Wenn anonyme Datensätze in einen neuen oder vorhandenen Personensatz zusammengeführt werden, werden benutzerdefinierte Feldwerte **nicht** übertragen.
