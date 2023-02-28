---
unique-page-id: 2359909
description: Verwalten von Benutzerrollen und Berechtigungen - Marketo-Dokumente - Produktdokumentation
title: Verwalten von Benutzerrollen und Berechtigungen
exl-id: e0213c5f-04e0-41a9-ac7b-873e2e39ac79
source-git-commit: 3bb7e8155491f810cc0e71637482e6da788dc068
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 4%

---

# Verwalten von Benutzerrollen und Berechtigungen {#managing-user-roles-and-permissions}

Legen Sie Benutzerrollen fest, erstellen und bearbeiten Sie sie und weisen Sie sie Benutzern zu. Auf diese Weise können Sie die Bereiche und Funktionen steuern, auf die jeder Marketo-Benutzer Zugriff hat.

Beispielsweise benötigt ein Marketing-Benutzer in der Regel einen umfassenden Zugriff auf die gesamte Anwendung, um E-Mails, Landingpages und Programme zu erstellen, zu ändern und bereitzustellen. Ein Webdesigner hingegen verbringt fast die ganze Zeit in Design Studio und erstellt Assets zur Verwendung in E-Mails und Landingpages. Und obwohl Unternehmensführer die Marketo-Berichte im Bereich Analytics umfassend nutzen, müssen sie die Assets oder Programme möglicherweise nicht selbst erstellen oder vorantreiben.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

Marketo bietet mehrere integrierte Rollen mit unterschiedlichen Zugriffsstufen:

* **Admin** - alle Teile der Anwendung, einschließlich des Administratorabschnitts
* **Standardbenutzer** - alle Teile der Anwendung mit Ausnahme des Administratorabschnitts
* **Marketing-Benutzer** - alle Teile der Anwendung mit Ausnahme des Administratorabschnitts
* **Web Designer** - nur Design Studio
* **Analytics-Benutzer** - nur der Analytics-Abschnitt

Sie können die Rollen &quot;Admin&quot;und &quot;Standardbenutzer&quot;nicht bearbeiten, die anderen können jedoch bearbeitet werden. Sie können auch neue benutzerdefinierte Rollen erstellen, die den jeweiligen Organisationsstrukturen in Ihrem Unternehmen entsprechen.

## Marketo mit Adobe Identity {#marketo-with-adobe-identity}

Wenn Sie Marketo mit Adobe Identity verwenden, die Liste der Profilbeschreibungen [finden Sie hier .](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md#profile-levels).

## Rollen einem Benutzer zuweisen {#assign-roles-to-a-user}

Sie können Benutzern Rollen zuweisen, wenn Sie [Benutzer zum ersten Mal erstellen](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) oder [Bearbeiten eines vorhandenen Benutzers](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md).

1. Navigieren Sie zum **Admin**-Bereich.

   ![](assets/managing-user-roles-and-permissions-1.png)

1. Klicken **Benutzer und Rollen**.

   ![](assets/managing-user-roles-and-permissions-2.png)

1. Wählen Sie in der Liste den Benutzer aus, den Sie bearbeiten möchten, und klicken Sie auf **Benutzer bearbeiten**.

   ![](assets/managing-user-roles-and-permissions-3.png)

1. under **Rollen**, wählen Sie die Rollen aus, die Sie dem Benutzer entsprechend den benötigten Berechtigungen zuweisen möchten, und klicken Sie auf **Speichern**.

   ![](assets/managing-user-roles-and-permissions-4.png)

   >[!NOTE]
   >
   >Informationen zu den einzelnen Rollen finden Sie unter  [Beschreibung der Rollenberechtigungen](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions/descriptions-of-role-permissions.md).

## Neue Rolle erstellen {#create-a-new-role}

Manchmal hat Ihr Unternehmen Mitarbeiter in sehr spezifischen Rollen, die eine benutzerdefinierte Kombination von Berechtigungen erfordern.

1. Navigieren Sie zum **Admin**-Bereich.

   ![](assets/managing-user-roles-and-permissions-5.png)

1. Klicken **Benutzer und Rollen**.

   ![](assets/managing-user-roles-and-permissions-6.png)

1. Klicken Sie auf **Rollen** Registerkarte.

   ![](assets/managing-user-roles-and-permissions-7.png)

1. Klicken **Neue Rolle**.

   ![](assets/managing-user-roles-and-permissions-8.png)

1. Geben Sie einen **Rollenname**, **Beschreibung** (optional) und wählen Sie die Berechtigungen aus, die Benutzer mit dieser Rolle benötigen.

   ![](assets/managing-user-roles-and-permissions-9.png)

## Rolle bearbeiten {#edit-a-role}

Wenn Sie die Berechtigungen ändern müssen, die mit einer vorhandenen Rolle verknüpft sind, können Sie die Rolle bearbeiten.

1. Navigieren Sie zum **Admin**-Bereich.

   ![](assets/managing-user-roles-and-permissions-10.png)

1. Klicken **Benutzer und Rollen**.

   ![](assets/managing-user-roles-and-permissions-11.png)

1. Klicken Sie auf **Rollen** Registerkarte.

   ![](assets/managing-user-roles-and-permissions-12.png)

1. Wählen Sie in der Liste die Rolle aus, die Sie ändern möchten, und klicken Sie auf **Rolle bearbeiten**.

   ![](assets/managing-user-roles-and-permissions-13.png)

1. Ändern Sie die **Rollenname** und **Beschreibung** bei Bedarf und ändern Sie dann die Auswahl der zugehörigen **Berechtigungen**.

   ![](assets/managing-user-roles-and-permissions-14.png)

   >[!NOTE]
   >
   >Benutzer mit der von Ihnen bearbeiteten Rolle erhalten die geänderten Berechtigungen, nachdem sie sich abgemeldet und wieder angemeldet haben.

## Rolle löschen {#delete-a-role}

Wenn eine Rolle unnötig wird, können Sie sie löschen.

1. Navigieren Sie zum **Admin**-Bereich.

   ![](assets/managing-user-roles-and-permissions-15.png)

1. Klicken **Benutzer und Rollen**.

   ![](assets/managing-user-roles-and-permissions-16.png)

1. Klicken Sie auf **Rollen** Registerkarte.

   ![](assets/managing-user-roles-and-permissions-17.png)

1. Wählen Sie in der Liste die Rolle aus, die Sie löschen möchten, und klicken Sie auf **Rolle löschen**.

   ![](assets/managing-user-roles-and-permissions-18.png)

1. Klicken **Löschen** zur Bestätigung.

   ![](assets/managing-user-roles-and-permissions-19.png)
