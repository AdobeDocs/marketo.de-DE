---
unique-page-id: 2359909
description: Verwalten von Benutzerrollen und Berechtigungen - Marketo-Dokumente - Produktdokumentation
title: Verwalten von Benutzerrollen und Berechtigungen
exl-id: e0213c5f-04e0-41a9-ac7b-873e2e39ac79
source-git-commit: a360b46ab1cd7149f609d139590124dcfcda8dad
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

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

Wenn Sie Marketo mit Adobe Identity verwenden, die Liste der Profilbeschreibungen [finden Sie hier .](/help/marketo/product-docs/administration/marketo-with-adobe-identity/overview.md#profile-levels).

## Rollen einem Benutzer zuweisen {#assign-roles-to-a-user}

Sie können Benutzern Rollen zuweisen, wenn Sie [Benutzer zum ersten Mal erstellen](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) oder [Bearbeiten eines vorhandenen Benutzers](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md).

1. Um einen vorhandenen Benutzer zu bearbeiten, navigieren Sie zu **Admin** und klicken Sie auf **Benutzer und Rollen**.

   ![](assets/image2014-9-9-18-3a7-3a32.png)

1. Wählen Sie in der Liste den Benutzer aus, den Sie bearbeiten möchten, und klicken Sie auf **Benutzer bearbeiten**.

   ![](assets/image2014-9-9-18-3a7-3a42.png)

1. under **Rollen**, wählen Sie die Rollen aus, die Sie dem Benutzer entsprechend den benötigten Berechtigungen zuweisen möchten, und klicken Sie auf **Speichern**.

   ![](assets/image2014-9-9-18-3a7-3a57.png)

   >[!NOTE]
   >
   >Informationen zu den einzelnen Rollen finden Sie unter  [Beschreibung der Rollenberechtigungen](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions/descriptions-of-role-permissions.md).

## Neue Rolle erstellen {#create-a-new-role}

Manchmal hat Ihr Unternehmen Mitarbeiter in sehr spezifischen Rollen, die eine benutzerdefinierte Kombination von Berechtigungen erfordern.

1. Um eine neue Benutzerrolle zu erstellen, gehen Sie zu &quot;Admin&quot;und klicken Sie auf **Benutzer und Rollen**.

   ![](assets/image2014-9-9-18-3a8-3a12.png)

1. Klicken Sie auf **Rollen** Registerkarte.

   ![](assets/image2014-9-9-18-3a8-3a22.png)

1. Klicken **Neue Rolle**.

   ![](assets/image2014-9-9-18-3a8-3a38.png)

1. Geben Sie einen **Rollenname**, **Beschreibung** (optional) und wählen Sie die Berechtigungen aus, die Benutzer mit dieser Rolle benötigen.

   ![](assets/image2014-9-9-18-3a9-3a3.png)

## Rolle bearbeiten {#edit-a-role}

Wenn Sie die Berechtigungen ändern müssen, die mit einer vorhandenen Rolle verknüpft sind, können Sie die Rolle bearbeiten.

1. Navigieren Sie zu **Admin** und klicken Sie auf **Benutzer und Rollen**.

   ![](assets/image2014-9-9-18-3a9-3a15.png)

1. Klicken Sie auf **Rollen** Registerkarte.

   ![](assets/image2014-9-9-18-3a9-3a26.png)

1. Wählen Sie in der Liste die Rolle aus, die Sie ändern möchten, und klicken Sie auf **Rolle bearbeiten**.

   ![](assets/image2014-9-9-18-3a9-3a40.png)

1. Ändern Sie die **Rollenname** und **Beschreibung** bei Bedarf und ändern Sie dann die Auswahl der zugehörigen **Berechtigungen**.

   ![](assets/image2014-9-9-18-3a10-3a3.png)

   >[!NOTE]
   >
   >Benutzer mit der von Ihnen bearbeiteten Rolle erhalten die geänderten Berechtigungen, nachdem sie sich abgemeldet und wieder angemeldet haben.

## Rolle löschen {#delete-a-role}

Wenn eine Rolle unnötig wird, können Sie sie löschen.

1. Navigieren Sie zu Admin und klicken Sie auf **Benutzer und Rollen**.

   ![](assets/image2014-9-9-18-3a10-3a15.png)

1. Klicken Sie auf **Rollen** Registerkarte.

   ![](assets/image2014-9-9-18-3a10-3a27.png)

1. Wählen Sie in der Liste die Rolle aus, die Sie löschen möchten, und klicken Sie auf **Rolle löschen**.

   ![](assets/image2014-9-9-18-3a10-3a39.png)

1. Klicken **Löschen** zur Bestätigung.

   ![](assets/image2014-9-9-18-3a10-3a50.png)
