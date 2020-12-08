---
unique-page-id: 1147154
description: Synchronisieren einer SFDC-Kampagne mit einem Programm - Marketing Docs - Produktdokumentation
title: Synchronisieren einer SFDC-Kampagne mit einem Programm
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---


# Synchronisieren einer SFDC-Kampagne mit einem Programm {#sync-an-sfdc-campaign-with-a-program}

Marketo ermöglicht Ihnen, Ihre Programme mit Salesforce-Kampagnen zu synchronisieren, um die gleiche Liste von Personen in beiden Systemen, einschließlich ihres Status, zu erhalten. Fangen wir an!

>[!NOTE]
>
>**Voraussetzungen**
>
>Sie müssen zuerst die Salesforce-Kampagne-Synchronisierung [](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/enable-disable-campaign-sync.md) aktivieren.

>[!CAUTION]
>
>Beim Synchronisieren einer SFDC-Kampagne mit einem Marketo-Programm werden die impliziten SFDC-Aktionen (z. B. Hinzufügen zur SFDC-Kampagne, Synchronisierung mit SFDC) für untergeordnete Kampagnen des Programms deaktiviert.

1. Gehen Sie zu **Marketing-Aktivitäten**.

   ![](assets/login-marketing-activities-1.png)

1. Wählen Sie Ihr Programm aus.

   ![](assets/image2015-7-22-8-3a47-3a28.png)

1. Klicken Sie auf **Programm-Aktionen** und wählen Sie dann **Salesforce-Kampagne-Synchronisierung**.

   ![](assets/image2015-7-22-8-3a48-3a5.png)

1. Wählen Sie **Neu erstellen **oder wählen Sie eine bestehende Salesforce-Kampagne.

   >[!TIP]
   >
   >Wenn Sie eine bestehende Salesforce-Kampagne auswählen, stellen Sie sicher, dass Sie [mit dem Programm-Status der Salesforce-Kampagne und des Marketo-Programms](../../../../product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-errors/how-to-match-program-statuses-and-salesforce-campaign-statuses-prior-to-sync.md)übereinstimmen.

1. Geben Sie einen Namen für die neue Kampagne ein und klicken Sie auf **Speichern**.

   ![](assets/image2015-7-22-8-3a57-3a19.png)

1. Jetzt können Sie die Synchronisierungsdaten der Kampagne auf der Seite &quot;Programm-Zusammenfassung&quot;überprüfen.

   ![](assets/image2015-7-22-8-3a59-3a33.png)

   Ausgezeichnet! Jetzt werden alle Statusänderungen des Programms in Marketo mit der SFDC-Kampagne synchronisiert und umgekehrt.

