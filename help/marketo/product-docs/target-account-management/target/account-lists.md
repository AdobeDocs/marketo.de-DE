---
unique-page-id: 11378814
description: '[!UICONTROL Kontolisten] - Marketo-Dokumente - Produktdokumentation'
title: '[!UICONTROL Kontolisten]'
exl-id: 31bb4341-d012-4239-8f40-10a07cd4c51c
feature: Target Account Management
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 1%

---

# [!UICONTROL Kontolisten] {#account-lists}

Eine Kontenliste ist eine Sammlung benannter Konten, die als Ziel ausgewählt werden können. Mit Account-Listen können Sie benannte Accounts nach Branche, Standort oder Größe des Unternehmens auswählen.

Zusätzlich zu den Kontolisten können Sie auch dynamische Kontolisten erstellen, die aus öffentlichen CRM-Kontoansichten generiert werden. Eine CRM-Kontoansicht ist ein Regelsatz, der beim Anzeigen von Konten als Filter dient. Sie können damit beispielsweise Konten suchen, bei denen die Branche das Gesundheitswesen ist *und der* über 100 Millionen US-Dollar beträgt.

![](assets/one.png)

>[!NOTE]
>
>In Marketo erstellte Kontolisten [!UICONTROL Target-Kontoverwaltung] sind beim Erstellen von Smart Lists und Web-Kampagnen in [Web Personalization](/help/marketo/product-docs/web-personalization/using-web-segments/web-segments.md) automatisch verfügbar.

## Erstellen einer neuen Kontoliste {#create-a-new-account-list}

1. Klicken Sie auf **[!UICONTROL Neu]** und wählen Sie **[!UICONTROL Neue Kontoliste erstellen]**.

   ![](assets/1a.png)

1. Benennen Sie Ihre Liste und klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/three-0.png)

1. Nachdem Sie Ihre Kontoliste erstellt haben, beginnen Sie mit dem [Hinzufügen benannter Konten](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)!

   >[!NOTE]
   >
   >Marketo zeigt nur Einblicke für Kontolisten mit 2.000 oder weniger benannten Konten an.

## Erstellen einer neuen Liste für dynamische Konten {#create-a-new-dynamic-account-list}

1. Klicken Sie auf **[!UICONTROL Neu]** und wählen Sie **[!UICONTROL Neue dynamische Liste erstellen]**.

   ![](assets/1.png)

1. Wählen Sie im Dialogfeld eine **CRM-Kontoansicht** aus der Dropdown-Liste aus oder geben Sie den Namen ein, um danach zu suchen.

   ![](assets/image2017-7-18-9-48-23.png)

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

   ![](assets/step4.jpg)

   >[!NOTE]
   >
   >Stellen Sie in Salesforce sicher, dass Sie dem Synchronisierungsbenutzer Berechtigungen für Listenansichtsobjekte gewähren.

## Umbenennen einer Kontoliste {#rename-an-account-list}

>[!NOTE]
>
>Diese Schritte gelten nur für Kontolisten. _Dynamic_-Kontolisten verwenden den Namen der zugehörigen CRM-Kontoansichten.

1. Wählen Sie das Konto aus, das Sie umbenennen möchten, klicken Sie auf die Dropdown **[!UICONTROL Liste der Kontoaktionen]** und wählen Sie **[!UICONTROL Kontoliste umbenennen]**.

   ![](assets/three.png)

1. Geben Sie den neuen Namen ein und klicken Sie auf &quot;**[!UICONTROL &quot;]**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Die CRM-Kontoansicht wird alle 8 Stunden mit der dynamischen Kontoliste synchronisiert. Wenn sie noch nicht synchronisiert sind, synchronisiert Marketo sie im nächsten Zyklus.

## Löschen einer Kontoliste {#delete-an-account-list}

>[!NOTE]
>
>Diese Schritte sind sowohl für Kontolisten als auch für dynamische Kontolisten identisch.

1. Wählen Sie das zu löschende Konto aus, klicken Sie auf die Dropdown **[!UICONTROL Liste „Aktionen“ und]** Sie **[!UICONTROL Kontoliste löschen]**.

   ![](assets/five.png)

1. Klicken Sie auf **[!UICONTROL Löschen]**.

   ![](assets/six.png)

>[!MORELIKETHIS]
>
>* [Hinzufügen eines vorhandenen [!UICONTROL benannten Kontos] zu einer Kontoliste](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)
>* [Einblicke in Kontolisten](/help/marketo/product-docs/target-account-management/measure/account-list-insights.md)
