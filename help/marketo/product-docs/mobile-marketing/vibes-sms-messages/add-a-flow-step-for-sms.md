---
unique-page-id: 11379045
description: Flussschritt für SMS hinzufügen - Marketo-Dokumente - Produktdokumentation
title: Flussschritt für SMS hinzufügen
exl-id: 8e96f6ad-43c9-4d64-8cb6-241664956d72
feature: Mobile Marketing
source-git-commit: cd09ad43c08855af63131aa385c4fd406c963926
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Flussschritt für SMS hinzufügen {#add-a-flow-step-for-sms}

Marketo verfügt über drei Flussprotokolle, die Sie in Ihren SMS-Smart-Kampagnen verwenden können:

* **SMS-Nachricht senden** - Diese FlusAktion sendet Nachrichten an Personen aus der Marketo-smartlist, die sich für eine vom Benutzer ausgewählte Vibes-Abonnementliste angemeldet haben. Der Abonnementprozess wird nicht initiiert.
* **Abonnieren der Vibes-Liste** - Mit dieser Flussaktion wird der SMS-Abonnementprozess über eine benutzerdefinierte Vibes Acquisition Campaign gestartet. Vibes sendet dann eine Bestätigungsnachricht. Der Empfänger muss darauf antworten, um den Abonnementprozess abzuschließen.
* **Abmeldung von der Vibes-Liste** - Mit dieser Flussaktion wird die Anmeldung für jede Person von einer vom Benutzer ausgewählten Abonnementliste &quot;Vibes&quot;aufgehoben.

>[!NOTE]
>
>Beim Senden von SMS-Nachrichten:
>
>* Marketo dedupliziert nach Telefonnummer. Wenn also mehrere Personen dieselbe Telefonnummer haben, erhält nur eine Person die Nachricht.
>* Marketo sendet keine Nachrichten an Personen, die auf die Blockierungsliste gesetzt oder Marketing ausgesetzt sind.

Allgemeine Informationen zum Einrichten von Flussschritten finden Sie unter [Hinzufügen eines Flussschritts zu einer Smart-Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md).

Hier finden Sie die Grundlagen zur Verwendung von SMS.

1. Klicken Sie in My Marketo auf **Marketingaktivitäten**.

   ![](assets/add-a-flow-step-for-sms-1.png)

1. Suchen Sie die Smart-Kampagne, der Sie den SMS-Fluss hinzufügen möchten. Klicken Sie auf **Fluss** Registerkarte.

   ![](assets/image2016-7-28-11-3a43-3a41.png)

1. Ziehen Sie beispielsweise über den Fluss **SMS-Nachricht senden**. Wählen Sie aus den Dropdown-Listen die Liste SMS-Nachricht und die Adressen aus.

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >Der Wähler &quot;Besuchsliste&quot;dient als weiterer Filter für die bereits in der Smart-Liste identifizierte Zielgruppe, sodass nur die Leads als Ziel ausgewählt werden, die zu dieser Vibes-Liste gehören.
   >
   >Die **Abonnieren der Vibes-Liste** und **Abmeldung von der Vibes-Liste** -Flüsse haben unterschiedliche Anforderungen. Für **Abonnieren** müssen Sie die Vibes-Liste und die Vibes-Akquise-Kampagne auswählen. Für **Abmelden**, ist nur die Vibes-Liste erforderlich.
