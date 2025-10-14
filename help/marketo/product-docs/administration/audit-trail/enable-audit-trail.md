---
unique-page-id: 11382122
description: Audit-Protokoll aktivieren - Marketo-Dokumente - Produktdokumentation
title: Aktivieren des Audit-Protokolls
exl-id: 3ab2d7b2-1be1-4b3f-a9cc-d3edfa963679
feature: Audit Trail
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 4%

---

# Aktivieren des Audit-Protokolls {#enable-audit-trail}

Das Audit-Protokoll steht allen Kunden zur Verfügung und wird von zwei Administratorberechtigungen gesteuert.

>[!NOTE]
>
>Standardmäßig sind für alle Systemadministratorrollen beide Berechtigungen aktiviert.

## Audit-Protokoll für eine Rolle aktivieren {#enable-audit-trail-for-a-role}

1. Klicken Sie auf **[!UICONTROL Admin]**.

   ![](assets/enable-audit-trail-1.png)

1. Wählen Sie **[!UICONTROL Benutzer und Rollen]** aus und klicken Sie auf **[!UICONTROL Rollen]**.

   ![](assets/enable-audit-trail-2.png)

1. Wählen Sie die Rolle aus, für die Sie das Audit-Protokoll aktivieren möchten, und klicken Sie auf **[!UICONTROL Rolle bearbeiten]**.

   ![](assets/enable-audit-trail-3.png)

   >[!NOTE]
   >
   >Hier haben Sie auch die Möglichkeit, eine neue Rolle zu erstellen und ihr Zugriff auf das Audit-Protokoll zu gewähren.

1. Erweitern Sie die **[!UICONTROL Zugriff auf Admin]**-Berechtigung. Wählen Sie **[!UICONTROL Zugriffs-Audit]** Protokoll und/oder **[!UICONTROL Zugriffs-Anmeldeverlauf]** aus, je nach Ihren Anforderungen. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/enable-audit-trail-4.png)

   >[!NOTE]
   >
   >**Definition**
   >
   >**[!UICONTROL Zugriffs-Audit-Protokoll]**: Ermöglicht Benutzern Zugriff auf [!UICONTROL Asset-Audit-Protokoll] und [!UICONTROL Admin-Audit-Protokoll].
   >
   >**[!UICONTROL Zugriff auf Anmeldeverlauf]**: Ermöglicht Benutzern Zugriff auf [Benutzeranmeldeverlauf](/help/marketo/product-docs/administration/audit-trail/user-login-history.md).

## Audit-Protokoll-Rolle einem Benutzer zuweisen {#assign-audit-trail-role-to-a-user}

>[!PREREQUISITES]
>
>[Erstellen](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#create-a-role) oder [Aktivieren](#enable-audit-trail) einer vorhandenen Rolle, der Berechtigungen für das Audit-Protokoll erteilt werden.

1. Klicken **[!UICONTROL unter „Benutzer]** Rollen“ auf **[!UICONTROL Benutzer]**.

   ![](assets/enable-audit-trail-5.png)

1. Wählen Sie den Benutzer aus, dem Sie Zugriff auf das Audit-Protokoll gewähren möchten, und klicken Sie auf **[!UICONTROL Benutzer bearbeiten]**.

   ![](assets/enable-audit-trail-6.png)

   >[!NOTE]
   >
   >Dieser Prozess gilt auch, wenn Sie einen neuen Benutzer erstellen.

1. Wählen Sie die erstellten Audit-Protokoll-Rollen aus. In diesem Beispiel haben wir „Audit-Protokoll - Asset und Admin“ und „Audit-Protokoll - mit Anmeldeverlauf“ erstellt.

   ![](assets/enable-audit-trail-7.png)

   >[!CAUTION]
   >
   >Wenn Arbeitsbereiche aktiviert sind, aktivieren Sie das Kontrollkästchen der Rolle, wodurch alle Arbeitsbereiche ausgewählt werden. Wenn Sie die Auswahl eines einzelnen Arbeitsbereichs aufheben, wird das Audit-Protokoll ausgeblendet. Das bedeutet, dass Audit-Protokoll-Daten für jeden Arbeitsbereich angezeigt werden. Sie haben die Möglichkeit, Arbeitsbereiche beim [Filtern“ &#x200B;](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md).

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/enable-audit-trail-8.png)
