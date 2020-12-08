---
unique-page-id: 2360251
description: Bearbeiten Sie die Meldung zum Abmelden - Marketing Docs - Produktdokumentation
title: Die Abmeldung bearbeiten
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 0%

---


# Die Abmeldung bearbeiten {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

Wenn Sie Marketing-E-Mails senden (nicht [funktionsfähig](../../../product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)), werden Text zum Abbestellen des Abonnements und Links am unteren Rand angehängt. Sie können die Standardwerte ändern. So geht es.

## Die Abmeldung bearbeiten {#edit-the-unsubscribe-message-1}

1. Klicken Sie unter **Admin** auf **E-Mail**.

   ![](assets/image2014-9-18-16-3a52-3a1.png)

   >[!CAUTION]
   >
   >
   >Die folgenden Variablen sind von entscheidender Bedeutung. Löschen Sie sie nicht!
   >
   >    
   >    
   >    * **%mkt_opt_out_prefix%**
   >    * **mkt_unsubscribe=1&amp;mkt_tok=##MKT_TOK#**


1. Bearbeiten Sie die **Versionen &quot;HTML** abmelden&quot;und &quot;Text **** abmelden&quot;nach Ihren Vorlieben und klicken Sie auf &quot;Änderungen **speichern&quot;**.

   ![](assets/image2016-8-26-13-3a40-3a55.png)

   Da hast du es. **Stellen Sie sicher, dass Sie es testen!** Sie möchten nicht, dass Ihre Marketing-E-Mails beschädigte Links zum Abmelden aufweisen.

>[!TIP]
>
>Sie können die Position des HTML-Abonnements für die Abmeldung in Ihrer E-Mail mit [Token](../../../product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md)anpassen.

## Standardtext für Abmeldung {#default-unsubscribe-text}

Wenn Sie jemals zum Standardsystemabonnement zurückkehren müssen, kopieren Sie Folgendes:

HTML abmelden:
`<pre data-theme="Confluence"><p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p></pre>` Text abmelden:
`<pre data-theme="Confluence">%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##</pre>`

>[!NOTE]
>
>**Verwandte Artikel**
>
>* [Die Meldung &quot;Ansicht als Webseite&quot;bearbeiten](edit-the-view-as-web-page-message.md)

>



