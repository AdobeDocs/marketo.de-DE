---
unique-page-id: 1147322
description: Informationen zu anonymen Aktivitäten und Personen - Marketo-Dokumente - Produktdokumentation
title: Informationen zu anonymen Aktivitäten und Personen
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
feature: Smart Lists
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---

# Informationen zu anonymen Aktivitäten und Personen {#understanding-anonymous-activity-and-people}

Wenn jemand zum ersten Mal eine Marketo-Landingpage besucht (oder eine Seite Ihrer Website, die den [Munchkin-Trackingcode](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} aufweist), erstellt Marketo eine *anonyme Aktivität* und verwendet ein Browser-Cookie, um diese zu verfolgen. Sobald er identifiziert ist, wird er zu einer Person und der mit ihrem Browser-Cookie verknüpfte Verlauf wird zusammengeführt.

>[!IMPORTANT]
>
>Durch die Aktivierung der anonymen Wiederholungsaktivität von Beta Feature **[!DNL Munchkin]V2 bei Bekanntem** sichergestellt, dass Kampagnen, die durch eine anonyme Lead-Promotion ausgelöst werden, immer wiederholt werden, nachdem der anonyme Lead erfolgreich mit dem bekannten Datensatz zusammengeführt wurde. Daher werden benutzerdefinierte Felder, die durch die Schritte „Datenwert ändern“ in allen wiedergegebenen Kampagnen geändert wurden, im bekannten Datensatz beibehalten.

**Eine anonyme** Aktivität wird erstellt, wenn jemand:

* Besucht Ihre Marketo-Landingpage beim ersten Mal.
* Besucht eine Seite auf Ihrer Site, die über [Munchkin-Tracking](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} verfügt.
* Klickt auf den [Als Webseite anzeigen](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"}-Link in einer Marketo-E-Mail.

>[!NOTE]
>
>Im Gegensatz zu anderen Links in Marketo-E[Mails wird „Als Webseite anzeigen](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"} nicht als E-Mail-Klick verfolgt.

Eine anonyme Aktivität wird zu einer neuen oder vorhandenen Person zusammengeführt, wenn jemand:

* Klickt auf einen [Link in einer Marketo-E-Mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"}.
* Füllen Sie ein Marketo [Formular](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md){target="_blank"} aus.
* Verwendet die Marketo-API [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md){target="_blank"} oder [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} (für Entwickler), um eine anonyme Person mit einem bekannten Datensatz zu verknüpfen.

Ein Name in der Datenbank kann mit vielen Cookies verknüpft sein, da Benutzer häufig verschiedene Geräte und Browser verwenden, um Ihre Site zu besuchen.

>[!NOTE]
>
>Wenn anonyme Datensätze in einen neuen oder vorhandenen Personendatensatz zusammengeführt werden, werden benutzerdefinierte Feldwerte *nicht* übertragen.
