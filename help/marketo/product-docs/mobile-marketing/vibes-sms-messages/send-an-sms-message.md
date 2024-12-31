---
description: Senden einer SMS-Nachricht - Marketo-Dokumente - Produktdokumentation
title: Senden einer SMS-Nachricht
feature: Mobile Marketing
exl-id: 2c863ded-f441-4217-9541-6dcc442d9831
source-git-commit: dae00c6877e638ae60305122f3f3e17b3c922e10
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Senden einer SMS-Nachricht {#send-a-vibes-sms-message}

Sie haben [Ihre SMS-Nachricht erstellt](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"} jetzt ist es an der Zeit, sie zu senden. Sie können ihn per Batch oder Trigger-Kampagne senden.

>[!NOTE]
>
>Beim Versand von SMS-Nachrichten:
>
>* Marketo Engage-Deduplizierungen nach Telefonnummer. Wenn also mehrere Personen dieselbe Telefonnummer haben, erhält nur eine Person die Nachricht, wenn sie nur Mitglied einer einzigen Vibes-Abonnement-Liste sind. Die Deduplizierung erfolgt auf der Ebene der Vibes-Abonnement-Liste, nicht auf der Ebene des Marketo-Programms.
>* Marketo sendet keine Nachrichten an Personen, die auf die Blockierungsliste setzte oder Marketing ausgesetzt sind.
>* Eine SMS-Nachricht wird an niemanden gesendet, der sich abgemeldet hat, wenn er sich nicht in der Liste der mobilen Vibes-Datenbank befindet.

## Senden einer Batch-SMS {#send-a-batch-sms}

1. Klicken Sie in My Marketo auf **Marketing-Aktivitäten**.

   ![](assets/send-an-sms-message-1.png)

1. Suchen Sie die gewünschte Smart Campaign und wählen Sie sie aus.

   ![](assets/send-an-sms-message-2.png)

1. Klicken Sie auf **Smart-Liste** und definieren Sie die Audience für die SMS. In diesem Beispiel senden wir an alle Personen in unserer Datenbank, die &quot;Adobe&quot; als ihr Unternehmen aufgeführt haben.

   ![](assets/send-an-sms-message-3.png)

1. Ziehen Sie auf der Registerkarte **Fluss** den Mauszeiger über **SMS senden**. Wählen Sie die gewünschte SMS-Nachricht und die gewünschte Vibes-Liste aus den Dropdown-Listen aus.

   ![](assets/send-an-sms-message-4.png)

   >[!NOTE]
   >
   >Der Selektor Vibes-Liste dient als weiterer Filter für die bereits in der Smart-Liste identifizierte Audience, um nur Personen anzusprechen, die zu dieser Vibes-Liste gehören.

1. Klicken Sie auf die **Zeitplan** und planen Sie Ihre SMS.

   ![](assets/send-an-sms-message-5.png)

## Senden einer Trigger-SMS {#send-a-trigger-sms}

1. Klicken Sie in My Marketo auf **Marketing-Aktivitäten**.

   ![](assets/send-an-sms-message-6.png)

1. Suchen Sie die gewünschte Smart Campaign und wählen Sie sie aus.

   ![](assets/send-an-sms-message-7.png)

1. Klicken Sie auf **Registerkarte** Smart-Liste“, wählen Sie den gewünschten Trigger aus und definieren Sie seinen Wert. In diesem Beispiel verwenden wir &quot;**Formular ausfüllen**.

   ![](assets/send-an-sms-message-8.png)

1. Ziehen Sie auf der Registerkarte **Fluss** den Mauszeiger über **SMS senden**. Wählen Sie die gewünschte SMS-Nachricht und die gewünschte Vibes-Liste aus den Dropdown-Listen aus.

   ![](assets/send-an-sms-message-9.png)

   >[!NOTE]
   >
   >Der Selektor Vibes-Liste dient als weiterer Filter für die bereits in der Smart-Liste identifizierte Audience, um nur Personen anzusprechen, die zu dieser Vibes-Liste gehören.

1. Klicken Sie auf die **Zeitplan** und dann auf **Aktivieren**.

   ![](assets/send-an-sms-message-10.png)

>[!MORELIKETHIS]
>
>* [Erstellen einer Vibes-Nachricht](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}
>* [Verwenden von SMS-Optionen in einer intelligenten Kampagne](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/using-sms-options-in-a-smart-campaign.md){target="_blank"}
