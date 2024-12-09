---
unique-page-id: 2360251
description: Bearbeiten der Abmeldemeldung - Marketo Docs - Produktdokumentation
title: Nachricht abmelden bearbeiten
exl-id: 68a3ebc1-b2c9-4e6c-bb13-e5a94c9596d2
feature: Email Setup
source-git-commit: a9f880bd32d533613020d0472c0e1bee07ab388c
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 0%

---

# Nachricht abmelden bearbeiten {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

Wenn Sie Marketing-E-Mails senden (nicht-[operativ](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)), werden der Text und die Links zum Abmelden am unteren Rand angehängt. Sie können die Standardeinstellungen ändern. So geht es.

## Wo kann ich die Bearbeitung vornehmen? {#where-to-make-the-edit}

1. Wechseln Sie zum Abschnitt **[!UICONTROL Admin]** .

   ![](assets/edit-the-unsubscribe-message-1.png)

1. Klicken Sie auf **[!UICONTROL E-Mail]**.

   ![](assets/edit-the-unsubscribe-message-2.png)

   >[!CAUTION]
   >
   >Die folgenden Variablen sind wichtig. Löschen Sie sie nicht!
   >
   >* `%mkt_opt_out_prefix%`
   >* `mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`

1. Bearbeiten Sie die Versionen **[!UICONTROL HTML abmelden]** und **[!UICONTROL Text abmelden]** und klicken Sie auf **[!UICONTROL Änderungen speichern]**.

   ![](assets/edit-the-unsubscribe-message-3.png)

   Da hast du es. _Stellen Sie sicher, dass Sie testen!_ Sie möchten nicht, dass Ihre Marketing-E-Mails die Abmelde-Links beschädigt haben.

>[!TIP]
>
>Sie können die Position der HTML zum Abmelden in Ihrer E-Mail mithilfe von [Token](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md) anpassen.

## Standardtext für Abmeldung {#default-unsubscribe-text}

Wenn Sie jemals zur standardmäßigen Systemabmeldung zurückkehren müssen, kopieren Sie Folgendes:

[!UICONTROL HTML abmelden]:
`<p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p>` [!UICONTROL Text abmelden]:
`%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`

>[!MORELIKETHIS]
>
>[Bearbeiten Sie die Meldung &quot;Als Webseite anzeigen&quot;](/help/marketo/product-docs/administration/email-setup/edit-the-view-as-web-page-message.md)
