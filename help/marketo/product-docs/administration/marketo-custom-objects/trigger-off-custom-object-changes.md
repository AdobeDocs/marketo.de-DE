---
unique-page-id: 11378713
description: Verwendung benutzerdefinierter Objekte Hinzufügen oder Ändern von Triggern in einer Smart Campaign-Smart-Liste für benutzerdefinierte Marketo-Objekte mit Schritten zum Hinzufügen des Triggers und Festlegen von Einschränkungen.
title: Auslösen von Änderungen an benutzerdefinierten Objekten
exl-id: a2a3d82f-33ae-4191-b114-dbbf944a66c8
feature: Custom Objects
TQID: 'https://experienceleague.adobe.com/KjZuM-gPLIFa1umPF4pzN2OTak51i9I5TUcC7SacmZ8'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
subfeature_v2:
  - id: ea4e3ff5-e7b9-4b4c-a5a0-dc27cc3f4275
    internal-label: Custom objects
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 8%
---
# Auslösen von Änderungen an benutzerdefinierten Objekten {#trigger-off-custom-object-changes}

>[!NOTE]
>
>Diese Funktion ist nur verfügbar:
>
>* Zur Verwendung nur mit benutzerdefinierten Marketo-Objekten, nicht mit benutzerdefinierten Objekten, die über die native [!DNL Salesforce]- oder [!DNL Microsoft Dynamics]-Integration synchronisiert werden
>
>* Als Trigger, nicht als Filter
>
>Wenden Sie sich an den [Marketo](https://nation.marketo.com/t5/support/ct-p/Support?profile.language=de)Support, um die Trigger für benutzerdefinierte Objektänderungen zu aktivieren.

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

1. Die Änderung wird automatisch gespeichert.

   ![](assets/trigger-off-custom-object-changes-6.png)

   >[!NOTE]
   >
   >* [Erstellen einer Smart-Liste](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
   >* [Grundlegendes zu benutzerdefinierten Marketo-Objekten](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
