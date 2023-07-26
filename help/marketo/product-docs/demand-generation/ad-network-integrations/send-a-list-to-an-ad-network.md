---
description: Senden einer Liste an ein Werbenetzwerk - Marketo Docs - Produktdokumentation
title: Senden einer Liste an ein Werbenetzwerk
exl-id: d5c55df7-53c8-491a-9d79-ecf7c25cee08
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Senden einer Liste an ein Werbenetzwerk {#send-a-list-to-an-ad-network}

Erfahren Sie, wie Sie eine statische Liste an LinkedIn, Facebook oder Google senden.

## Senden einer Liste {#how-to-send-a-list}

1. Wählen Sie in Marketo Ihre Liste aus und klicken Sie auf das **Aktionen auflisten** und wählen Sie **An Werbenetzwerk senden**.

   ![](assets/send-a-list-to-an-ad-network-1.png)

1. Wählen Sie zwischen LinkedIn, Facebook oder Google (die anderen Optionen sind derzeit nicht verfügbar). In diesem Beispiel wählen wir **LinkedIn**. Klicks **Nächste**.

   ![](assets/send-a-list-to-an-ad-network-2.png)

1. Klicken Sie auf das Dropdown-Menü Zielgruppe und wählen Sie die gewünschte Zielgruppe aus.

   ![](assets/send-a-list-to-an-ad-network-3.png)

   >[!TIP]
   >
   >Wenn Sie jemals eine Prüfung durchführen müssen, können Sie über den Tab Status die Ziel-Audience sehen, mit der eine Liste synchronisiert wird.

1. Wählen Sie den gewünschten Push-Typ aus und klicken Sie auf **Aktualisieren**.

   ![](assets/send-a-list-to-an-ad-network-4.png)

   >[!NOTE]
   >
   >Wenn Sie &quot;Kontinuierliche Zielgruppensynchronisierung aktivieren&quot;auswählen, behält Marketo die Liste im ausgewählten Werbenetzwerk auf dem neuesten Stand, da sich die Liste in Ihrer Marketo-Instanz ändert. Wir fügen beide hinzu **und** Personen aus der Zielgruppe entfernen, wenn sie der statischen Liste hinzugefügt/daraus entfernt wurden.

1. Und das ist es! Klicks **OK** zu beenden.

   ![](assets/send-a-list-to-an-ad-network-5.png)

## FAQs {#faq}

**Kann eine einzelne statische Liste mit mehreren Anzeigenzielgruppen synchronisiert werden?**

Nein, eine Liste kann nur mit einer einzelnen Ziel-Audience synchronisiert werden.

**Wird die vorhandene Zielgruppe ersetzt, wenn ich die kontinuierliche Synchronisierung mit einer vorhandenen Anzeigenzielgruppe aktivieren?**

Nein, die bestehende Zielgruppe wird hinzugefügt, nicht ersetzt.
