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

Marketo Engage kann einen E-Mail-Warnhinweis mit Personeninformationen an jede Person senden - den Vertriebsmitarbeiter, einen Partner oder eine andere Person. Verwenden Sie den Flussschritt &quot;[!UICONTROL Warnhinweis senden]&quot;.

![](assets/send-alert-1.png)

1. Wählen Sie die zu sendende E-Mail aus.

   ![](assets/send-alert-2.png)

   >[!NOTE]
   >
   >Ihr E-Mail-Warnhinweis muss alle Kopfzeileninformationen enthalten und sich im Status &quot;**[!UICONTROL Genehmigt]**&quot; befinden.

1. Sie können auf das Vorschausymbol klicken, um sicherzustellen, dass Sie die richtige E-Mail ausgewählt haben.

   ![](assets/send-alert-3.png)

   >[!NOTE]
   >
   >Verwenden Sie unbedingt das Token &quot;[!UICONTROL Warnhinweisinformationen senden]&quot; in Ihrer E-Mail.

1. Wählen Sie den Empfänger der Warnung aus. Sie können [!UICONTROL Vertriebsmitarbeiter] oder [!UICONTROL Kontoinhaber] auswählen.

   ![](assets/send-alert-4.png)

1. Fügen Sie optional alle anderen gewünschten E-Mail-Adressen hinzu (durch Kommas oder Semikolons getrennt).

   ![](assets/send-alert-5.png)

   >[!TIP]
   >
   >In Trigger-Kampagnen können Sie Token in **[!UICONTROL zu anderen E-Mails]** wie `{{lead.Territory Owner}}` oder `{{my.Alert Recipient}}` verwenden, solange es sich bei den Werten um gültige E-Mail-Adressen handelt. Token in **[!UICONTROL An andere E-Mails]** funktionieren in einer Batch-Kampagne nicht.

>[!MORELIKETHIS]
>
>[E-Mail erstellen](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md){target="_blank"}
