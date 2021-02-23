---
unique-page-id: 2360181
description: Verfolgung anonymer Aktivitäten und Personen - Marketing Docs - Produktdokumentation
title: Verfolgung anonymer Aktivitäten und Personen
translation-type: tm+mt
source-git-commit: 03ee7b69f691efce12825aa708c81dffa23cecd9
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---


# Verfolgung anonymer Aktivitäten und Personen {#tracking-anonymous-activity-and-people}

Wenn jemand zum ersten Mal eine Marketo [Landingpage](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) (oder eine Seite auf Ihrer Website mit dem [Munchkin-Trackingcode](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)) besucht, erstellt Marketo eine _anonyme Aktivität_ und verwendet zur Verfolgung ein Browsercookie. Sobald der Besucher identifiziert wurde, wird er zu einer Person und der mit dem Browser-Cookie verknüpfte Verlauf wird zusammengeführt.

1. Eine anonyme Aktivität wird erstellt, wenn jemand:

   * Besucht zum ersten Mal Ihre Marke [Landingpage](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md).
   * Besucht eine Seite auf Ihrer Site, die über [Munchkin-Verfolgung](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) verfügt.
   * Klicken Sie auf den Link [Ansicht als Webseite](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) in einer Marketing-E-Mail.

   >[!NOTE]
   >
   >Im Gegensatz zu anderen Links in Marketing-E-Mails wird die Ansicht als Webseite nicht als E-Mail-Klick verfolgt.

   Eine anonyme Aktivität wird zu einer neuen oder vorhandenen Person zusammengeführt, wenn eine Person:

   * Klicken Sie auf einen [Link in einer Marketing-E-Mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * Füllt ein Marketo [form](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md) aus.
   * Verwendet die [REST-API](https://developers.marketo.com/rest-api/lead-database/leads/) oder die [Munchkin](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/)-API (für Entwickler) von Marketo, um eine anonyme Aktivität mit einem bekannten Datensatz zu verknüpfen.

   Ein Name in der Datenbank kann mit vielen Cookies verknüpft sein, da Benutzer Ihre Site oft mit verschiedenen Geräten und Browsern besuchen.

   >[!NOTE]
   >
   >Wenn anonyme Datensätze in einen neuen oder vorhandenen Personensatz zusammengeführt werden, werden benutzerdefinierte Feldwerte **nicht** übertragen.

   >[!MORELIKETHIS]
   >
   >[Personen oder anonyme Besucher in Webberichten anzeigen](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
