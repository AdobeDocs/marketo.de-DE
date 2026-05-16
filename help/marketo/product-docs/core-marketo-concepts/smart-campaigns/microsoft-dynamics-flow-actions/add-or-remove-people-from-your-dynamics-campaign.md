---
description: Erfahren Sie, wie Sie mit einem Flussschritt Personen zu einer Microsoft Dynamics-Kampagne hinzufügen oder daraus entfernen. Marketo mit Dynamics-Kampagnen synchronisieren.
title: Personen zu Ihrer Kampagne hinzufügen oder aus  [!DNL Dynamics]  entfernen
exl-id: 4fea2f7c-0655-4816-8640-76878f760b6e
feature: Smart Campaigns, Microsoft Dynamics
TQID: https://experienceleague.adobe.com/b6tUqixPGr7ZWTUKVg4L6EKryziHA2IwzpuTepWWEwU
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: a7170d27-32ab-462b-a333-269abc654483
subfeature_v2:
  - id: ad89fb33-8541-4339-afe7-bb13d1633714
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 324
ht-degree: 0%

---

# Personen zu Ihrer [!DNL Dynamics] Campaign hinzufügen oder daraus entfernen {#add-or-remove-people-from-your-dynamics-campaign}

## Zu Dynamics Campaign hinzufügen {#add-to-dynamics-campaign}

Dieser Flussschritt kann in Marketo Engage Smart Campaign verwendet werden, um Personen als Leads oder Kontakte in einer Microsoft-Kampagne hinzuzufügen. Wenn der Lead noch nicht in Dynamics vorhanden ist, wird er automatisch synchronisiert und der Kampagne hinzugefügt.

>[!NOTE]
>
>Diese Flussaktion ist nur für Trigger-Kampagnen verfügbar.

Suchen Sie in Ihrer Smart-Kampagne die Dynamics-Kampagne, der Sie Ihre Mitarbeiter hinzufügen möchten, und wählen Sie sie aus.

![](assets/add-or-remove-people-from-your-dynamics-campaign-1.png)

>[!NOTE]
>
>Wenn eine Dynamics-Kampagne nicht in der Kampagnenliste angezeigt wird:
>
>* Überprüfen, ob die Kampagnensynchronisierung funktioniert
>* Die Kampagne ist in [!DNL Microsoft Dynamics] nicht aktiv

Das System erstellt automatisch für jede Kampagne eine statische Marketing-Liste für Leads und Kontakte, um die Person hinzuzufügen. Es handelt sich um eine einmalige Aktion und einmal für nachfolgende Synchronisationen mit der Kampagne wird dieselbe Marketing-Liste verwendet. Der für den statischen Namen der Marketing-Liste verwendete Benennungsstandard ist für Leads und `Mkto-contacts-<uniqueID>` für Kontakte `Mkto-leads-<uniqueID>`.

Die Zuordnung dieser von Marketo generierten Marketing-Listen zu anderen Kampagnen könnte zu verwirrendem Verhalten führen. Das Hinzufügen zu einer Kampagne führt beispielsweise auch zum Hinzufügen zu der zweiten Kampagne. Es wird auch nicht empfohlen, die von Marketo generierte Marketing-Liste von der Kampagne in [!DNL Dynamics] zu trennen.

## Aus Dynamics Campaign entfernen {#remove-from-dynamics-campaign}

Dieser Flussschritt kann in Marketo Smart-Kampagnen verwendet werden, um Personen aus einer Microsoft-Kampagne zu entfernen. Dadurch werden nur die Leads aus einer Kampagne entfernt, die zuvor über die Flussaktion „Zu Microsoft Campaign hinzugefügt“ zur Kampagne hinzugefügt wurden.

>[!NOTE]
>
>Diese Flussaktion ist nur für Trigger-Kampagnen verfügbar.

Suchen Sie in Ihrer Smart-Kampagne die Dynamics-Kampagne, aus der Sie Ihre Personen entfernen möchten, und wählen Sie sie aus.

![](assets/add-or-remove-people-from-your-dynamics-campaign-2.png)

>[!NOTE]
>
>Wenn in der Kampagnenliste keine [!DNL Dynamics] Kampagne angezeigt wird:
>
>* Überprüfen, ob die Kampagnensynchronisierung funktioniert
>* Die Kampagne ist in [!DNL Microsoft Dynamics] nicht aktiv
