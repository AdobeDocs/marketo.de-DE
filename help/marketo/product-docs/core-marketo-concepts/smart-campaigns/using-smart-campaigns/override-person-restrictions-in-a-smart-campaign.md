---
unique-page-id: 1147066
description: Überschreiben von Personenbeschränkungen in einer Smart-Kampagne - Marketo-Dokumente - Produktdokumentation
title: Überschreiben von Personenbeschränkungen in einer Smart-Kampagne
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
feature: Smart Campaigns
source-git-commit: 47bc93665a7efa0d64cd4d5f34b868895d407527
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---

# Überschreiben von Personenbeschränkungen in einer Smart-Kampagne {#override-person-restrictions-in-a-smart-campaign}

Mit Marketo Engage können Sie die maximale Anzahl von Personen festlegen, die sich für eine Smart-Kampagne qualifizieren können. Dadurch wird verhindert, dass versehentlich eine E-Mail an Ihre gesamte Datenbank gesendet wird. Wenn Sie _dieses Limit überschreiben_ möchten, sehen Sie wie:

>[!PREREQUISITES]
>
>Stellen Sie sicher, dass Sie in Marketo Admin [Personenbeschränkungen für Smart-Kampagnen](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md){target="_blank"} aktivieren.

1. Wechseln Sie in **[!UICONTROL Marketingaktivitäten]** zu Ihrer Smart-Kampagne und klicken Sie auf **[!UICONTROL Planung]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-1.png)

1. Klicken Sie in den Smart Campaign-Einstellungen auf **[!UICONTROL Bearbeiten]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >Die Standardbegrenzung ist die in Admin festgelegte.

1. Geben Sie eine neue Begrenzung ein und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-3.png)

   Die Smart-Kampagne wird nicht ausgeführt, wenn die Anzahl der Personen, die sich qualifizieren, die festgelegte Grenze überschreitet.

   >[!CAUTION]
   >
   >Seien Sie vorsichtig mit dieser Funktion, damit Sie nicht versehentlich zu viele Personen einschließen.
