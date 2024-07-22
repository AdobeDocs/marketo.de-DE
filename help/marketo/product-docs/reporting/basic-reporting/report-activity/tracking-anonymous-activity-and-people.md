---
unique-page-id: 2360181
description: Tracking von anonymen Aktivitäten und Personen - Marketo-Dokumente - Produktdokumentation
title: Tracking anonymer Aktivitäten und Personen
exl-id: 95a39e57-4636-4bae-8ca8-00cb43cb566c
feature: Reporting
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Tracking anonymer Aktivitäten und Personen {#tracking-anonymous-activity-and-people}

Wenn ein Besucher zum ersten Mal eine Marketo [Landingpage](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) (oder eine Seite auf Ihrer Website mit dem Trackingcode [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)) besucht, erstellt Marketo eine _anonyme Aktivität_ und verwendet ein Browser-Cookie, um sie zu verfolgen. Sobald der Besucher identifiziert wurde, wird er zu einer Person und der mit dem Browser-Cookie verknüpfte Verlauf wird zusammengeführt.

1. Eine anonyme Aktivität wird erstellt, wenn ein Benutzer:

   * Besucht Ihre Marketo [Landingpage](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) zum ersten Mal.
   * Besucht eine Seite Ihrer Site mit dem [Munchkin-Tracking](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
   * Klicken Sie auf den Link [Als Webseite anzeigen](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) in einer Marketo-E-Mail.

   >[!NOTE]
   >
   >Im Gegensatz zu anderen Links in Marketo-E-Mails wird &quot;Als Webseite anzeigen&quot;nicht als E-Mail-Klick verfolgt.

   Eine anonyme Aktivität wird zu einer neuen oder vorhandenen Person zusammengeführt, wenn jemand:

   * Klickt auf einen [Link in einer Marketo-E-Mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * Fügt ein Marketo [form](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md) aus.
   * Verwendet die API [REST API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/leads) oder die API [Munchkin](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/lead-tracking) von Marketo (für Entwickler), um eine anonyme Aktivität mit einem bekannten Datensatz zu verknüpfen.

   Ein Name in der Datenbank kann mit vielen Cookies verknüpft sein, da Benutzer oft verschiedene Geräte und Browser verwenden, um Ihre Site zu besuchen.

   >[!NOTE]
   >
   >Wenn anonyme Datensätze zu einem neuen oder vorhandenen Personendatensatz zusammengeführt werden, werden benutzerdefinierte Feldwerte **nicht** übertragen.

   >[!MORELIKETHIS]
   >
   >[Personen oder anonyme Besucher in Webberichten anzeigen](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
