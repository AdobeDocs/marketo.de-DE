---
description: Filtern der E-Mail-Bot-Aktivität - Marketo-Dokumente - Produktdokumentation
title: Filtern der E-Mail-Bot-Aktivität
exl-id: 70c97159-72bf-46e5-b29b-247615d0fa80
source-git-commit: a64c499f6972e94adfecbe164d86f7db1b1447aa
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 0%

---

# Filtern der E-Mail-Bot-Aktivität {#filtering-email-bot-activity}

Manchmal kann die E-Mail-Bot-Aktivität fälschlicherweise die Daten Ihrer E-Mail-Öffnungen und Klicks verfälschen. Hier ist, wie man das repariert.

>[!NOTE]
>
>Verwenden der [IAB/ABC International Spiders and Bots List](https://www.iab.com/guidelines/iab-abc-international-spiders-bots-list/), werden alle Öffnungs-/Klickaktivitäten mit einer IP-Adresse oder einem Benutzeragenten, die mit irgendetwas aus dieser Liste übereinstimmen, als Bot-Aktivität identifiziert und nicht in Marketo protokolliert.

1. Klicken **Admin**.

   ![](assets/filtering-email-bot-activity-1.png)

1. Klicken **Email**.

   ![](assets/filtering-email-bot-activity-2.png)

1. Klicken Sie auf **Bot-Aktivität** Registerkarte.

   ![](assets/filtering-email-bot-activity-3.png)

1. Klicken Sie auf den Regler, um **Bot-Aktivität filtern**.

   ![](assets/filtering-email-bot-activity-4.png)

>[!NOTE]
>
>Sie können getrennt entscheiden, ob die Bot-Aktivität protokolliert werden soll oder nicht. Wenn Sie dies ablehnen, können Sie einen Rückgang bei E-Mail-Öffnungen und Klicks sehen, da falsche Zahlen herausgefiltert werden.

**OPTIONALER SCHRITT**: Um die Funktion zu deaktivieren, deaktivieren Sie einfach den Schieberegler. Wenn Sie die Option deaktivieren, werden die Daten zur &quot;Bot-Aktivität in den letzten 90 Tagen&quot;wie folgt geändert: **not** zurücksetzen.

>[!TIP]
>
>Nutzen Sie Bot-Aktivitätsdaten in Smart-Listen über den booleschen Wert &quot;Is Bot Activity&quot;(Ja/Nein) oder in entsprechenden Filter-/Trigger-Beschränkungen.
