---
unique-page-id: 1146958
description: Send Alert - Marketo Docs - Produktdokumentation
title: Benachrichtigung senden
exl-id: 2016e2e7-0361-4bb2-8740-819e21fbd15b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 3%

---

# Benachrichtigung senden {#send-alert}

## Übersicht {#overview}

Marketo kann eine E-Mail-Benachrichtigung mit persönlichen Informationen an jeden senden - den Vertriebsmitarbeiter, einen Partner oder eine andere Person. Verwenden Sie den Schritt **Warnung senden**.

![](assets/one-1.png)

## Nutzung {#usage}

1. Suchen und wählen Sie die E-Mail aus, die Sie senden möchten.

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >Ihre E-Mail-Warnung muss alle Kopfzeileninformationen enthalten und sich im Status **Genehmigt** befinden.

1. Sie können auf das Symbol Vorschau klicken, um sicherzustellen, dass Sie die richtige E-Mail ausgewählt haben.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Verwenden Sie unbedingt das Token **Warnhinweisinformationen senden** in Ihrer E-Mail.

1. Wählen Sie den Empfänger alert aus. Sie können zwischen Verkaufseigentümer oder Kontoinhaber wählen.

   ![](assets/four-2.png)

1. Fügen Sie optional alle weiteren gewünschten E-Mail-Adressen hinzu (durch Kommas oder Semikolons getrennt).

   ![](assets/five.png)

   >[!TIP]
   >
   >In Trigger-Kampagnen können Sie Token in **zu anderen E-Mails** wie `{{lead.Territory Owner}}` oder `{{my.Alert Recipient}}` verwenden, solange die Werte gültige E-Mail-Adressen sind. Tokens in **An andere E-Mails** funktionieren in einer Batch-Kampagne nicht.

Das ist&#39;s! Jetzt wissen Sie, wie Sie den Flussschritt **Warnung senden** verwenden.

>[!MORELIKETHIS]
>
>[E-Mail erstellen](/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md)
