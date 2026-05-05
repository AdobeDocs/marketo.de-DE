---
unique-page-id: 2360358
description: SSO für alle Benutzer verlangen, damit sie die SSO-Sicherheit über die Admin-Anmeldeeinstellungen nicht umgehen können (gilt nicht für Adobe IMS).
title: Beschränken der Benutzeranmeldung auf SSO
exl-id: 74915871-dcf5-478d-a5ae-b20c3d2de553
feature: Administration
source-git-commit: 40f06a5391f2f7263bea0c5b8cefc1f3a607c68c
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 5%

---

# Beschränken der Benutzeranmeldung auf SSO {#restrict-user-login-to-sso-only}

Wenn Sie [SSO verwenden](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md) und sicherstellen möchten, dass Benutzer die SSO-Sicherheit nicht umgehen können, befolgen Sie diese Anweisungen.

>[!IMPORTANT]
>
>Dieser Artikel gilt nicht für Marketo[Abonnements mit aktiviertem &#x200B;](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md).

>[!NOTE]
>
>**Admin-Berechtigungen erforderlich**

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/restrict-user-login-to-sso-only-1.png)

1. Klicken Sie **[!UICONTROL Anmeldeeinstellungen]**.

   ![](assets/restrict-user-login-to-sso-only-2.png)

1. Klicken Sie **[!UICONTROL Sicherheitseinstellungen bearbeiten]**.

   ![](assets/restrict-user-login-to-sso-only-3.png)

1. Erweitern Sie **[!UICONTROL Erweitert]**, aktivieren Sie **[!UICONTROL SSO erforderlich]** und klicken Sie auf **[!UICONTROL Speichern]**.

![](assets/restrict-user-login-to-sso-only-4.png)

>[!NOTE]
>
>Es empfiehlt sich, die Benutzer einzuladen und die Einladung anzunehmen. _Nachdem_ Einladung angenommen wurde, sollten Administratoren sie auf &quot;[!UICONTROL SSO erforderlich“ &#x200B;].

>[!TIP]
>
>Wenn Sie **[!UICONTROL SSO erforderlich]** auswählen, können Sie eine [Benutzerrolle](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) von dieser Einschränkung ausschließen, indem Sie die Option **[!UICONTROL Einmaliges Anmelden umgehen]** beim Einrichten der Rolle aktivieren. Dadurch können sich Benutzer normal anmelden. Beispielsweise müssen sich Administratorbenutzer möglicherweise weiterhin über den Anmeldebildschirm bei Marketo anmelden. Wenn sowohl SSO als auch universelle ID aktiviert sind, müssen Sie die Berechtigung zum Umgehen von Single Sign-On besitzen, um zwischen Abonnements umzuschalten.

>[!CAUTION]
>
>Wenn neue Benutzer eingeladen werden, erhalten sie Einladungs-E-Mails. Wenn jedoch **[!UICONTROL SSO erforderlich]** ausgewählt ist, erhalten diese E-Mails nicht, es sei denn, sie wurden einer Rolle zugewiesen, die auf **[!UICONTROL Single Sign-On umgehen]** festgelegt ist.

Jetzt sind alle Benutzer (mit Ausnahme der Benutzer mit der Berechtigung, Single Sign-on zu umgehen) auf die ausschließliche Verwendung der SSO-Anmeldung beschränkt.

>[!MORELIKETHIS]
>
>* [Hinzufügen von Single Sign-on zu einem Portal](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Einladen von Marketo-Benutzern zu zwei Instanzen mit universeller ID](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)
