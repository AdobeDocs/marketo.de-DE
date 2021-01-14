---
unique-page-id: 2360251
description: Bearbeiten Sie die Meldung zum Abmelden - Marketing Docs - Produktdokumentation
title: Die Abmeldung bearbeiten
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 0%

---


# Bearbeiten Sie die Meldung zum Abmelden {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

Wenn Sie Marketing-E-Mails senden (nicht-[operativ](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)), werden Text zum Abmelden und Links am unteren Rand angehängt. Sie können die Standardwerte ändern. So geht es.

## Bearbeiten Sie die Meldung zum Abmelden {#edit-the-unsubscribe-message-1}

1. Klicken Sie unter **Admin** auf **E-Mail**.

   ![](assets/image2014-9-18-16-3a52-3a1.png)

   >[!CAUTION]
   >
   >Die folgenden Variablen sind von entscheidender Bedeutung. Löschen Sie sie nicht!
   >
   >* **%mkt_opt_out_prefix%**
   >* **mkt_unsubscribe=1&amp;mkt_tok=##MKT_TOK#**


1. Bearbeiten Sie die Versionen **Abmelden von HTML** und **Abmelden von Text** nach Ihren Vorlieben und klicken Sie auf **Änderungen speichern**.

   ![](assets/image2016-8-26-13-3a40-3a55.png)

   Da hast du es. _Stellen Sie sicher, dass Sie es testen!_ Sie möchten nicht, dass Ihre Marketing-E-Mails beschädigte Links zum Abmelden aufweisen.

>[!TIP]
>
>Sie können die Position des HTML-Abmeldung in Ihrer E-Mail mit [Token](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md) anpassen.

## Standard-Abmeldung von Text {#default-unsubscribe-text}

Wenn Sie jemals zum Standardsystemabonnement zurückkehren müssen, kopieren Sie Folgendes:

HTML abmelden:
`<pre data-theme="Confluence"><p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p></pre>` Abmelden von Text:
`<pre data-theme="Confluence">%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##</pre>`

>[!MORELIKETHIS]
>
>[Die Meldung &quot;Ansicht als Webseite&quot;bearbeiten](/help/marketo/product-docs/administration/email-setup/edit-the-view-as-web-page-message.md)
