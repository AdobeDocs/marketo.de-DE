---
unique-page-id: 11378814
description: Kontolisten - Marketo-Dokumente - Produktdokumentation
title: Kontolisten
exl-id: 31bb4341-d012-4239-8f40-10a07cd4c51c
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 1%

---

# Kontolisten {#account-lists}

Eine Kontoliste ist eine Sammlung benannter Konten, die gemeinsam als Ziel ausgewählt werden können. Mit Kontolisten können Sie spezifische Konten nach Branche, Standort oder Größe des Unternehmens auswählen.

Zusätzlich zu den Kontolisten können Sie auch dynamische Kontolisten erstellen, die aus öffentlichen CRM-Kontoansichten generiert werden. Eine CRM-Kontoansicht ist ein Regelsatz, der beim Anzeigen von Konten als Filter dient. Sie können ihn beispielsweise verwenden, um Konten zu finden, in denen die Branche Gesundheitswesen ist. *und* Der Umsatz beträgt über 100 Mio. US-Dollar.

![](assets/one.png)

>[!NOTE]
>
>In der Marketo Target-Kontoverwaltung erstellte Kontolisten sind beim Erstellen von Smart-Listen und Webkampagnen in automatisch verfügbar. [Web-Personalisierung](/help/marketo/product-docs/web-personalization/using-web-segments/web-segments.md).

## Neue Kontoliste erstellen {#create-a-new-account-list}

1. Klicken Sie auf **Neu** und wählen Sie **Neue Kontoliste erstellen**.

   ![](assets/1a.png)

1. Benennen Sie Ihre Liste und klicken Sie auf **Erstellen**.

   ![](assets/three-0.png)

1. Nachdem Sie Ihre Kontoliste erstellt haben, beginnen Sie mit [Hinzufügen von benannten Konten](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)!

   >[!NOTE]
   >
   >Marketo zeigt nur Einblicke für Kontolisten mit 2.000 oder weniger benannten Konten an.

## Erstellen einer neuen dynamischen Kontoliste {#create-a-new-dynamic-account-list}

1. Klicken Sie auf **Neu** und wählen Sie **Erstellen einer neuen dynamischen Liste**.

   ![](assets/1.png)

1. Wählen Sie im Dialogfeld eine **CRM-Kontoansicht** aus der Dropdown-Liste oder geben Sie den Namen ein, nach dem gesucht werden soll.

   ![](assets/image2017-7-18-9-48-23.png)

1. Klicken Sie auf **Erstellen**.

   ![](assets/step4.jpg)

   >[!NOTE]
   >
   >Stellen Sie in Salesforce sicher, dass Sie dem Synchronisierungsbenutzer Berechtigungen für die Listenansicht &quot;Objekt&quot;gewähren.

## Umbenennen einer Kontoliste {#rename-an-account-list}

>[!NOTE]
>
>Diese Schritte gelten nur für Kontolisten. _Dynamik_ Kontolisten verwenden den Namen ihrer zugehörigen CRM-Kontoansichten.

1. Wählen Sie das Konto aus, das Sie umbenennen möchten, und klicken Sie auf das **Aktionen auf Kontolisten** und wählen Sie **Kontoliste umbenennen**.

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

1. Wählen Sie das Konto aus, das Sie löschen möchten, und klicken Sie auf das **Aktionen auf Kontolisten** und wählen Sie **Kontoliste löschen**.

   ![](assets/five.png)

1. Klicks **Löschen**.

   ![](assets/six.png)

>[!MORELIKETHIS]
>
>* [Vorhandenes benanntes Konto zu einer Kontoliste hinzufügen](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)
>* [Einblicke in die Kontoliste](/help/marketo/product-docs/target-account-management/measure/account-list-insights.md)
