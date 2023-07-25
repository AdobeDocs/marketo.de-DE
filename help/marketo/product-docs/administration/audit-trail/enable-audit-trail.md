---
unique-page-id: 11382122
description: Audit-Protokoll aktivieren - Marketo-Dokumente - Produktdokumentation
title: Audit-Protokoll aktivieren
exl-id: 3ab2d7b2-1be1-4b3f-a9cc-d3edfa963679
feature: Audit Trail
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# Audit-Protokoll aktivieren {#enable-audit-trail}

Audit-Protokoll ist für alle Kunden verfügbar und wird von zwei Administratorberechtigungen gesteuert.

>[!NOTE]
>
>Standardmäßig sind für alle Systemadministratorrollen beide Berechtigungen aktiviert.

## Audit-Protokoll für eine Rolle aktivieren {#enable-audit-trail-for-a-role}

1. Klicken **[!UICONTROL Admin]**.

   ![](assets/enable-audit-trail-1.png)

1. Auswählen **[!UICONTROL Benutzer und Rollen]** und klicken Sie auf **[!UICONTROL Rollen]**.

   ![](assets/enable-audit-trail-2.png)

1. Wählen Sie die Rolle aus, für die Sie das Audit-Protokoll aktivieren möchten, und klicken Sie auf **[!UICONTROL Rolle bearbeiten]**.

   ![](assets/enable-audit-trail-3.png)

   >[!NOTE]
   >
   >Sie können hier auch eine neue Rolle erstellen und ihr den Audit-Protokoll-Zugriff gewähren.

1. Erweitern Sie die **[!UICONTROL Auf Admin zugreifen]** Berechtigung. Auswählen **[!UICONTROL Audit-Protokoll aufrufen]** und/oder **[!UICONTROL Anmeldeverlauf aufrufen]**, entsprechend Ihren Anforderungen. Klicken **[!UICONTROL Speichern]**.

   ![](assets/enable-audit-trail-4.png)

   >[!NOTE]
   >
   >**Definition**
   >
   >**[!UICONTROL Audit-Protokoll aufrufen]**: Gewährt Benutzern Zugriff auf beide [!UICONTROL Asset-Audit-Protokoll] und [!UICONTROL Admin-Audit-Protokoll].
   >
   >**[!UICONTROL Anmeldeverlauf aufrufen]**: Gewährt Benutzern Zugriff auf [Anmeldeverlauf für Benutzer](/help/marketo/product-docs/administration/audit-trail/user-login-history.md).

## Zuweisen einer Audit-Protokollrolle zu einem Benutzer {#assign-audit-trail-role-to-a-user}

>[!PREREQUISITES]
>
>[Erstellen](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#create-a-role) oder [enable](#enable-audit-trail) eine vorhandene Rolle, die ihr Audit-Protokoll-Berechtigungen erteilt.

1. In **[!UICONTROL Benutzer und Rollen]** klicken **[!UICONTROL Benutzer]**.

   ![](assets/enable-audit-trail-5.png)

1. Wählen Sie den Benutzer aus, auf den Sie Audit Trail Zugriff gewähren möchten, und klicken Sie auf **[!UICONTROL Benutzer bearbeiten]**.

   ![](assets/enable-audit-trail-6.png)

   >[!NOTE]
   >
   >Dieser Prozess gilt auch bei der Erstellung eines neuen Benutzers.

1. Wählen Sie die von Ihnen erstellten Audit-Protokoll-Rollen aus. In diesem Beispiel haben wir &quot;Audit-Protokoll - Asset und Admin&quot;und &quot;Audit-Protokoll - mit Anmeldeverlauf&quot;erstellt.

   ![](assets/enable-audit-trail-7.png)

   >[!CAUTION]
   >
   >Wenn Sie Arbeitsbereiche aktiviert haben, aktivieren Sie das Kontrollkästchen der Rolle, mit dem alle Arbeitsbereiche ausgewählt werden. Wenn Sie die Auswahl eines einzelnen Arbeitsbereichs aufheben, wird das Audit-Protokoll ausgeblendet. Das bedeutet, dass Sie Audit-Protokolldaten für jeden Arbeitsbereich sehen. Sie haben die Möglichkeit, Arbeitsbereiche auszublenden, wenn [Filter](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md).

1. Klicken **[!UICONTROL Speichern]**.

   ![](assets/enable-audit-trail-8.png)
