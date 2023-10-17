---
unique-page-id: 1146958
description: Warnhinweis senden - Marketo-Dokumente - Produktdokumentation
title: Alarm senden
exl-id: 2016e2e7-0361-4bb2-8740-819e21fbd15b
feature: Smart Campaigns
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 3%

---

# Alarm senden {#send-alert}

## Überblick {#overview}

Marketo kann einen E-Mail-Warnhinweis mit Personeninformationen an jede Person senden - den Vertriebsmitarbeiter, einen Partner oder eine andere Person. Verwenden Sie die[!UICONTROL Warnhinweis senden]&quot;Flussschritt.

![](assets/one-1.png)

## Nutzung {#usage}

1. Wählen Sie die zu sendende E-Mail aus.

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >Ihr E-Mail-Warnhinweis muss alle Kopfzeileninformationen enthalten und sich im **[!UICONTROL Genehmigt]** state.

1. Sie können auf das Vorschausymbol klicken, um sicherzustellen, dass Sie die richtige E-Mail ausgewählt haben.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Verwenden Sie unbedingt die[!UICONTROL Warnhinweisinformationen senden]&quot; Token in Ihrer E-Mail.

1. Wählen Sie den Empfänger der Warnung aus. Sie können [!UICONTROL Sales Owner] oder [!UICONTROL Kontoinhaber].

   ![](assets/four-2.png)

1. Fügen Sie optional alle anderen gewünschten E-Mail-Adressen hinzu (durch Kommas oder Semikolons getrennt).

   ![](assets/five.png)

   >[!TIP]
   >
   >In Trigger-Kampagnen können Sie Token in **[!UICONTROL zu anderen E-Mails]** wie `{{lead.Territory Owner}}` oder `{{my.Alert Recipient}}` solange die Werte gültige E-Mail-Adressen sind. Token in **[!UICONTROL zu anderen E-Mails]** funktioniert nicht in einer Batch-Kampagne.

>[!MORELIKETHIS]
>
>[E-Mail erstellen](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md){target="_blank"}
