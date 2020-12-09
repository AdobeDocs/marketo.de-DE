---
title: override-person-limits-in-a-smart-Kampagne
description: Personenbeschränkungen in einer intelligenten Kampagne überschreiben
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---


# Personenbeschränkungen in einer intelligenten Kampagne überschreiben

<br> 

Mit Marketo können Sie festlegen, wie viele Personen maximal für eine intelligente Kampagne qualifiziert sein können. Dadurch vermeiden Sie versehentlich das Versenden Ihrer gesamten Datenbank per E-Mail. Wenn Sie diese Beschränkung überschreiben möchten, so geht es.

>[!IMPORTANT]
>
>Stellen Sie sicher, dass Sie [Personenbeschränkungen für intelligente Kampagnen](https://docs.marketo.com/display/DOCS/Enable+Person+Restrictions+for+Smart+Campaigns) in Marketing [!UICONTROL Admin]aktivieren.

1. Suchen Sie Ihre intelligente Kampagne und klicken Sie auf **[!UICONTROL Planen]**.

   ![Bild eins](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-1.png)

1. Klicken Sie auf **[!UICONTROL Qualifikationsregeln]**.

   ![Bild zwei](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >Der Standardwert ist der in Admin festgelegte Grenzwert.

1. Geben Sie neben Kampagne **[!UICONTROL abbrechen, wenn qualifizierte Interessenten größer]** sind, einen neuen Grenzwert ein.

   ![Bild drei](/help/sky/assets/smart-campaigns/override-person-restrictions-in-a-smart-campaign/override-person-restrictions-in-a-smart-campaign-3.png)

>[!NOTE]
>
>Die intelligente Kampagne wird nicht ausgeführt, wenn die Anzahl der Personen, die sich qualifizieren, die festgelegte Grenze überschreitet.

>[!CAUTION]
>
>Seien Sie vorsichtig mit dieser Funktion, damit Sie nicht versehentlich zu viele Personen einschließen.
