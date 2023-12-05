---
description: Flussschritt für SMS hinzufügen - Marketo-Dokumente - Produktdokumentation
title: Flussschritt für SMS hinzufügen
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: cd09ad43c08855af63131aa385c4fd406c963926
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# Flussschritt für SMS hinzufügen {#add-a-flow-step-for-sms}

Marketo Engage verfügt über drei Flussprotokolle, die Sie in Ihren SMS-Smart-Kampagnen verwenden können:

* **SMS-Nachricht senden** - Diese FlusAktion sendet Nachrichten an Personen aus der Marketo-Smart-Liste, die sich für eine angemeldete Vibes-Abonnementliste eines Benutzers angemeldet haben. Der Abonnementprozess wird nicht initiiert.
* **Abonnieren der Vibes-Liste** - Mit dieser Flussaktion wird der SMS-Abonnementprozess über eine benutzerdefinierte Vibes Acquisition Campaign gestartet. Vibes sendet dann eine Bestätigungsnachricht. Der Empfänger muss &quot;Y&quot;an ihn senden, um die Anmeldung innerhalb von 24 Stunden zu bestätigen. Nachdem sich der Benutzer angemeldet hat, wird er Mitglied Ihrer zugehörigen Vibes-Abonnementliste.
* **Abmeldung von der Vibes-Liste** - Mit dieser Flussaktion wird die Anmeldung jeder Person von einer angemeldeten Benutzer-Abonnementliste für Vibes aufgehoben. Wenn ein Benutzer &quot;stop&quot;in Ihren Code schreibt, wird sein Personendatensatz aktualisiert, um anzuzeigen, dass er nicht mehr Mitglied der Vibes-Abonnementliste ist.

>[!NOTE]
>
>Beim Senden von SMS-Nachrichten:
>
>* Marketo dedupliziert nach Telefonnummer. Wenn also mehrere Personen über dieselbe Telefonnummer verfügen, erhält nur eine Person die Nachricht, wenn sie nur einer Vibes-Abonnementliste angehört. Die Deduplizierung erfolgt auf der Ebene der Vibes-Abonnement-Liste, nicht auf der Programmebene von Marketo.
>* Marketo sendet keine Nachrichten an Personen, die auf die Blockierungsliste gesetzt oder Marketing ausgesetzt sind.

Allgemeine Informationen zum Einrichten von Flussschritten finden Sie unter [Hinzufügen eines Flussschritts zu einer Smart-Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md).

Hier finden Sie die Grundlagen zur Verwendung von SMS.

1. Klicken Sie in My Marketo auf **Marketingaktivitäten**.

   ![](assets/add-a-flow-step-for-sms-1.png)

1. Wählen Sie die Smart-Kampagne aus, der Sie den SMS-Fluss hinzufügen möchten.

   SCREENSHOT

1. Wählen Sie auf der Registerkarte Smart-Liste die gewünschten Trigger aus (z. B. &quot;ausgefülltes Formular&quot;).

   SCREENSHOT

1. Im **Fluss** -Registerkarte über den Schritt &quot;Fluss&quot;ziehen (z. B. **SMS-Nachricht senden**). Wählen Sie aus den Dropdown-Listen die Liste SMS-Nachricht und die Adressen aus.

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >Der Wähler &quot;Besuchsliste&quot;dient als weiterer Filter für die bereits in der Smart-Liste identifizierte Zielgruppe, sodass nur die Leads als Ziel ausgewählt werden, die zu dieser Vibes-Liste gehören.
   >
   >Die **Abonnieren der Vibes-Liste** und **Abmeldung von der Vibes-Liste** -Flüsse haben unterschiedliche Anforderungen. Für **Abonnieren** müssen Sie die Vibes-Liste und die Vibes-Akquise-Kampagne auswählen. Für **Abmelden**, ist nur die Vibes-Liste erforderlich.
