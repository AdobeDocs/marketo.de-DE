---
unique-page-id: 2360253
description: Bearbeiten der Nachricht „Als Web-Seite anzeigen“ - Marketo-Dokumente - Produktdokumentation
title: Bearbeiten der Nachricht „Als Web-Seite anzeigen“
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
feature: Email Setup
source-git-commit: 65d607e279fb86b0816ccaec2f4bf3c69e309cb9
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 11%

---

# Bearbeiten der Nachricht „Als Web-Seite anzeigen“ {#edit-the-view-as-web-page-message}

Wenn Sie den Text &quot;[ als Web-Seite anzeigen](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) bearbeiten müssen, sehen Sie folgendes:

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

## Bearbeiten der Nachricht „Als Web-Seite anzeigen“ {#edit-the-view-as-web-page-message-1}

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/edit-the-view-as-web-page-message-1.png)

1. Klicken Sie auf **[!UICONTROL E-Mail]**.

   ![](assets/edit-the-view-as-web-page-message-2.png)

   >[!CAUTION]
   >
   >Die folgenden Variablen sind wichtig. Löschen Sie sie nicht!
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >Der zweite Teil `##MKT_TOK##` ist der [!UICONTROL -]-Keks dieser Person. Dadurch wird sichergestellt, dass sie beim Klicken auf den Link entsprechend gecoacht werden.

1. HTML Bearbeiten Sie die Versionen **[!UICONTROL Als Web-Seite anzeigen]** und **[!UICONTROL Als Web-]** anzeigen nach Ihren Wünschen und klicken Sie auf **[!UICONTROL Änderungen speichern]**.

   ![](assets/edit-the-view-as-web-page-message-3.png)

>[!CAUTION]
>
>Vermeiden Sie Folgendes:
>
>* Hinzufügen zusätzlicher URLs zu einem der HTML-Felder
>* Einbetten von HTML in die Textversion

Da haben Sie es. Senden Sie Test-E-Mails, um die Formatierung sicherzustellen.

## Standardtext „Als Web-Seite anzeigen“ {#default-view-as-web-page-text}

Wenn Sie jemals zum Standardsystem „Als Web-Seite anzeigen[!UICONTROL &#x200B; zurückkehren müssen] kopieren Sie Folgendes:

**[!UICONTROL Als Webseite anzeigen HTML]**:

`<div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div>`

**[!UICONTROL Als Webseitentext anzeigen]**:

Um diese E-Mail als Web-Seite anzuzeigen, gehen Sie zu der folgenden Adresse:
`%mkt_webview_url%?mkt_tok=##MKT_TOK##`

Das war&#39;s!
