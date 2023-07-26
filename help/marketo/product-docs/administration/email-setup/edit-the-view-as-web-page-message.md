---
unique-page-id: 2360253
description: Bearbeiten Sie die Meldung "Als Webseite anzeigen"- Marketo Docs - Produktdokumentation
title: Bearbeiten Sie die Meldung "Als Webseite anzeigen"
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 8%

---

# Bearbeiten Sie die Meldung &quot;Als Webseite anzeigen&quot; {#edit-the-view-as-web-page-message}

Wenn Sie die[Als Webseite anzeigen](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)&quot; Text, so ist es.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

## Bearbeiten Sie die Meldung &quot;Als Webseite anzeigen&quot; {#edit-the-view-as-web-page-message-1}

1. Navigieren Sie zum **[!UICONTROL Admin]**-Bereich.

   ![](assets/edit-the-view-as-web-page-message-1.png)

1. Klicks **[!UICONTROL Email]**.

   ![](assets/edit-the-view-as-web-page-message-2.png)

   >[!CAUTION]
   >
   >Die folgenden Variablen sind wichtig. Löschen Sie sie nicht!
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >Der zweite Teil `##MKT_TOK##` ist die [!UICONTROL Munchkin] Cookie dieser Person. Dadurch wird sichergestellt, dass die Cookies beim Klicken auf den Link entsprechend Cookies erhalten.

1. Bearbeiten Sie die **[!UICONTROL Als Webseiten-HTML anzeigen]** und **[!UICONTROL Als Webseiten-Text anzeigen]** Versionen nach Ihren Wünschen und klicken Sie auf **[!UICONTROL Änderungen speichern]**.

   ![](assets/edit-the-view-as-web-page-message-3.png)

>[!CAUTION]
>
>Vermeiden Sie Folgendes:
>
>* Hinzufügen zusätzlicher URLs zu einem der HTML-Felder
>* HTML in Textversion platzieren

Da hast du es. Senden Sie Test-E-Mails, um die Formatierung sicherzustellen.

## Standardtext &quot;Als Webseite anzeigen&quot; {#default-view-as-web-page-text}

Wenn Sie jemals zum Standardsystem zurückkehren müssen[!UICONTROL Als Webseite anzeigen]&quot;, kopieren/fügen Sie Folgendes ein:

**[!UICONTROL Als Webseiten-HTML anzeigen]**:

`<pre data-theme="Confluence"><div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div></pre>`

**[!UICONTROL Als Webseitentext anzeigen]**:

Um diese E-Mail als Webseite anzuzeigen, gehen Sie zur folgenden Adresse:
`<pre data-theme="Confluence">%mkt_webview_url%?mkt_tok=##MKT_TOK##</pre>`

Das ist es!
