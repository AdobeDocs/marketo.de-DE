---
unique-page-id: 1146958
description: Warnhinweis senden - Marketo-Dokumente - Produktdokumentation
title: Alarm senden
exl-id: 2016e2e7-0361-4bb2-8740-819e21fbd15b
feature: Smart Campaigns
source-git-commit: 12f2399859c784095cc2c1df772c66c649106ba3
workflow-type: tm+mt
source-wordcount: '153'
ht-degree: 2%

---

# Alarm senden {#send-alert}

Marketo Engage kann einen E-Mail-Warnhinweis mit Personeninformationen an jeden senden - den Verkaufsinhaber, einen Partner oder eine andere Person. Verwenden Sie den Flussschritt [!UICONTROL Warnhinweis senden].

![](assets/send-alert-1.png)

1. Suchen Sie die E-Mail, die Sie senden möchten, und wählen Sie sie aus.

   ![](assets/send-alert-2.png)

   >[!NOTE]
   >
   >Ihr E-Mail-Warnhinweis muss alle Kopfzeileninformationen enthalten und sich im Status **[!UICONTROL Genehmigt]** befinden.

1. Sie können auf das Vorschausymbol klicken, um sicherzustellen, dass Sie die richtige E-Mail ausgewählt haben.

   ![](assets/send-alert-3.png)

   >[!NOTE]
   >
   >Denken Sie daran, in Ihrer E[!UICONTROL Mail das Token &quot;]Warnhinweisinfo senden“ zu verwenden.

1. Wählen Sie den Warnhinweisempfänger aus. Sie können &quot;[!UICONTROL &quot; ] &quot;[!UICONTROL &quot; ].

   ![](assets/send-alert-4.png)

1. Fügen Sie optional eine beliebige andere E-Mail-Adresse hinzu (durch ein Komma oder ein Semikolon getrennt).

   ![](assets/send-alert-5.png)

   >[!TIP]
   >
   >In Trigger-Kampagnen können Sie Token in &quot;**[!UICONTROL andere E-Mails“]**. B. `{{lead.Territory Owner}}` oder `{{my.Alert Recipient}}` verwenden, solange die Werte gültige E-Mail-Adressen sind. Token in **[!UICONTROL Zu anderen E]** Mails) funktionieren in einer Batch-Kampagne nicht.

>[!MORELIKETHIS]
>
>[E-Mail erstellen](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md){target="_blank"}
