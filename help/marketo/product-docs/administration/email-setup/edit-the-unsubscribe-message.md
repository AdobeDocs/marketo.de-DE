---
unique-page-id: 2360251
description: Bearbeiten der Abmeldemeldung - Marketo Docs - Produktdokumentation
title: Bearbeiten der Abmelde-Nachricht
exl-id: 68a3ebc1-b2c9-4e6c-bb13-e5a94c9596d2
source-git-commit: aeaf1f55b81da70ac8415cab265165a3848b5a0e
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---

# Bearbeiten der Abmelde-Nachricht {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

Wenn Sie Marketing-E-Mails (Nicht-Marketing-E-Mails) senden[operation](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)), werden der Text und die Links zum Abmelden am unteren Rand angehängt. Sie können die Standardeinstellungen ändern. So geht es.

## Wo kann ich die Bearbeitung vornehmen? {#where-to-make-the-edit}

1. Navigieren Sie zu **Admin** Abschnitt.

   ![](assets/edit-the-unsubscribe-message-1.png)

1. Klicken **Email**.

   ![](assets/edit-the-unsubscribe-message-2.png)

   >[!CAUTION]
   >
   >Die folgenden Variablen sind wichtig. Löschen Sie sie nicht!
   >
   >* `%mkt_opt_out_prefix%`
   >* `mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`


1. Bearbeiten Sie die **HTML abmelden** und **Text abmelden** Versionen nach Ihren Wünschen und klicken Sie auf **Änderungen speichern**.

   ![](assets/edit-the-unsubscribe-message-3.png)

   Da hast du es. _Testen Sie unbedingt!_ Sie möchten nicht, dass Ihre Marketing-E-Mails fehlerhafte Abmelde-Links aufweisen.

>[!TIP]
>
>Sie können die Position der Abmelde-HTML in Ihrer E-Mail anpassen, indem Sie [Token](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).

## Standardtext für Abmeldung {#default-unsubscribe-text}

Wenn Sie jemals zur standardmäßigen Systemabmeldung zurückkehren müssen, kopieren Sie Folgendes:

HTML abmelden:
`<pre data-theme="Confluence"><p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p></pre>` Text abmelden:
`<pre data-theme="Confluence">%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##</pre>`

>[!MORELIKETHIS]
>
>[Bearbeiten Sie die Meldung &quot;Als Webseite anzeigen&quot;.](/help/marketo/product-docs/administration/email-setup/edit-the-view-as-web-page-message.md)
