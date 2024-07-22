---
unique-page-id: 11378713
description: Trigger von benutzerdefinierten Objektänderungen - Marketo Docs - Produktdokumentation
title: Trigger von benutzerdefinierten Objektänderungen
exl-id: a2a3d82f-33ae-4191-b114-dbbf944a66c8
feature: Custom Objects
source-git-commit: acaf2b421ed65f74bedf18b121ce54e30c19c721
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Trigger von benutzerdefinierten Objektänderungen {#trigger-off-custom-object-changes}

>[!NOTE]
>
>Diese Funktion ist nur verfügbar:
>
>* Nur für die Verwendung mit benutzerdefinierten Marketo-Objekten, nicht jedoch für benutzerdefinierte Objekte, die durch die native [!DNL Salesforce] - oder [!DNL Microsoft Dynamics] -Integration synchronisiert werden
>* Trigger, kein Filter
>
>Wenden Sie sich an den [Marketo-Support](https://nation.marketo.com/t5/Support/ct-p/Support) , damit benutzerdefinierte Trigger zur Objektänderung aktiviert sind.

In der Smart-Liste einer Smart-Kampagne können Sie eine Flow-Aktion Trigger haben, wenn ein benutzerdefiniertes Objekt zu einer Person oder einem Unternehmen hinzugefügt wird. Sie können auch eine Smart-Liste erstellen, die eine _change_ in einem benutzerdefinierten Objekt als Trigger verwendet. Beispielsweise können Sie damit eine E-Mail senden, wenn ein Kursname aktualisiert wird.

>[!NOTE]
>
>Ein Aktivitätsprotokolleintrag wird nicht erstellt, wenn ein benutzerdefinierter Objektdatensatz geändert wird.

1. Wechseln Sie unter Marketo Engage zu **[!UICONTROL Marketingaktivitäten]**.

   ![](assets/trigger-off-custom-object-changes-1.png)

1. Erstellen oder öffnen Sie eine vorhandene Smart-Kampagne und wählen Sie die Smart-Liste aus.

   ![](assets/trigger-off-custom-object-changes-2.png)

1. Suchen Sie nach dem benötigten Trigger und ziehen Sie ihn auf die Arbeitsfläche.

   ![](assets/trigger-off-custom-object-changes-3.png)

1. Wählen Sie das Attribut [!UICONTROL Trigger] aus.

   ![](assets/trigger-off-custom-object-changes-4.png)

1. Optional können Sie eine Einschränkung festlegen.

   ![](assets/trigger-off-custom-object-changes-5.png)

1. Und da bist du. Die Änderung wird automatisch gespeichert.

   ![](assets/trigger-off-custom-object-changes-6.png)

   >[!NOTE]
   >
   >* [Erstellen einer Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
   >* [Grundlegendes zu benutzerdefinierten Marketo-Objekten](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
