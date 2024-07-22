---
description: SMS senden - Marketo Docs - Produktdokumentation
title: SMS-Nachricht senden
feature: Mobile Marketing
exl-id: 2c863ded-f441-4217-9541-6dcc442d9831
source-git-commit: dae00c6877e638ae60305122f3f3e17b3c922e10
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# SMS-Nachricht senden {#send-a-vibes-sms-message}

Sie haben [Ihre SMS-Nachricht erstellt](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}, jetzt ist es an der Zeit, sie zu senden. Sie können sie über Batch oder Trigger Campaign versenden.

>[!NOTE]
>
>Beim Senden von SMS-Nachrichten:
>
>* Marketo Engage dedupliziert nach Telefonnummer. Wenn also mehrere Personen über dieselbe Telefonnummer verfügen, erhält nur eine Person die Nachricht, wenn sie nur einer Vibes-Abonnementliste angehört. Die Deduplizierung erfolgt auf der Ebene der Vibes-Abonnement-Liste, nicht auf der Programmebene von Marketo.
>* Marketo sendet keine Nachrichten an Personen, die auf die Blockierungsliste gesetzt oder Marketing ausgesetzt sind.
>* Eine SMS-Nachricht wird an niemanden gesendet, der sich abgemeldet hat, wenn er nicht in der Liste der mobilen Vibes-Datenbank aufgeführt ist.

## Senden einer Batch-SMS {#send-a-batch-sms}

1. Klicken Sie in My Marketo auf **Marketingaktivitäten**.

   ![](assets/send-an-sms-message-1.png)

1. Wählen Sie die gewünschte Smart-Kampagne aus.

   ![](assets/send-an-sms-message-2.png)

1. Klicken Sie auf die Registerkarte **Smart List** und definieren Sie die Zielgruppe für die SMS. In diesem Beispiel senden wir an alle Benutzer in unserer Datenbank, deren Firma &quot;Adobe&quot;ist.

   ![](assets/send-an-sms-message-3.png)

1. Ziehen Sie auf der Registerkarte **Fluss** den Mauszeiger über **SMS-Nachricht senden**. Wählen Sie aus den Dropdown-Listen die gewünschte Liste für SMS-Nachrichten und Besuche aus.

   ![](assets/send-an-sms-message-4.png)

   >[!NOTE]
   >
   >Der Wähler &quot;Besuchsliste&quot;dient als weiterer Filter für die bereits in der Smart-Liste identifizierte Zielgruppe, sodass nur Personen in die Liste aufgenommen werden, die zu dieser Vibes-Liste gehören.

1. Klicken Sie auf den Tab **Planung** und planen Sie Ihre SMS.

   ![](assets/send-an-sms-message-5.png)

## Trigger-SMS senden {#send-a-trigger-sms}

1. Klicken Sie in My Marketo auf **Marketingaktivitäten**.

   ![](assets/send-an-sms-message-6.png)

1. Wählen Sie die gewünschte Smart-Kampagne aus.

   ![](assets/send-an-sms-message-7.png)

1. Klicken Sie auf die Registerkarte **Smart List** , wählen Sie den gewünschten Trigger aus und definieren Sie dessen Wert. In diesem Beispiel verwenden wir **Formular ausfüllen**.

   ![](assets/send-an-sms-message-8.png)

1. Ziehen Sie auf der Registerkarte **Fluss** den Mauszeiger über **SMS-Nachricht senden**. Wählen Sie aus den Dropdown-Listen die gewünschte Liste für SMS-Nachrichten und Besuche aus.

   ![](assets/send-an-sms-message-9.png)

   >[!NOTE]
   >
   >Der Wähler &quot;Besuchsliste&quot;dient als weiterer Filter für die bereits in der Smart-Liste identifizierte Zielgruppe, sodass nur Personen in die Liste aufgenommen werden, die zu dieser Vibes-Liste gehören.

1. Klicken Sie auf die Registerkarte **Plan** und dann auf **Aktivieren**.

   ![](assets/send-an-sms-message-10.png)

>[!MORELIKETHIS]
>
>* [Erstellen einer Videomeldung](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}
>* [Verwenden von SMS-Optionen in einer Smart-Kampagne](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/using-sms-options-in-a-smart-campaign.md){target="_blank"}
