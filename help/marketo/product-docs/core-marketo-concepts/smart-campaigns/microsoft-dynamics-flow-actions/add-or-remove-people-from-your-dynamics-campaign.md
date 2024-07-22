---
description: Hinzufügen oder Entfernen von Personen aus Ihrer Dynamics Campaign - Marketo Docs - Produktdokumentation
title: Hinzufügen oder Entfernen von Personen aus Ihrer Dynamics-Kampagne
exl-id: 4fea2f7c-0655-4816-8640-76878f760b6e
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 0%

---

# Hinzufügen oder Entfernen von Personen aus Ihrer Dynamics-Kampagne {#add-or-remove-people-from-your-dynamics-campaign}

## Zu Dynamics Campaign hinzufügen {#add-to-dynamics-campaign}

Dieser Flussschritt kann in Marketo Engage-Smart-Kampagnen verwendet werden, um Personen als Leads oder Kontakte in einer Microsoft-Kampagne hinzuzufügen. Wenn der Lead noch nicht in Dynamics vorhanden ist, wird er automatisch synchronisiert und zur Kampagne hinzugefügt.

>[!NOTE]
>
>Diese Flussaktion ist nur für Trigger-Kampagnen verfügbar.

Suchen und wählen Sie in Ihrer Smart-Kampagne die Dynamics-Kampagne aus, der Sie Ihre Personen hinzufügen möchten.

![](assets/add-or-remove-people-from-your-dynamics-campaign-1.png)

>[!NOTE]
>
>Wenn eine Dynamics-Kampagne nicht in der Kampagnenliste angezeigt wird:
>
>* Sicherstellen, dass die Kampagnensynchronisierung funktioniert
>* Die Kampagne ist in [!DNL Microsoft Dynamics] nicht aktiv

Das System erstellt automatisch eine kampagnenspezifische statische Marketing-Liste, die jeweils für Leads und Kontakte verwendet wird, um die Person hinzuzufügen. Es handelt sich um eine einmalige Aktion, bei der für nachfolgende Synchronisierungen mit der Kampagne dieselbe Marketing-Liste verwendet wird. Der für den statischen Namen der Marketing-Liste verwendete Namensstandard lautet `Mkto-leads-<uniqueID>` für Leads und `Mkto-contacts-<uniqueID>` für Kontakte.

Die Zuordnung dieser von Marketo generierten Marketinglisten zu anderen Kampagnen könnte zu Verwirrung führen. Beispiel: Wenn Sie eine Kampagne hinzufügen, wird auch die zweite Kampagne hinzugefügt. Ebenso ist es nicht empfehlenswert, die von Marketo generierte Marketingliste von der Kampagne in Dynamics zu trennen.

## Aus Dynamics Campaign entfernen {#remove-from-dynamics-campaign}

Dieser Flussschritt kann in Marketo-Smart-Kampagnen verwendet werden, um Personen aus einer Microsoft-Kampagne zu entfernen. Dadurch werden nur die Leads aus einer Kampagne entfernt, die zuvor über die Flussaktion &quot;Hinzugefügt zu Microsoft Campaign&quot;zur Kampagne hinzugefügt wurden.

>[!NOTE]
>
>Diese Flussaktion ist nur für Trigger-Kampagnen verfügbar.

Suchen und wählen Sie in Ihrer Smart-Kampagne die Dynamics-Kampagne aus, aus der Ihre Personen entfernt werden sollen.

![](assets/add-or-remove-people-from-your-dynamics-campaign-2.png)

>[!NOTE]
>
>Wenn keine Dynamics-Kampagne in der Kampagnenliste angezeigt wird:
>
>* Sicherstellen, dass die Kampagnensynchronisierung funktioniert
>* Die Kampagne ist in [!DNL Microsoft Dynamics] nicht aktiv
