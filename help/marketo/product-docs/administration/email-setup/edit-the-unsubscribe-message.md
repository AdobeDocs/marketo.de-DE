---
unique-page-id: 2360251
description: Bearbeiten der Abmeldenachricht - Marketo-Dokumente - Produktdokumentation
title: Bearbeiten der Abmeldenachricht
exl-id: 68a3ebc1-b2c9-4e6c-bb13-e5a94c9596d2
feature: Email Setup
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '139'
ht-degree: 7%

---

# Bearbeiten der Abmeldenachricht {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

Beim Versand von Marketing-E-Mails ([operationell](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)) werden Text und Links zur Abmeldung unten angehängt. Sie können die Standardeinstellungen ändern. Und so geht das.

## Wo die Bearbeitung vorgenommen werden soll {#where-to-make-the-edit}

1. Navigieren Sie zum Abschnitt **[!UICONTROL Admin]**.

   ![](assets/edit-the-unsubscribe-message-1.png)

1. Klicken Sie auf **[!UICONTROL E-Mail]**.

   ![](assets/edit-the-unsubscribe-message-2.png)

   >[!CAUTION]
   >
   >Die folgenden Variablen sind wichtig. Löschen Sie sie nicht!
   >
   >* `%mkt_opt_out_prefix%`
   >* `mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`

1. Bearbeiten Sie die Versionen **[!UICONTROL HTML abmelden]** und **[!UICONTROL Text abmelden]** nach Ihren Wünschen und klicken Sie auf **[!UICONTROL Änderungen speichern]**.

   ![](assets/edit-the-unsubscribe-message-3.png)

   Da haben Sie es. _Stellen Sie sicher, zu testen!_ Sie möchten nicht, dass Ihre Marketing-E-Mails fehlerhafte Abmelde-Links enthalten.

>[!TIP]
>
>Sie können die Abmeldeposition von HTML in Ihrer E-Mail mit „Token[ anpassen](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).

## Standardtext zur Abmeldung {#default-unsubscribe-text}

Wenn Sie jemals zum Standardsystem zurückkehren müssen, um das Abonnement zu kündigen, kopieren Sie Folgendes:

[!UICONTROL HTML abmelden]:
`<p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p>` [!UICONTROL Text zum Abmelden]:
`%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`

>[!MORELIKETHIS]
>
>[Bearbeiten Sie die Nachricht „Als Web-Seite anzeigen“](/help/marketo/product-docs/administration/email-setup/edit-the-view-as-web-page-message.md)
