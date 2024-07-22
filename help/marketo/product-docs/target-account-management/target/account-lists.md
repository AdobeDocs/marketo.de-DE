---
unique-page-id: 11378814
description: Kontolisten - Marketo-Dokumente - Produktdokumentation
title: Kontenlisten
exl-id: 31bb4341-d012-4239-8f40-10a07cd4c51c
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 1%

---

# Kontenlisten {#account-lists}

Eine Kontoliste ist eine Sammlung benannter Konten, die gemeinsam als Ziel ausgewählt werden können. Mit Kontolisten können Sie spezifische Konten nach Branche, Standort oder Größe des Unternehmens auswählen.

Zusätzlich zu den Kontolisten können Sie auch dynamische Kontolisten erstellen, die aus öffentlichen CRM-Kontoansichten generiert werden. Eine CRM-Kontoansicht ist ein Regelsatz, der beim Anzeigen von Konten als Filter dient. Sie können ihn beispielsweise verwenden, um Konten zu finden, bei denen die Branche im Gesundheitswesen über 100 Mio. US-Dollar und der Umsatz über 100 Mio. US-Dollar liegt.**

![](assets/one.png)

>[!NOTE]
>
>In der Marketo Target-Kontoverwaltung erstellte Kontolisten sind beim Erstellen von Smart-Listen und Webkampagnen in [Web Personalization](/help/marketo/product-docs/web-personalization/using-web-segments/web-segments.md) automatisch verfügbar.

## Neue Kontoliste erstellen {#create-a-new-account-list}

1. Klicken Sie auf die Dropdownliste **Neu** und wählen Sie **Neue Kontoliste erstellen** aus.

   ![](assets/1a.png)

1. Geben Sie der Liste einen Namen und klicken Sie auf **Erstellen**.

   ![](assets/three-0.png)

1. Nachdem Sie Ihre Kontoliste erstellt haben, beginnen Sie mit [Hinzufügen benannter Konten dazu](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)!

   >[!NOTE]
   >
   >Marketo zeigt nur Einblicke für Kontolisten mit 2.000 oder weniger benannten Konten an.

## Erstellen einer neuen dynamischen Kontoliste {#create-a-new-dynamic-account-list}

1. Klicken Sie auf die Dropdownliste **Neu** und wählen Sie **Neue dynamische Liste erstellen** aus.

   ![](assets/1.png)

1. Wählen Sie im Dialogfeld eine **CRM-Kontoansicht** aus der Dropdown-Liste aus oder geben Sie den Namen ein, nach dem gesucht werden soll.

   ![](assets/image2017-7-18-9-48-23.png)

1. Klicken Sie auf **Erstellen**.

   ![](assets/step4.jpg)

   >[!NOTE]
   >
   >Stellen Sie in Salesforce sicher, dass Sie dem Synchronisierungsbenutzer Berechtigungen für die Listenansicht &quot;Objekt&quot;gewähren.

## Umbenennen einer Kontoliste {#rename-an-account-list}

>[!NOTE]
>
>Diese Schritte gelten nur für Kontolisten. _Dynamische_ Kontolisten verwenden den Namen der zugehörigen CRM-Kontoansichten.

1. Wählen Sie das Konto aus, das Sie umbenennen möchten, klicken Sie auf die Dropdownliste **Kontolistenaktionen** und wählen Sie **Kontoliste umbenennen** aus.

   ![](assets/three.png)

1. Geben Sie den neuen Namen ein und klicken Sie auf **Umbenennen**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Die Ansicht des CRM-Kontos wird alle 8 Stunden mit der Liste des dynamischen Kontos synchronisiert. Wenn sie noch nicht synchronisiert sind, synchronisiert Marketo sie während des nächsten Zyklus.

## Eine Kontoliste löschen {#delete-an-account-list}

>[!NOTE]
>
>Diese Schritte sind für Kontolisten und dynamische Kontolisten identisch.

1. Wählen Sie das Konto aus, das Sie löschen möchten, klicken Sie auf die Dropdownliste **Kontolistenaktionen** und wählen Sie **Kontoliste löschen** aus.

   ![](assets/five.png)

1. Klicken Sie auf **Löschen**.

   ![](assets/six.png)

>[!MORELIKETHIS]
>
>* [Hinzufügen eines vorhandenen benannten Kontos zu einer Kontoliste](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)
>* [Kontolisteneinblicke](/help/marketo/product-docs/target-account-management/measure/account-list-insights.md)
