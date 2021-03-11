---
unique-page-id: 2360358
description: Benutzeranmeldung auf "Nur SSO" beschränken - Marketing Docs - Produktdokumentation
title: Benutzeranmeldung auf "Nur SSO"beschränken
translation-type: tm+mt
source-git-commit: a7c90193e5c934119fa3b6bdf864d1458d1aad7c
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---


# Benutzeranmeldung auf &quot;Nur SSO&quot; beschränken {#restrict-user-login-to-sso-only}

Wenn Sie [SSO](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md) verwenden und sicherstellen möchten, dass Benutzer die SSO-Sicherheit nicht umgehen können, befolgen Sie diese Anweisungen.

>[!NOTE]
>
>**Administratorberechtigungen erforderlich**

1. Gehen Sie zu **Admin** und klicken Sie auf **Anmeldeeinstellungen**.

   ![](assets/image2014-9-24-14-3a44-3a40.png)

1. Klicken Sie auf **Sicherheitseinstellungen bearbeiten**.

   ![](assets/image2014-9-24-14-3a44-3a53.png)

1. Erweitern Sie die erweiterten Einstellungen, aktivieren Sie **SSO** erforderlich und klicken Sie auf **Speichern**.

![](assets/image2014-9-24-14-3a45-3a6.png)

>[!NOTE]
>
>Es empfiehlt sich, den/die Benutzer einzuladen und die Einladung anzunehmen. _Nachdem_ die Einladung angenommen wurde, sollten Administratoren sie auf &quot;Einladung erforderlich&quot;setzen.

>[!TIP]
>
>Wenn Sie **Einmalige Anmeldung erforderlich** auswählen, können Sie eine [Benutzerrolle](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) aus dieser Einschränkung ausschließen, indem Sie beim Einrichten der Rolle die Option **Einmaliges Anmelden umgehen** aktivieren. Auf diese Weise können Benutzer sich normal anmelden. So müssen sich Admin-Benutzer z. B. über den Anmeldebildschirm bei Marketo anmelden.

>[!CAUTION]
>
>Wenn neue Benutzer eingeladen werden, erhalten sie eine Einladungs-E-Mail. Wenn Sie jedoch **SSO** anfordern auswählen, erhalten diese E-Mails nur dann, wenn sie einer Rolle zugewiesen sind, die auf **Single-Sign-On umgehen** eingestellt ist.

Das ist&#39;s! Jetzt sind alle Benutzer (mit Ausnahme von Benutzern mit der Berechtigung, Single Sign-On zu umgehen) auf die Verwendung der einmaligen Anmeldung beschränkt.

>[!MORELIKETHIS]
>
>* [hinzufügen Einmal-Anmeldung bei einem Portal](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Verwenden einer universellen ID für die Abonnement-Anmeldung](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [Einladen von Marketing-Benutzern zu zwei Instanzen mit universeller ID](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)

