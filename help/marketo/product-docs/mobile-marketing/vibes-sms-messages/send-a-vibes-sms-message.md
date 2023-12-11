---
description: Senden einer Video-SMS-Nachricht - Marketo-Dokumente - Produktdokumentation
title: Senden einer Video-SMS-Nachricht
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: d4bd94b22b4f9da993150a94d2757014cbf87d80
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---

# Senden einer Video-SMS-Nachricht {#send-a-vibes-sms-message}

Du hast [eine Vibes-SMS-Nachricht erstellt haben](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md), jetzt ist es Zeit, es zu senden. Sie können sie über Batch oder Trigger Campaign versenden.

>[!NOTE]
>
>Beim Senden von SMS-Nachrichten:
>
>* Marketo Engage dedupliziert nach Telefonnummer. Wenn also mehrere Personen über dieselbe Telefonnummer verfügen, erhält nur eine Person die Nachricht, wenn sie nur einer Vibes-Abonnementliste angehört. Die Deduplizierung erfolgt auf der Ebene der Vibes-Abonnement-Liste, nicht auf der Programmebene von Marketo.
>* Marketo sendet keine Nachrichten an Personen, die auf die Blockierungsliste gesetzt oder Marketing ausgesetzt sind.

## Senden einer Batch-SMS {#send-a-batch-sms}

1. Klicken Sie in My Marketo auf **Marketingaktivitäten**.

   ![](assets/send-a-vibes-sms-message-1.png)

1. Wählen Sie die gewünschte Smart-Kampagne aus.

   ![](assets/send-a-vibes-sms-message-2.png)

1. Klicken Sie auf **Smart List** und definieren Sie die Audience für die SMS. In diesem Beispiel senden wir an alle Benutzer in unserer Datenbank, deren Firma &quot;Adobe&quot;ist.

   ![](assets/send-a-vibes-sms-message-3.png)

1. Im **Fluss** Registerkarte, ziehen **SMS-Nachricht senden**. Wählen Sie aus den Dropdown-Listen die gewünschte Liste für SMS-Nachrichten und Besuche aus.

   ![](assets/send-a-vibes-sms-message-4.png)

   >[!NOTE]
   >
   >Der Wähler &quot;Besuchsliste&quot;dient als weiterer Filter für die bereits in der Smart-Liste identifizierte Zielgruppe, sodass nur Personen in die Liste aufgenommen werden, die zu dieser Vibes-Liste gehören.

1. Klicken Sie auf **Zeitplan** und planen Sie Ihre SMS.

   ![](assets/send-a-vibes-sms-message-5.png)

## Trigger-SMS senden {#send-a-trigger-sms}

1. Klicken Sie in My Marketo auf **Marketingaktivitäten**.

   ![](assets/send-a-vibes-sms-message-6.png)

1. Wählen Sie die gewünschte Smart-Kampagne aus.

   ![](assets/send-a-vibes-sms-message-7.png)

1. Klicken Sie auf **Smart List** wählen Sie den gewünschten Trigger aus und legen Sie dessen Wert fest. In diesem Beispiel verwenden wir **Formular ausfüllen**.

   ![](assets/send-a-vibes-sms-message-8.png)

1. Im **Fluss** Registerkarte, ziehen **SMS-Nachricht senden**. Wählen Sie aus den Dropdown-Listen die gewünschte Liste für SMS-Nachrichten und Besuche aus.

   ![](assets/send-a-vibes-sms-message-9.png)

   >[!NOTE]
   >
   >Der Wähler &quot;Besuchsliste&quot;dient als weiterer Filter für die bereits in der Smart-Liste identifizierte Zielgruppe, sodass nur Personen in die Liste aufgenommen werden, die zu dieser Vibes-Liste gehören.

1. Klicken Sie auf **Zeitplan** tab, dann **Aktivieren**.

   ![](assets/send-a-vibes-sms-message-10.png)

>[!MORELIKETHIS]
>
>* [Erstellen einer Vibes-Nachricht](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md)
>* Schritte zum Ablauf von Videos

