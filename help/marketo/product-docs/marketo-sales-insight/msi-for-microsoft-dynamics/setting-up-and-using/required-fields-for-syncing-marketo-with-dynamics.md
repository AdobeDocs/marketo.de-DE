---
unique-page-id: 11375827
description: Erforderliche Felder für die Synchronisierung von Marketing mit Dynamik - Marketing Docs - Produktdokumentation
title: Erforderliche Felder für die Synchronisierung von Marketing mit Dynamik
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---


# Erforderliche Felder für die Synchronisierung von Marketing mit Dynamik {#required-fields-for-syncing-marketo-with-dynamics}

Diese Felder *müssen mit Marketo synchronisiert werden, damit Lead und Kontaktinformationen für Sales Insight funktionieren:*

* Priorität
* Dringlichkeit
* Relative Bewertung

Wenn eines dieser Felder fehlt, wird in Marketo eine Fehlermeldung mit dem Namen der fehlenden Felder angezeigt. Um dies zu beheben, überprüfen Sie in Ihrer Instanz, ob die Felder für **Lead** und **Kontakt** synchronisiert werden. Falls nicht, fügen Sie sie hinzu.

So überprüfen und fügen Sie Synchronisierungsfelder hinzu:

1. Gehen Sie zu Admin und klicken Sie auf **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicken Sie unter &quot;Details zur Feldsynchronisierung&quot;auf **Bearbeiten**.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Aktivieren Sie unter &quot;Interessent&quot;das Kontrollkästchen Priorität.

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. Blättern Sie jetzt nach unten und aktivieren Sie das Kontrollkästchen &quot;Dringlichkeit&quot;...

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. ...und das Kontrollkästchen Relative Bewertung.

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. Aktivieren Sie anschließend die Kontrollkästchen für Priorität, Dringlichkeit und relative Punktzahl für Kontakt.

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>Warten Sie mindestens 10 Minuten, bis eine Synchronisierung ausgeführt wird, bevor Sie überprüfen, ob das Problem behoben wurde.

>[!MORELIKETHIS]
>
>[Einrichten von Sternen und Flammen für Lead-/Kontaktdatensätze](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
