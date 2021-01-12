---
unique-page-id: 11382122
description: Audit-Protokoll - Marketing-Dokumente - Produktdokumentation aktivieren
title: Prüfpfad aktivieren
translation-type: tm+mt
source-git-commit: 78961a3e163ce903facf955a9dda6909b5e85bad
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---


# Audit-Protokoll {#enable-audit-trail} aktivieren

Prüfpfad steht allen Kunden zur Verfügung und wird durch zwei Administratorberechtigungen gesteuert.

>[!NOTE]
>
>Standardmäßig sind für alle Systemadministratorrollen beide Berechtigungen aktiviert.

## Prüfpfad für eine Rolle {#enable-audit-trail-for-a-role} aktivieren

1. Klicken Sie auf **Admin**.

   ![](assets/one-2.png)

1. Wählen Sie **Benutzer und Rollen** und klicken Sie auf **Rollen**.

   ![](assets/two-2.png)

1. Wählen Sie die Rolle, für die Sie den Prüfpfad aktivieren möchten, und klicken Sie auf **Rolle bearbeiten**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Sie haben hier auch die Möglichkeit, eine neue Rolle zu erstellen und ihr den Audit-Protokoll-Zugriff zu gewähren.

1. Erweitern Sie die Berechtigung **Zugriff auf Admin**. Wählen Sie **Zugriffsprüfungsprotokoll** und/oder **Zugriffsanmeldeverlauf** je nach Ihren Anforderungen. Klicken Sie auf **Speichern**.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >**Definition**
   >
   >**Zugriffsprüfungsprotokoll:** Ermöglicht Benutzern Zugriff auf den Asset-Prüfpfad und den Admin-Prüfpfad.
   >
   >**Anmeldeverlauf aufrufen:** Ermöglicht Benutzern Zugriff auf den  [Anmeldeverlauf](/help/marketo/product-docs/administration/audit-trail/user-login-history.md).

## Prüfprotokoll-Rolle einem Benutzer {#assign-audit-trail-role-to-a-user} zuweisen

>[!PREREQUISITES]
>
>[](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md#create-a-role) Erstellen oder  [](#enable-audit-trail) aktivieren Sie eine vorhandene Rolle, wobei Sie ihr die Berechtigung &quot;Prüfpfad&quot;zuweisen.

1. Klicken Sie unter **Benutzer und Rollen** auf **Benutzer**.

   ![](assets/five-1.png)

1. Wählen Sie den Benutzer aus, auf den Sie Audit Trail zugreifen möchten, und klicken Sie auf **Benutzer bearbeiten**.

   ![](assets/six-1.png)

   >[!NOTE]
   >
   >Dieser Vorgang gilt auch, wenn Sie einen neuen Benutzer erstellen.

1. Wählen Sie die von Ihnen erstellten Audit-Trail-Rollen aus. In diesem Beispiel haben wir &quot;Prüfpfad - Asset und Admin&quot;und &quot;Prüfpfad - mit Anmeldeverlauf&quot;erstellt.

   ![](assets/seven-1.png)

   >[!CAUTION]
   >
   >Wenn Sie Arbeitsbereiche aktiviert haben, aktivieren Sie das Kontrollkästchen der Rolle, in dem alle Arbeitsbereiche ausgewählt werden. Wenn Sie eine einzelne Arbeitsfläche deaktivieren, wird der Prüfpfad ausgeblendet. Dies bedeutet, dass Sie Audit-Trail-Daten für jeden Arbeitsbereich sehen. Sie haben die Möglichkeit, Arbeitsflächen auszublenden, wenn [filter](/help/marketo/product-docs/administration/audit-trail/filtering-in-audit-trail.md).

1. Klicken Sie auf **Speichern**.

   ![](assets/eight-1.png)
