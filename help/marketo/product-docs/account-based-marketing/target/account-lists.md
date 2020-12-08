---
unique-page-id: 11378814
description: Account-Listen - Marketing Docs - Produktdokumentation
title: Listen von Konten
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---


# Listen von Konten {#account-lists}

Bei einer Kontosammlung handelt es sich um eine Liste benannter Konten, auf die ein Targeting durchgeführt werden kann. Mit den Kontoeinstellungen können Sie benannte Listen nach Branche, Standort oder Größe der Firma Zielgruppen vornehmen.

Zusätzlich zu den Listen für das Konto können Sie auch dynamische Kontoeinstellungen erstellen, die aus öffentlichen CRM-Konto-Ansichten generiert wurden. Eine CRM-Konto-Ansicht ist ein Regelsatz, der beim Anzeigen von Konten als Filter dient. Sie können es beispielsweise verwenden, um Konten zu finden, bei denen die Branche Gesundheitswesen ist *und* der Umsatz über 100 Mio. US-Dollar liegt.

![](assets/one.png)

>[!NOTE]
>
>Bei der Erstellung intelligenter Listen und Web-Kampagnen in der [Web-Personalisierung](http://docs.marketo.com/display/DOCS/RTP+Segments)stehen in Marketing-to-Account-basiertem Marketing erstellte Kontoeinstellungen automatisch zur Verfügung.

## Eine Liste für ein neues Konto erstellen {#create-a-new-account-list}

1. Klicken Sie auf die Dropdownliste **Neu** und wählen Sie Liste **Neues Konto** erstellen.

   ![](assets/1a.png)

1. Benennen Sie Ihre Liste und klicken Sie auf **Erstellen**.

   ![](assets/three-0.png)

1. Nachdem Sie Ihre Account-Liste erstellt haben, beginnen Sie damit, benannte Konten [hinzuzufügen](http://docs.marketo.com/display/DOCS/Add+an+Existing+Named+Account+to+an+Account+List)!

   >[!NOTE]
   >
   >Marketo zeigt nur Einblicke in Kontokonten mit 2.000 oder weniger benannten Listen an.

## Neue Liste für dynamische Konten erstellen {#create-a-new-dynamic-account-list}

1. Klicken Sie auf die Dropdownliste **Neu** und wählen Sie Neue dynamische Liste **erstellen**.

   ![](assets/1.png)

1. Wählen Sie im Dialogfeld eine **CRM-Konto-Ansicht** aus der Dropdown-Liste aus oder geben Sie den gewünschten Namen ein.

   ![](assets/image2017-7-18-9-48-23.png)

1. Klicken Sie auf **Erstellen**.

   ![](assets/step4.jpg)

   >[!NOTE]
   >
   >Stellen Sie in Salesforce sicher, dass Sie dem Synchronisierungsbenutzer die Liste Ansicht Object-Berechtigungen zuweisen.

## Umbenennen einer Konto-Liste {#rename-an-account-list}

>[!NOTE]
>
>Diese Schritte gelten nur für Listen von Konten. *Dynamische* Listen verwenden den Namen ihrer zugehörigen CRM-Ansichten.

1. Wählen Sie das Konto aus, das Sie umbenennen möchten, klicken Sie auf die Dropdownliste Aktionen zur **Liste** des Kontos und wählen Sie Liste **** umbenennen.

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

1. Wählen Sie das zu löschende Konto aus, klicken Sie auf die Dropdownliste Aktionen zur **KontoListe** und wählen Sie Liste **zum** Löschen des Kontos.

   ![](assets/five.png)

1. Klicken Sie auf **Löschen**.

   ![](assets/six.png)

>[!NOTE]
>
>**Verwandte Artikel**
>
>* [hinzufügen eines vorhandenen benannten Kontos zu einer Konto-Liste](named-accounts/add-an-existing-named-account-to-an-account-list.md)
>* [Kontoeinblicke zur Liste](../../../product-docs/account-based-marketing/measure/account-list-insights.md)

>



