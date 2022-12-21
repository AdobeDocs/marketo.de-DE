---
unique-page-id: 11378713
description: Trigger von benutzerdefinierten Objektänderungen - Marketo Docs - Produktdokumentation
title: Trigger von benutzerdefinierten Objektänderungen
exl-id: a2a3d82f-33ae-4191-b114-dbbf944a66c8
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---

# Trigger von benutzerdefinierten Objektänderungen {#trigger-off-custom-object-changes}

>[!NOTE]
>
>Diese Funktion ist nur verfügbar:
>
>* Für Kunden in der Orion-Infrastruktur
>* Nur für die Verwendung mit benutzerdefinierten Marketo-Objekten, nicht jedoch für benutzerdefinierte Objekte, die durch die native Salesforce- oder Microsoft Dynamics-Integration synchronisiert werden
>* Trigger, kein Filter
>
>Bitte kontaktieren Sie uns [Marketo-Support](https://nation.marketo.com/t5/Support/ct-p/Support) , damit die Trigger für die benutzerdefinierte Objektänderung aktiviert sind.

In der Smart-Liste einer Smart-Kampagne können Sie eine Flow-Aktion Trigger haben, wenn ein benutzerdefiniertes Objekt zu einer Person oder einem Unternehmen hinzugefügt wird. Sie können auch eine Smart-Liste erstellen, die eine *change* in einem benutzerdefinierten Objekt als Trigger. Beispielsweise können Sie damit eine E-Mail senden, wenn ein Kursname aktualisiert wird.

>[!NOTE]
>
>Ein Aktivitätsprotokolleintrag wird nicht erstellt, wenn ein benutzerdefinierter Objektdatensatz geändert wird.

1. Navigieren Sie in Marketo zu **Marketingaktivitäten.**

   ![](assets/image2016-7-25-15-3a49-3a52.png)

1. Erstellen oder öffnen Sie eine vorhandene Smart-Kampagne und wählen Sie die Smart-Liste aus.

   ![](assets/image2016-7-25-16-3a9-3a19.png)

1. Suchen Sie nach dem benötigten Trigger und ziehen Sie ihn auf die Arbeitsfläche.

   ![](assets/image2016-7-25-16-3a16-3a43.png)

1. Wählen Sie das Attribut Trigger aus.

   ![](assets/image2016-7-25-16-3a21-3a42.png)

1. Optional können Sie eine Einschränkung festlegen.

   ![](assets/image2016-9-6-14-3a25-3a22.png)

1. Und da bist du. Die Änderung wird automatisch gespeichert.

   ![](assets/image2016-9-6-14-3a25-3a54.png)

   >[!NOTE]
   >
   >* [Erstellen einer Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
   >* [Grundlegendes zu benutzerdefinierten Marketo-Objekten](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

