---
unique-page-id: 11378814
description: Account-Listen - Marketing Docs - Produktdokumentation
title: Listen von Konten
translation-type: tm+mt
source-git-commit: e125f8469239a026aefb703fdb6ba99c32e33565
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---


# Konto-Listen {#account-lists}

Bei einer Kontosammlung handelt es sich um eine Liste benannter Konten, auf die ein Targeting durchgeführt werden kann. Mit den Kontoeinstellungen können Sie benannte Listen nach Branche, Standort oder Größe der Firma Zielgruppen vornehmen.

Zusätzlich zu den Listen für das Konto können Sie auch dynamische Kontoeinstellungen erstellen, die aus öffentlichen CRM-Konto-Ansichten generiert wurden. Eine CRM-Konto-Ansicht ist ein Regelsatz, der beim Anzeigen von Konten als Filter dient. Beispielsweise können Sie damit Konten suchen, bei denen der Umsatz unter &quot;Branche&quot;und unter *und* unter $100M liegt.

![](assets/one.png)

>[!NOTE]
>
>In &quot;Marketing to Account Based Marketing&quot;erstellte Listen stehen beim Erstellen intelligenter Listen und Web-Kampagnen in [Web-Personalisierung](/help/marketo/product-docs/web-personalization/using-web-segments/web-segments.md) automatisch zur Verfügung.

## Neue Konto-Liste {#create-a-new-account-list} erstellen

1. Klicken Sie auf die Dropdownliste **Neu** und wählen Sie **Neue Liste für das Konto erstellen**.

   ![](assets/1a.png)

1. Geben Sie der Liste einen Namen und klicken Sie auf **Erstellen**.

   ![](assets/three-0.png)

1. Nachdem Sie Ihre Konto-Liste erstellt haben, beginnen Sie mit dem [Hinzufügen benannter Konten zu ihr](/help/marketo/product-docs/account-based-marketing/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)!

   >[!NOTE]
   >
   >Marketo zeigt nur Einblicke in Kontokonten mit 2.000 oder weniger benannten Listen an.

## Neue Liste für dynamische Konten {#create-a-new-dynamic-account-list} erstellen

1. Klicken Sie auf die Dropdownliste **Neu** und wählen Sie **Neue dynamische Liste erstellen**.

   ![](assets/1.png)

1. Wählen Sie im Dialogfeld eine **CRM-Ansicht** aus der Dropdownliste oder geben Sie den Namen ein, nach dem gesucht werden soll.

   ![](assets/image2017-7-18-9-48-23.png)

1. Klicken Sie auf **Erstellen**.

   ![](assets/step4.jpg)

   >[!NOTE]
   >
   >Stellen Sie in Salesforce sicher, dass Sie dem Synchronisierungsbenutzer die Liste Ansicht Object-Berechtigungen zuweisen.

## Umbenennen einer Konto-Liste {#rename-an-account-list}

>[!NOTE]
>
>Diese Schritte gelten nur für Listen von Konten. _Dynamische_ Listen verwenden den Namen ihrer zugehörigen CRM-Konto-Ansichten.

1. Wählen Sie das Konto, das Sie umbenennen möchten, klicken Sie auf die Dropdownliste **Aktionen zur Liste von Konten** und wählen Sie **Liste des Kontos umbenennen**.

   ![](assets/three.png)

1. Geben Sie den neuen Namen ein und klicken Sie auf **Umbenennen**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >Die CRM-Konto-Ansicht wird alle 8 Stunden mit der Liste des dynamischen Kontos synchronisiert. Wenn sie noch nicht synchronisiert sind, synchronisiert Marketo sie im nächsten Zyklus.

## Löschen einer Konto-Liste {#delete-an-account-list}

>[!NOTE]
>
>Diese Schritte sind für Konto- und dynamische Listen gleich.

1. Wählen Sie das zu löschende Konto aus, klicken Sie auf die Dropdownliste **Aktionen zur Liste des Kontos** und wählen Sie **Liste des Kontos löschen**.

   ![](assets/five.png)

1. Klicken Sie auf **Löschen**.

   ![](assets/six.png)

>[!MORELIKETHIS]
>
>* [hinzufügen eines vorhandenen benannten Kontos zu einer Konto-Liste](/help/marketo/product-docs/account-based-marketing/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)
>* [Kontoeinblicke zur Liste](/help/marketo/product-docs/account-based-marketing/measure/account-list-insights.md)

