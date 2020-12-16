---
unique-page-id: 1147322
description: Verstehen der anonymen Aktivität und der Menschen - Marketing-Dokumente - Produktdokumentation
title: Verstehen der anonymen Aktivität und der Personen
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# Verstehen der anonymen Aktivität und der Personen {#understanding-anonymous-activity-and-people}

Wenn jemand zum ersten Mal einen Marketo [l `anding page`](http://docs.marketo.com/display/DOCS/Personalizing+Landing+Pages) (oder eine Seite auf Ihrer Website, die den [Munchkin-Rückverfolgungscode](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)enthält) besucht, erstellt Marketo eine *anonyme **Aktivität* und verwendet ein Browsercookie, um sie zu verfolgen. Sobald es identifiziert wurde, wird es zu einer Person und der mit ihrem Browser-Cookie verknüpfte Verlauf wird zusammengeführt.

**Eine anonyme** Aktivität wird erstellt, wenn jemand:

* Besucht zum ersten Mal Ihre Marketing-Landingpage.

* Besucht eine Seite auf Ihrer Site mit [Munchkin-Verfolgung](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).

* Klicken Sie auf die [Ansicht als Webseiten](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) -Link in einer Marketing-E-Mail.

>[!NOTE]
>
>Im Gegensatz zu anderen Links in Marketing-E-Mails wird die [Ansicht als Webseite](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) nicht als E-Mail-Klick verfolgt.

Eine anonyme Aktivität wird zu einer neuen oder vorhandenen Person zusammengeführt, wenn eine Person:

* Klicken Sie auf einen [Link in einer Marketing-E-Mail](../../../../product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).
* Fügt ein Marketo- [Formular](../../../../product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md)aus.
* Verwendet Marketos [SOAP](http://docs.marketo.com/pages/viewpage.action?pageid=7509846) - oder [Munchkin](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) -API (für Entwickler), um eine anonyme Person mit einem bekannten Datensatz zu verknüpfen.

Ein Name in der Datenbank kann mit vielen Cookies verknüpft sein, da Benutzer Ihre Site oft mit verschiedenen Geräten und Browsern besuchen.

>[!NOTE]
>
>Wenn anonyme Datensätze in einen neuen oder vorhandenen Personensatz zusammengeführt werden, werden benutzerdefinierte Feldwerte **nicht** übertragen.

