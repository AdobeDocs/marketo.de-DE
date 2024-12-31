---
description: Flussschritt für SMS hinzufügen - Marketo-Dokumente - Produktdokumentation
title: Hinzufügen eines Flussschritts für SMS
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: fee2d692acd8d54f2e308e2d5edc9876d13d5a4d
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 3%

---

# Hinzufügen eines Flussschritts für SMS {#add-a-flow-step-for-sms}

Marketo Engage verfügt über drei Flussschritte, die Sie in Ihren SMS Smart-Kampagnen verwenden können:

<table>
<tbody>
  <tr>
    <td style="width:25%">SMS-Nachricht senden</td>
    <td>Diese Flussaktion sendet Nachrichten an Personen aus der Smart-Liste von Marketo, die sich für eine Abonnement-Liste mit angemeldeten Benutzern von Vibes angemeldet haben. Der Anmeldevorgang wird nicht initiiert. <a href="/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-a-vibes-sms-message.md">Weitere Informationen</a>.</td>
  </tr>

<tr>
    <td style="width:25%">Abonnement der Vibes-Liste</td>
    <td>Diese Flussaktion initiiert den SMS-Abonnementprozess über eine vom Benutzer ausgewählte Vibes-Akquise-Kampagne. Vibes sendet dann eine Bestätigungsnachricht, und der Empfänger muss innerhalb von 24 Stunden mit „Y“ antworten, um die Anmeldung zu bestätigen. Nachdem sich der Benutzer angemeldet hat, wird er Mitglied der zugehörigen Vibes-Abonnement-Liste.</td>
  </tr>
  <tr>
    <td style="width:25%">Abbestelltes Abonnement der Vibes-Liste</td>
    <td>Mit dieser Flussaktion wird jede Person von einer Abonnement-Liste für angemeldete Benutzer abgemeldet. Wenn ein(e) Benutzende(r) „STOP“ zu Ihrem Code per SMS sendet, wird sein/ihr Personendatensatz aktualisiert, um anzugeben, dass er/sie nicht mehr zur Vibes-Abonnement-Liste gehört.</td>
  </tr>
  </tbody>
</table>

>[!NOTE]
>
>Beim Versand von SMS-Nachrichten:
>
>* Marketo dedupliziert nach Telefonnummer. Wenn also mehrere Personen dieselbe Telefonnummer haben, erhält nur eine Person die Nachricht, wenn sie nur Mitglied einer einzigen Vibes-Abonnement-Liste sind. Die Deduplizierung erfolgt auf der Ebene der Vibes-Abonnement-Liste, nicht auf der Ebene des Marketo-Programms.
>* Marketo sendet keine Nachrichten an Personen, die auf die Blockierungsliste setzte oder Marketing ausgesetzt sind.

Allgemeine Informationen zum Einrichten von Flussschritten finden Sie unter [Hinzufügen eines Flussschritts zu einer Smart-Kampagne](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/add-a-flow-step-to-a-smart-campaign.md).

Im Folgenden finden Sie die Grundlagen zur Verwendung von SMS.

1. Klicken Sie in My Marketo auf **Marketing-Aktivitäten**.

   ![](assets/add-a-flow-step-for-sms-1.png)

1. Suchen Sie die Smart Campaign, der Sie den SMS-Fluss hinzufügen möchten, und wählen Sie sie aus.

   SCREENSHOT

1. Wählen Sie auf der Registerkarte Smart-Liste die gewünschten Trigger aus (z. B. „Ausgefülltes Formular„).

   SCREENSHOT

1. Ziehen Sie auf **Registerkarte** Fluss“ den Fluss-Schritt (z. B. &quot;**-Nachricht senden**). Wählen Sie die SMS-Nachricht und die Liste Vibes aus den Dropdown-Listen aus.

   ![](assets/send-sms-message-hands.jpg)

   >[!NOTE]
   >
   >Der Selektor Vibes-Liste dient als weiterer Filter für die bereits in der Smart-Liste identifizierte Audience, um nur die Leads anzusprechen, die zu dieser Vibes-Liste gehören.
   >
   >Die **Abonnieren einer Vibes-Liste** und **Abmelden von einer Vibes-Liste** haben unterschiedliche Anforderungen. Für **Abonnieren** müssen Sie die Vibes-Liste und die Vibes-Akquise-Kampagne auswählen. Für **Abmelden** ist nur die Liste Vibes erforderlich.
