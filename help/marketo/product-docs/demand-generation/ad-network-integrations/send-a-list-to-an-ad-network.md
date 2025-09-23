---
description: Senden einer Liste an ein Werbenetzwerk - Marketo-Dokumente - Produktdokumentation
title: Senden einer Liste an ein Anzeigennetzwerk
exl-id: d5c55df7-53c8-491a-9d79-ecf7c25cee08
feature: Integrations
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 7%

---

# Senden einer Liste an ein Anzeigennetzwerk {#send-a-list-to-an-ad-network}

Erfahren Sie, wie Sie eine statische Liste an [!DNL LinkedIn], [!DNL Facebook] oder Google senden.

## Senden einer Liste {#how-to-send-a-list}

1. Wählen Sie in Marketo Ihre Liste aus, klicken Sie auf die Dropdown **[!UICONTROL Liste Aktionen]** und wählen Sie **[!UICONTROL An Anzeigennetzwerk senden]**.

   ![](assets/send-a-list-to-an-ad-network-1.png)

1. Wählen Sie zwischen [!DNL LinkedIn], [!DNL Facebook] oder Google (die anderen Optionen sind derzeit nicht verfügbar). In diesem Beispiel wählen wir **[!DNL LinkedIn]**. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/send-a-list-to-an-ad-network-2.png)

1. Klicken Sie auf **[!UICONTROL Zielgruppe]** und wählen Sie Ihre gewünschte Zielgruppe aus.

   ![](assets/send-a-list-to-an-ad-network-3.png)

   >[!TIP]
   >
   >Wenn Sie eine Überprüfung vornehmen müssen, können Sie über die Registerkarte Status die Ziel-Audience sehen, mit der eine Liste synchronisiert wird.

1. Wählen Sie den gewünschten [!UICONTROL Push-Typ] aus und klicken Sie auf **[!UICONTROL Aktualisieren]**.

   ![](assets/send-a-list-to-an-ad-network-4.png)

   >[!NOTE]
   >
   >Wenn Sie &quot;[!UICONTROL Fortlaufende Zielgruppensynchronisierung aktivieren] auswählen, hält Marketo die Liste im ausgewählten Werbenetzwerk auf dem neuesten Stand, wenn sich die Liste in Ihrer Marketo-Instanz ändert. Wir fügen sowohl **und** Personen aus der Zielgruppe hinzu, wenn sie der statischen Liste hinzugefügt oder daraus entfernt werden.

1. Und das war&#39;s! Zum Beenden **[!UICONTROL OK]**.

   ![](assets/send-a-list-to-an-ad-network-5.png)

## FAQs {#faq}

**Kann eine einzelne statische Liste mit mehreren Anzeigenzielgruppen synchronisiert werden?**

Nein, eine Liste kann nur mit einer einzigen Zielgruppe synchronisiert werden.

**Wenn ich die kontinuierliche Synchronisierung mit einer bestehenden Anzeigenzielgruppe aktiviere, wird dann die vorhandene Zielgruppe ersetzt?**

Nein, die vorhandene Zielgruppe wird hinzugefügt, nicht ersetzt.
