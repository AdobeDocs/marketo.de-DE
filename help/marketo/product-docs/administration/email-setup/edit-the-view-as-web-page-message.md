---
unique-page-id: 2360253
description: Bearbeiten Sie die Meldung "Als Webseite anzeigen"- Marketo Docs - Produktdokumentation
title: Bearbeiten Sie die Meldung "Als Webseite anzeigen"
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---

# Bearbeiten Sie die Meldung &quot;Als Webseite anzeigen&quot; {#edit-the-view-as-web-page-message}

Wenn Sie den Text &quot;[Als Webseite anzeigen](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)&quot; bearbeiten müssen, sehen Sie wie:

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

## Bearbeiten Sie die Meldung &quot;Als Webseite anzeigen&quot; {#edit-the-view-as-web-page-message-1}

1. Wechseln Sie zum Bereich **[!UICONTROL Admin]** .

   ![](assets/edit-the-view-as-web-page-message-1.png)

1. Klicken Sie auf **[!UICONTROL E-Mail]**.

   ![](assets/edit-the-view-as-web-page-message-2.png)

   >[!CAUTION]
   >
   >Die folgenden Variablen sind wichtig. Löschen Sie sie nicht!
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >Der zweite Teil `##MKT_TOK##` ist das Cookie [!UICONTROL munchkin] dieser Person. Dadurch wird sichergestellt, dass die Cookies beim Klicken auf den Link entsprechend Cookies erhalten.

1. Bearbeiten Sie die Versionen **[!UICONTROL Als Webseiten-HTML anzeigen]** und **[!UICONTROL Als Webseiten-Text anzeigen]** nach Ihren Vorstellungen und klicken Sie auf **[!UICONTROL Änderungen speichern]**.

   ![](assets/edit-the-view-as-web-page-message-3.png)

>[!CAUTION]
>
>Vermeiden Sie Folgendes:
>
>* Hinzufügen zusätzlicher URLs zu einem der HTML-Felder
>* HTML in Textversion platzieren

Da hast du es. Senden Sie Test-E-Mails, um die Formatierung sicherzustellen.

## Standardtext &quot;Als Webseite anzeigen&quot; {#default-view-as-web-page-text}

Wenn Sie jemals zum Standardsystem &quot;[!UICONTROL Als Webseite anzeigen]&quot;zurückkehren müssen, kopieren/fügen Sie Folgendes ein:

**[!UICONTROL Als HTML der Webseite anzeigen]**:

`<pre data-theme="Confluence"><div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div></pre>`

**[!UICONTROL Als Webseiten-Text anzeigen]**:

Um diese E-Mail als Webseite anzuzeigen, gehen Sie zur folgenden Adresse:
`<pre data-theme="Confluence">%mkt_webview_url%?mkt_tok=##MKT_TOK##</pre>`

Das ist es!
