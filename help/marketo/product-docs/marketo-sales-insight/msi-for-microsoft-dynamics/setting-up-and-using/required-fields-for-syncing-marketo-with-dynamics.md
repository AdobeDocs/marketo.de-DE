---
unique-page-id: 11375827
description: Erforderliche Felder zum Synchronisieren von Marketo mit Dynamics - Marketo-Dokumente - Produktdokumentation
title: Erforderliche Felder zum Synchronisieren von Marketo mit Dynamics
exl-id: c1b9d208-bdc0-4718-b3e5-e9e915b8ae0f
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 7%

---

# Erforderliche Felder zum Synchronisieren von Marketo mit [!DNL Dynamics] {#required-fields-for-syncing-marketo-with-dynamics}

Diese Felder *müssen* mit Marketo synchronisiert werden, [!UICONTROL &#x200B; sowohl Lead] als auch [!UICONTROL Kontakt] funktionieren [!DNL Sales Insight]:

* Priorität
* Dringlichkeit
* Relative Bewertung

Wenn eines dieser Felder fehlt, wird in Marketo eine Fehlermeldung mit dem Namen der fehlenden Felder angezeigt. Um dies zu beheben, überprüfen Sie Ihre Instanz, um sicherzustellen, dass die Felder sowohl für **[!UICONTROL Lead]** als auch für **[!UICONTROL Kontakt]** synchronisiert sind. Falls nicht, fügen Sie sie hinzu.

So können Sie Synchronisierungsfelder überprüfen und hinzufügen.

1. Wechseln Sie zu [!UICONTROL Admin] und klicken Sie auf **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicken Sie **[!UICONTROL Bearbeiten]** auf [!UICONTROL Details zur Feldsynchronisierung].

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Aktivieren [!UICONTROL &#x200B; unter &#x200B;] das Kontrollkästchen [!UICONTROL Priorität].

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. Scrollen Sie nun nach unten und aktivieren Sie das Kontrollkästchen [!UICONTROL Dringlichkeit] …

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. …und das Kontrollkästchen [!UICONTROL Relative Bewertung].

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. Aktivieren Sie anschließend die Kontrollkästchen für [!UICONTROL Priorität], [!UICONTROL Dringlichkeit] und [!UICONTROL Relative Bewertung] für [!UICONTROL Kontakt].

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>Warten Sie mindestens 10 Minuten, bis eine Synchronisierung ausgeführt wird, bevor Sie überprüfen, ob Sie das Problem behoben haben.

>[!MORELIKETHIS]
>
>[Einrichten von Sternen und Flammen für Lead-/Kontakt-Datensätze](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
