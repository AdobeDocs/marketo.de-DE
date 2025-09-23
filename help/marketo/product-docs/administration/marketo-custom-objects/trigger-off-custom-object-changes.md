---
unique-page-id: 11378713
description: Trigger von benutzerdefinierten Objektänderungen - Marketo-Dokumente - Produktdokumentation
title: Auslösen von Änderungen an benutzerdefinierten Objekten
exl-id: a2a3d82f-33ae-4191-b114-dbbf944a66c8
feature: Custom Objects
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 5%

---

# Auslösen von Änderungen an benutzerdefinierten Objekten {#trigger-off-custom-object-changes}

>[!NOTE]
>
>Diese Funktion ist nur verfügbar:
>
>* Zur Verwendung nur mit benutzerdefinierten Marketo-Objekten, nicht mit benutzerdefinierten Objekten, die über die native [!DNL Salesforce]- oder [!DNL Microsoft Dynamics]-Integration synchronisiert werden
>* Als Trigger, nicht als Filter
>
>Wenden Sie sich an den [Marketo](https://nation.marketo.com/t5/Support/ct-p/Support)Support, um die Trigger für benutzerdefinierte Objektänderungen zu aktivieren.

In der Smart-Liste einer Smart-Kampagne können Sie eine Flussaktion mit Trigger versehen, wenn ein benutzerdefiniertes Objekt einer Person oder einem Unternehmen hinzugefügt wird. Sie können auch eine Smart-Liste erstellen, die eine _Änderung_ in einem benutzerdefinierten Objekt als Trigger verwendet. Verwenden Sie sie beispielsweise, um eine E-Mail zu senden, wenn ein Kursname aktualisiert wird.

>[!NOTE]
>
>Wenn ein benutzerdefinierter Objektdatensatz geändert wird, wird kein Aktivitätsprotokolleintrag erstellt.

1. Navigieren Sie in Marketo Engage zu **[!UICONTROL Marketing-Aktivitäten]**.

   ![](assets/trigger-off-custom-object-changes-1.png)

1. Erstellen oder öffnen Sie eine vorhandene Smart-Kampagne und wählen Sie die Smart-Liste aus.

   ![](assets/trigger-off-custom-object-changes-2.png)

1. Suchen Sie nach dem gewünschten Trigger und ziehen Sie ihn auf die Arbeitsfläche.

   ![](assets/trigger-off-custom-object-changes-3.png)

1. Wählen Sie das Attribut [!UICONTROL Trigger &#x200B;].

   ![](assets/trigger-off-custom-object-changes-4.png)

1. Legen Sie optional eine Einschränkung fest.

   ![](assets/trigger-off-custom-object-changes-5.png)

1. Und hier sind sie. Die Änderung wird automatisch gespeichert.

   ![](assets/trigger-off-custom-object-changes-6.png)

   >[!NOTE]
   >
   >* [Erstellen einer Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
   >* [Grundlegendes zu benutzerdefinierten Marketo-Objekten](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
