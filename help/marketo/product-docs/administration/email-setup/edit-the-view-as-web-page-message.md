---
unique-page-id: 2360253
description: Bearbeiten Sie die Meldung "Ansicht als Webseite"- Marketing Docs - Produktdokumentation
title: Die Meldung "Ansicht als Webseite"bearbeiten
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---


# Bearbeiten Sie die Meldung &quot;Ansicht als Webseite&quot; {#edit-the-view-as-web-page-message}

Wenn Sie den Text &quot; [Ansicht als Webseite](../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)&quot;bearbeiten müssen, hier sehen Sie wie.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

## Bearbeiten Sie die Meldung &quot;Ansicht als Webseite&quot; {#edit-the-view-as-web-page-message-1}

1. Klicken Sie unter **Admin** auf **E-Mail**.

   ![](assets/image2014-9-18-17-3a13-3a2.png)

   >[!CAUTION]
   >
   >Die folgenden Variablen sind von entscheidender Bedeutung. Löschen Sie sie nicht!
   >
   >    
   >    
   >    * %mkt_webview_url%?mkt_tok=##MKT_TOK#
   >    
   >    
   >Der zweite Teil ##MKT_TOK# ist das munchkin-Cookie dieser Person. Dadurch wird sichergestellt, dass sie beim Klicken auf den Link entsprechend gekocht werden.

1. Bearbeiten Sie die Ansicht **als Webseiten-HTML** und **Ansicht als Webseiten-Text **Versionen nach Ihren Wünschen und klicken Sie auf **Änderungen speichern**.

   ![](assets/image2016-8-26-14-3a40-3a29.png)

>[!CAUTION]
>
>Vermeiden Sie Folgendes:
>
>* Hinzufügen zusätzlicher URLs zu einem der HTML-Felder
>* HTML in der Textversion bereitstellen

>



Da hast du es. Senden Sie Test-E-Mails, um die Formatierung sicherzustellen.

## Standardtext &quot;Ansicht als Webseite&quot; {#default-view-as-web-page-text}

Wenn Sie jemals zum Standardsystem &quot;Ansicht als Webseite&quot;zurückkehren müssen, kopieren Sie Folgendes:

**Ansicht als Webseiten-HTML:**
`<pre data-theme="Confluence"><div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div></pre>` **Ansicht als Webseiten-Text:**

Um diese E-Mail als Webseite Ansicht, gehen Sie zur folgenden Adresse:
`<pre data-theme="Confluence">%mkt_webview_url%?mkt_tok=##MKT_TOK##</pre>` Boom! Du bist fertig.
