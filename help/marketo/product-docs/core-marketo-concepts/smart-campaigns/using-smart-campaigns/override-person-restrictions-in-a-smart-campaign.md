---
unique-page-id: 1147066
description: Außerkraftsetzen von Personenbeschränkungen in einer intelligenten Kampagne - Marketing Docs - Produktdokumentation
title: Personenbeschränkungen in einer intelligenten Kampagne überschreiben
translation-type: tm+mt
source-git-commit: 4a0bd2efe99284807a46d07ffef0070d9a303631
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 0%

---


# Personenbeschränkungen in einer intelligenten Kampagne {#override-person-restrictions-in-a-smart-campaign} überschreiben

Mit Marketo können Sie festlegen, wie viele Personen maximal für eine intelligente Kampagne qualifiziert sein können. Dadurch vermeiden Sie versehentlich das Versenden Ihrer gesamten Datenbank per E-Mail. Wenn Sie _override_ diese Beschränkung anwenden möchten, hier sehen Sie wie.

>[!PREREQUISITES]
>
>Stellen Sie sicher, dass Sie in Marketing Admin Personenbeschränkungen für intelligente Kampagnen](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md) aktivieren.[

1. Gehen Sie in den Marketing-Aktivitäten zu Ihrer Smart-Kampagne und klicken Sie auf **Plan**.

   ![](assets/one.png)

1. Klicken Sie in den Einstellungen für intelligente Kampagne auf **Bearbeiten**.

   ![](assets/two.png)

   >[!NOTE]
   >
   >Der Standardwert ist der in Admin festgelegte Grenzwert.

1. Geben Sie einen neuen Grenzwert ein und klicken Sie auf **Speichern.**

   ![](assets/three.png)

   Die intelligente Kampagne wird nicht ausgeführt, wenn die Anzahl der Personen, die sich qualifizieren, die festgelegte Grenze überschreitet.

   >[!CAUTION]
   >
   >Seien Sie vorsichtig mit dieser Funktion, damit Sie nicht versehentlich zu viele Personen einschließen.
