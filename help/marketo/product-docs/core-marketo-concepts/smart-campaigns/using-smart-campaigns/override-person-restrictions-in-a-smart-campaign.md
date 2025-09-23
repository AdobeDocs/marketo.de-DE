---
unique-page-id: 1147066
description: Überschreiben von Personenbeschränkungen in einer Smart-Kampagne - Marketo-Dokumente - Produktdokumentation
title: Überschreiben von Personenbeschränkungen in einer intelligenten Kampagne
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
feature: Smart Campaigns
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 10%

---

# Überschreiben von Personenbeschränkungen in einer intelligenten Kampagne {#override-person-restrictions-in-a-smart-campaign}

Mit Marketo Engage können Sie die maximale Anzahl von Personen festlegen, die sich für eine intelligente Kampagne qualifizieren können. So vermeiden Sie, dass Sie versehentlich eine E-Mail an Ihre gesamte Datenbank senden. Wenn Sie diese _außer Kraft setzen_, sehen Sie wie folgt aus:

>[!PREREQUISITES]
>
>Stellen Sie sicher, dass Sie [Personenbeschränkungen für Smart-Kampagnen aktivieren](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md){target="_blank"} in Marketo Admin auswählen.

1. Gehen Sie **[!UICONTROL Marketing]** Aktivitäten) zu Ihrer Smart-Kampagne und klicken Sie auf **[!UICONTROL Zeitplan]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-1.png)

1. Klicken Sie in den Einstellungen für intelligente Kampagnen auf **[!UICONTROL Bearbeiten]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >Das Standardlimit ist dasjenige, das in Admin festgelegt ist.

1. Geben Sie ein neues Limit ein und klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-3.png)

   Die intelligente Kampagne wird nicht ausgeführt, wenn die Anzahl der Personen, die sich qualifizieren, das festgelegte Limit überschreitet.

   >[!CAUTION]
   >
   >Seien Sie bei dieser Funktion vorsichtig, damit Sie nicht versehentlich zu viele Personen einbeziehen.
