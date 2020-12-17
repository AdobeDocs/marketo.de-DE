---
unique-page-id: 2360358
description: Benutzeranmeldung auf "Nur SSO" beschränken - Marketing Docs - Produktdokumentation
title: Benutzeranmeldung auf "Nur SSO"beschränken
translation-type: tm+mt
source-git-commit: c33b7ab59e612f37d3f64bb954579700dc574068
workflow-type: tm+mt
source-wordcount: '167'
ht-degree: 0%

---


# Benutzeranmeldung auf &quot;Nur SSO&quot; beschränken {#restrict-user-login-to-sso-only}

Wenn Sie [SSO](add-single-sign-on-to-a-portal.md) verwenden und sicherstellen möchten, dass Benutzer die SSO-Sicherheit nicht umgehen können, befolgen Sie diese Anweisungen.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

1. Gehen Sie zu Admin und klicken Sie auf Anmeldeeinstellungen.

![](assets/image2014-9-24-14-3a44-3a40.png)

1. Klicken Sie auf Sicherheitseinstellungen bearbeiten.

   ![](assets/image2014-9-24-14-3a44-3a53.png)

1. Erweitern Sie die erweiterten Einstellungen, aktivieren Sie &quot;SSO erforderlich&quot;und klicken Sie auf &quot;Speichern&quot;.

![](assets/image2014-9-24-14-3a45-3a6.png)

>[!TIP]
>
>Wenn Sie **Einmalige Anmeldung erforderlich** auswählen, können Sie eine [Benutzerrolle](../../../product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) aus dieser Einschränkung ausschließen, indem Sie beim Einrichten der Rolle die Option **Einmaliges Anmelden umgehen** aktivieren. Auf diese Weise können Benutzer sich normal anmelden. So müssen sich Admin-Benutzer z. B. über den Anmeldebildschirm bei Marketo anmelden.

>[!CAUTION]
>
>Wenn neue Benutzer eingeladen werden, erhalten sie eine Einladungs-E-Mail. Wenn Sie jedoch **SSO** anfordern auswählen, erhalten diese E-Mails nur dann, wenn sie einer Rolle zugewiesen sind, die auf **Single-Sign-On umgehen** eingestellt ist.

Das ist&#39;s! Jetzt sind alle Benutzer (mit Ausnahme von Benutzern mit der Berechtigung, Single Sign-On zu umgehen) auf die Verwendung der einmaligen Anmeldung beschränkt.