---
unique-page-id: 1147066
description: Erfahren Sie, wie Sie Personenbeschränkungen in einer intelligenten Kampagne überschreiben. Erlauben Sie Benutzern, selbst dann zu laufen, wenn sie Kommunikationsbeschränkungen erreichen.
title: Überschreiben von Personenbeschränkungen in einer intelligenten Kampagne
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
feature: Smart Campaigns
TQID: https://experienceleague.adobe.com/GUIwrHBCrtl5NONZAqCY9sXt1FaLfjBwe3N3t1u98a4
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 146
ht-degree: 9%

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
