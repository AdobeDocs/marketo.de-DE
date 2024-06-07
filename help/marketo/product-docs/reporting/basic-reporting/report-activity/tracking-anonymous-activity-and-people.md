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

Erstmaliger Besuch eines Marketo [Landingpage](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) (oder auf einer Seite Ihrer Website, auf der die Variable [Munchkin-Trackingcode](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)), erstellt Marketo eine _anonyme Aktivität_ und verwendet ein Browser-Cookie, um es zu verfolgen. Sobald der Besucher identifiziert wurde, wird er zu einer Person und der mit dem Browser-Cookie verknüpfte Verlauf wird zusammengeführt.

1. Eine anonyme Aktivität wird erstellt, wenn ein Benutzer:

   * Besuchen Sie Ihre Marketo [Landingpage](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) das erste Mal.
   * Besucht eine Seite Ihrer Site, die [Munchkin-Tracking](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
   * Klicks auf die [Als Webseite anzeigen](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) in einer Marketo-E-Mail.

   >[!NOTE]
   >
   >Im Gegensatz zu anderen Links in Marketo-E-Mails wird &quot;Als Webseite anzeigen&quot;nicht als E-Mail-Klick verfolgt.

   Eine anonyme Aktivität wird zu einer neuen oder vorhandenen Person zusammengeführt, wenn jemand:

   * Klicks a [Link in einer Marketo-E-Mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * Ausfüllen eines Marketo [Formular](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md).
   * Verwendet Marketo [REST-API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/leads) oder [Munchkin](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/lead-tracking) API (für Entwickler) zum Verknüpfen einer anonymen Aktivität mit einem bekannten Datensatz.

   Ein Name in der Datenbank kann mit vielen Cookies verknüpft sein, da Benutzer oft verschiedene Geräte und Browser verwenden, um Ihre Site zu besuchen.

   >[!NOTE]
   >
   >Wenn anonyme Datensätze zu einem neuen oder vorhandenen Datensatz zusammengeführt werden, werden benutzerdefinierte Feldwerte **not** Übertragung.

   >[!MORELIKETHIS]
   >
   >[Personen oder anonyme Besucher in Webberichten anzeigen](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
