---
unique-page-id: 2360181
description: Erfahren Sie mehr über das Tracking anonymer Aktivitäten und Personen in Marketo Engage, einschließlich des Trackings anonymer Aktivitäten und Kontakte. Verwenden Sie dieses Handbuch, um Ihren nächsten Schritt abzuschließen.
title: Tracking anonymer Aktivitäten und Personen
exl-id: 95a39e57-4636-4bae-8ca8-00cb43cb566c
feature: Reporting
TQID: https://experienceleague.adobe.com/BZakQFVtQystRyrlzo81s-p8N65LXHUJ2ZoSAzeTG6Q
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 255
ht-degree: 8%

---

# Tracking anonymer Aktivitäten und Personen {#tracking-anonymous-activity-and-people}

Wenn jemand zum ersten Mal eine Marketo [Landingpage](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) (oder eine Seite Ihrer Website mit dem [Munchkin-Trackingcode](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)) besucht, erstellt Marketo eine _anonyme Aktivität_ und verwendet ein Browser-Cookie, um diese zu verfolgen. Sobald der Besucher identifiziert ist, wird er zu einer Person und der mit dem Browser-Cookie verknüpfte Verlauf wird zusammengeführt.

1. Eine anonyme Aktivität wird erstellt, wenn jemand:

   * Besucht Ihre Marketo [Landingpage](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) beim ersten Mal.
   * Besucht eine Seite auf Ihrer Site, die über [Munchkin-Tracking](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) verfügt.
   * Klickt auf den [Als Webseite anzeigen](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)-Link in einer Marketo-E-Mail.

   >[!NOTE]
   >
   >Im Gegensatz zu anderen Links in Marketo-E-Mails wird „Als Web-Seite anzeigen“ nicht als E-Mail-Klick verfolgt.

   Eine anonyme Aktivität wird zu einer neuen oder vorhandenen Person zusammengeführt, wenn jemand:

   * Klickt auf einen [Link in einer Marketo-E-Mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * Füllen Sie ein Marketo-[&#x200B; aus](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md).
   * Verwendet die Marketo [REST-API](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/leads) oder die [Munchkin](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/leadtracking/lead-tracking)-API (für Entwickler), um eine anonyme Aktivität mit einem bekannten Datensatz zu verknüpfen.

   Ein Name in der Datenbank kann mit vielen Cookies verknüpft sein, da Benutzer häufig verschiedene Geräte und Browser verwenden, um Ihre Site zu besuchen.

   >[!NOTE]
   >
   >Wenn anonyme Datensätze in einen neuen oder vorhandenen Personendatensatz zusammengeführt werden, werden benutzerdefinierte Feldwerte **nicht** übertragen.

   >[!MORELIKETHIS]
   >
   >[Personen oder anonyme Besucher in Web-Berichten anzeigen](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
