---
unique-page-id: 2360327
description: Wie man Zuweisungsregeln einrichtet, um Personen aus dem CRM in die richtigen Personenpartitionen zu leiten.
title: Zuweisen von Personen-Partitionen mit Zuweisungsregeln
exl-id: 6b54dcb7-8da9-466b-b153-099ebcb96424
feature: Partitions
TQID: https://experienceleague.adobe.com/7e7A0wXFiKVttSm7BXEJYtVBnSW6qAah1ygNqO4qdr0
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 170
ht-degree: 10%

---

# Zuweisen von Personen-Partitionen mit Zuweisungsregeln {#assigning-person-partitions-with-assignment-rules}

>[!NOTE]
>
>**Admin-Berechtigungen erforderlich**

>[!PREREQUISITES]
>
>[Erstellen einer Personenpartition](/help/marketo/product-docs/administration/workspaces-and-person-partitions/create-a-person-partition.md)

Richten Sie bei der Verwendung von Personenpartitionen Zuweisungsregeln ein, um Personen, die aus Ihrem CRM erstellt wurden, zu ihren jeweiligen Partitionen weiterzuleiten.

>[!NOTE]
>
>Auf Personen, die in Marketo aus Ihrem CRM und über die SOAP-API erstellt wurden, werden Zuweisungsregeln angewendet.

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-1.png)

1. Klicken Sie **[!UICONTROL Arbeitsbereiche und Partitionen]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-2.png)

1. Klicken Sie auf **[!UICONTROL Registerkarte]** Personenpartitionen“ auf **[!UICONTROL Zuweisungsregeln]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-3.png)

1. Klicken Sie **[!UICONTROL Auswahl hinzufügen]**, um Bedingungen für das Routing von Personen in Personenpartitionen hinzuzufügen.

   ![](assets/assigning-person-partitions-with-assignment-rules-4.png)

1. Wählen Sie das Feld aus, auf dem die Bedingung erstellt werden soll.

   ![](assets/assigning-person-partitions-with-assignment-rules-5.png)

1. Wählen Sie den Auswahloperator aus und geben Sie einen Wert ein.

   ![](assets/assigning-person-partitions-with-assignment-rules-6.png)

1. Wählen Sie die Personenpartition aus, in die die Personen, die die Bedingungen erfüllen, aufgenommen werden sollen.

   ![](assets/assigning-person-partitions-with-assignment-rules-7.png)

   >[!NOTE]
   >
   >Sie können beliebig viele Optionen hinzufügen.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/assigning-person-partitions-with-assignment-rules-8.png)

Die Zuweisungsregeln für die Personenpartitionen wurden konfiguriert.

>[!NOTE]
>
>Die Standardauswahl wird angewendet, wenn keine der vorherigen Bedingungen erfüllt ist.
