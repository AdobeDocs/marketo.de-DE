---
unique-page-id: 11375827
description: Erforderliche Felder für die Synchronisierung von Marketo mit Dynamics - Marketo Docs - Produktdokumentation
title: Erforderliche Felder für die Synchronisierung von Marketo mit Dynamics
exl-id: c1b9d208-bdc0-4718-b3e5-e9e915b8ae0f
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 3%

---

# Erforderliche Felder für die Synchronisierung von Marketo mit Dynamics {#required-fields-for-syncing-marketo-with-dynamics}

Diese Felder *müssen* mit Marketo synchronisiert werden, damit sowohl Lead als auch Contact for Sales Insight funktionieren:

* Priorität
* Dringlichkeit
* Relative Bewertung

Wenn eines dieser Felder fehlt, wird in Marketo eine Fehlermeldung mit dem Namen der fehlenden Felder angezeigt. Um dies zu beheben, überprüfen Sie in Ihrer Instanz, ob die Felder sowohl für **Lead** als auch für **Kontakt** synchronisiert sind. Wenn nicht, fügen Sie sie hinzu.

So können Sie Synchronisierungsfelder überprüfen und hinzufügen.

1. Wechseln Sie zu &quot;Admin&quot;und klicken Sie auf **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Klicken Sie in den Details zur Feldsynchronisierung auf **Bearbeiten** .

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Aktivieren Sie unter Lead das Kontrollkästchen Priorität .

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. Scrollen Sie jetzt nach unten und aktivieren Sie das Kontrollkästchen &quot;Dringlichkeit&quot;...

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. ... und das Kontrollkästchen Relative Bewertung .

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. Aktivieren Sie als Nächstes die Kontrollkästchen für &quot;Priorität&quot;, &quot;Dringlichkeit&quot;und &quot;Relatives Ergebnis für Kontakt&quot;.

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. Klicken Sie auf **Speichern**.

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>Warten Sie mindestens 10 Minuten, bis eine Synchronisation ausgeführt wird, bevor Sie überprüfen, ob Sie das Problem behoben haben.

>[!MORELIKETHIS]
>
>[Einrichten von Sternen und Flammen für Lead-/Kontaktdatensätze](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
