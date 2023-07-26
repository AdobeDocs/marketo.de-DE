---
unique-page-id: 1147066
description: Überschreiben von Personenbeschränkungen in einer Smart-Kampagne - Marketo-Dokumente - Produktdokumentation
title: Überschreiben von Personenbeschränkungen in einer Smart-Kampagne
exl-id: 45ff3e36-01fd-42ea-ba74-efd98867a58a
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 0%

---

# Überschreiben von Personenbeschränkungen in einer Smart-Kampagne {#override-person-restrictions-in-a-smart-campaign}

Mit Marketo können Sie die maximale Anzahl von Personen festlegen, die sich für eine intelligente Kampagne qualifizieren können. So können Sie verhindern, dass versehentlich eine E-Mail an Ihre gesamte Datenbank gesendet wird. Wenn Sie möchten _override_ diese Grenze, so ist es.

>[!PREREQUISITES]
>
>Stellen Sie sicher, [Personenbeschränkungen für intelligente Kampagnen aktivieren](/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md) in Marketo Admin.

1. Gehen Sie in Marketingaktivitäten zu Ihrer Smart-Kampagne und klicken Sie auf **Zeitplan**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-1.png)

1. Klicken Sie in den Einstellungen für Smart Campaign auf **Bearbeiten**.

   ![](assets/override-person-restrictions-in-a-smart-campaign-2.png)

   >[!NOTE]
   >
   >Die Standardbegrenzung ist die in Admin festgelegte.

1. Geben Sie eine neue Begrenzung ein und klicken Sie auf **Speichern Sie.**

   ![](assets/override-person-restrictions-in-a-smart-campaign-3.png)

   Die Smart-Kampagne wird nicht ausgeführt, wenn die Anzahl der Personen, die sich qualifizieren, die festgelegte Grenze überschreitet.

   >[!CAUTION]
   >
   >Seien Sie vorsichtig mit dieser Funktion, damit Sie nicht versehentlich zu viele Personen einschließen.
