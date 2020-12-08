---
unique-page-id: 11379045
description: hinzufügen eines Flussschritts für SMS - Marketing Docs - Produktdokumentation
title: hinzufügen eines Flussschritts für SMS
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---


# hinzufügen eines Flussschritts für SMS {#add-a-flow-step-for-sms}

Marketo verfügt über drei Flussschritte, die Sie in Ihren SMS-Smart-Kampagnen verwenden können:

* **SMS-Nachricht** senden - Diese Flussaktion sendet Nachrichten an Personen aus der Marketing-Smart-Liste, die eine benutzerdefinierte Vibes-Abonnement-Liste abonniert haben. Das Abonnement wird nicht initiiert.
* **Abonnieren der Vibes-Liste** - Diese Flussaktion initiiert den SMS-Abonnement-Vorgang über eine benutzerdefinierte Vibes-Akquise-Kampagne. Vibes sendet dann eine Bestätigungsmeldung; der Empfänger muss darauf antworten, um das Abonnement abzuschließen.
* **Abmelden bei der Vibes-Liste** - Bei dieser Flussaktion wird jeder Benutzer von einer vom Benutzer ausgewählten Vibes-Abonnement-Liste abgemeldet.

>[!NOTE]
>
>Beim Senden von SMS-Nachrichten:
>
>* Marketo dedupliziert per Telefonnummer. Wenn also mehrere Personen dieselbe Telefonnummer haben, erhält nur eine Person die Nachricht.
>* Marketo sendet keine Personen, die auf die Blockierungsliste gesetzt oder Marketing ausgesetzt sind.

>



Allgemeine Informationen zum Einrichten von Flussschritten finden Sie unter [Hinzufügen Flussschritt zu einer intelligenten Kampagne](../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md).

Hier sind die Grundlagen für die Verwendung von SMS.

1. Klicken Sie in &quot;Mein Marketing&quot;auf **Marketing-Aktivitäten**.

   ![](assets/image2016-7-28-11-3a41-3a17.png)

1. Finden Sie die intelligente Kampagne, der Sie den SMS-Fluss hinzufügen möchten. Klicken Sie auf die Registerkarte **Fluss** .

   ![](assets/image2016-7-28-11-3a43-3a41.png)

1. Ziehen Sie über den Fluss, z. B. SMS- **Nachricht** senden. Wählen Sie die SMS-Nachricht und die Vibes-Liste aus den Dropdownfeldern aus.

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >Der Vibes-Liste-Selektor dient als weiterer Filter für die bereits in der intelligenten Liste identifizierte Audience, sodass nur die Leads, die zu dieser Vibes-Liste gehören, Zielgruppe werden.
   >
   >
   >Die Liste **zum** Abonnieren von Vibes und zum **Abmelden von Vibes Liste** haben unterschiedliche Anforderungen. Für **Abonnieren** müssen Sie die Vibes-Liste und die Vibes-Akquise-Kampagne auswählen. Für das **Abmelden** ist nur die Vibes-Liste erforderlich.

