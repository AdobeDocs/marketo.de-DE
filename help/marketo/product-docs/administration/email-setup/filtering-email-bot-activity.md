---
description: Filtern der E-Mail-Bot-Aktivität - Marketo Docs - Produktdokumentation
title: Filtern der E-Mail-Bot-Aktivität
source-git-commit: b491f476c4facc6343559a0acf5d5527e9afc618
workflow-type: tm+mt
source-wordcount: '136'
ht-degree: 0%

---

# Filtern der E-Mail-Bot-Aktivität {#filtering-email-bot-activity}

Manchmal kann die E-Mail-Bot-Aktivität fälschlicherweise dazu führen, dass Ihre E-Mail geöffnet und Klickdaten hochgezählt werden. Hier ist, wie man das repariert.

>[!NOTE]
>
>Mit der [IAB/ABC International Spiders and Bots-Liste](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/) werden alle open/click-Aktivitäten mit einer IP oder einem Benutzeragent, die zu irgendetwas aus dieser Liste passen, als Bot-Aktivität identifiziert und nicht in Marketo angemeldet.

1. Klicken Sie auf **Admin**.

   ![](assets/filtering-email-bot-activity-1.png)

1. Klicken Sie auf **E-Mail**.

   ![](assets/filtering-email-bot-activity-2.png)

1. Klicken Sie auf die Registerkarte **Bot-Aktivität**.

   ![](assets/filtering-email-bot-activity-3.png)

1. Aktivieren Sie das Kontrollkästchen **Filterung der E-Mail-Bot-Aktivität aktivieren**.

   ![](assets/filtering-email-bot-activity-4.png)

>[!NOTE]
>
>Wenn Sie diese Funktion aktivieren, wird möglicherweise eine Dropdown-E-Mail geöffnet, und es werden Klicks angezeigt, wenn die Anzahl der Falsch-Zahlen herausgefiltert wird.

**OPTIONALER SCHRITT**: Um die Funktion zu deaktivieren, deaktivieren Sie einfach das Kontrollkästchen. Wenn Sie die Option deaktivieren, werden die Daten für die &quot;Bot-Aktivität in den letzten 90 Tagen&quot; **nicht** zurückgesetzt.
