---
description: Senden einer Liste an ein Werbenetzwerk - Marketo Docs - Produktdokumentation
title: Senden einer Liste an ein Werbenetzwerk
exl-id: d5c55df7-53c8-491a-9d79-ecf7c25cee08
feature: Integrations
source-git-commit: bebf61037f37a06b40b4d9c1df872f1cf62a1403
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# Senden einer Liste an ein Werbenetzwerk {#send-a-list-to-an-ad-network}

Erfahren Sie, wie Sie eine statische Liste an LinkedIn, Facebook oder Google senden.

## Senden einer Liste {#how-to-send-a-list}

1. Wählen Sie unter Marketo Engage Ihre Liste aus, klicken Sie auf das Dropdown-Menü **[!UICONTROL Listenaktionen]** und wählen Sie **[!UICONTROL An Werbenetzwerk senden]** aus.

   ![](assets/send-a-list-to-an-ad-network-1.png)

1. Wählen Sie zwischen LinkedIn, Facebook oder Google (die anderen Optionen sind derzeit nicht verfügbar). In diesem Beispiel wählen wir **[!UICONTROL LinkedIn]**. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/send-a-list-to-an-ad-network-2.png)

1. Klicken Sie auf die Dropdownliste **[!UICONTROL Zielgruppe]** und wählen Sie die gewünschte Zielgruppe aus.

   ![](assets/send-a-list-to-an-ad-network-3.png)

   >[!TIP]
   >
   >Wenn Sie jemals eine Prüfung durchführen müssen, können Sie über den Tab Status die Ziel-Audience sehen, mit der eine Liste synchronisiert wird.

1. Wählen Sie den gewünschten Push-Typ aus und klicken Sie auf **[!UICONTROL Aktualisieren]**.

   ![](assets/send-a-list-to-an-ad-network-4.png)

   >[!NOTE]
   >
   >Wenn Sie &quot;Kontinuierliche Zielgruppensynchronisierung aktivieren&quot;auswählen, behält Marketo die Liste im ausgewählten Werbenetzwerk auf dem neuesten Stand, da sich die Liste in Ihrer Marketo-Instanz ändert. Sowohl _als auch_ entfernen Personen aus der Zielgruppe, wenn sie der statischen Liste hinzugefügt/daraus entfernt werden.

1. Und das ist es! Klicken Sie zum Beenden auf **[!UICONTROL OK]** .

   ![](assets/send-a-list-to-an-ad-network-5.png)

## FAQs {#faq}

**Kann eine einzelne statische Liste mit mehreren Anzeigenzielgruppen synchronisiert werden?**

Nein, eine Liste kann nur mit einer einzelnen Ziel-Audience synchronisiert werden.

**Wenn ich die kontinuierliche Synchronisierung mit einer vorhandenen Anzeigenzielgruppe aktivieren, wird die vorhandene Zielgruppe ersetzt?**

Nein, die bestehende Zielgruppe wird hinzugefügt, nicht ersetzt.
