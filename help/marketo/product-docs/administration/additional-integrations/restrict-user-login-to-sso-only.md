---
unique-page-id: 2360358
description: Einschränken der Benutzeranmeldung auf "Nur SSO"- Marketo-Dokumente - Produktdokumentation
title: Benutzeranmeldung auf SSO beschränken
exl-id: 74915871-dcf5-478d-a5ae-b20c3d2de553
feature: Administration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 7%

---

# Benutzeranmeldung auf SSO beschränken {#restrict-user-login-to-sso-only}

Wenn du [Verwendung von SSO](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md) und sicherstellen möchten, dass Benutzer die SSO-Sicherheit nicht umgehen können, befolgen Sie diese Anweisungen.

>[!IMPORTANT]
>
>Dieser Artikel gilt nicht für [Adobe IMS-fähig](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md) Marketo-Abonnements.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

1. Navigieren Sie zum **[!UICONTROL Admin]**-Bereich.

   ![](assets/restrict-user-login-to-sso-only-1.png)

1. Klicken **[!UICONTROL Anmeldeeinstellung]s**.

   ![](assets/restrict-user-login-to-sso-only-2.png)

1. Klicken **[!UICONTROL Sicherheitseinstellungen bearbeiten]**.

   ![](assets/restrict-user-login-to-sso-only-3.png)

1. Erweitern Sie die **[!UICONTROL Erweitert]** Einstellungen, überprüfen **[!UICONTROL SSO erforderlich]** und klicken Sie auf **[!UICONTROL Speichern]**.

![](assets/restrict-user-login-to-sso-only-4.png)

>[!NOTE]
>
>Es empfiehlt sich, die Benutzer einzuladen und die Einladung anzunehmen. _Nachher_ Wenn die Einladung angenommen wird, sollten Administratoren sie auf &quot;[!UICONTROL SSO erforderlich].&quot;

>[!TIP]
>
>Wenn Sie **[!UICONTROL SSO erforderlich]**, können Sie eine [Benutzerrolle](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) aus dieser Einschränkung durch Überprüfen der **[!UICONTROL Single Sign-on umgehen]** -Option beim Einrichten der Rolle. Auf diese Weise können sich Benutzer normal anmelden. Beispielsweise müssen sich Admin-Benutzer möglicherweise weiterhin über den Anmeldebildschirm bei Marketo anmelden.

>[!CAUTION]
>
>Wenn neue Benutzer eingeladen werden, erhalten sie Einladungs-E-Mails. Wenn **[!UICONTROL SSO erforderlich]** ausgewählt ist, werden diese E-Mails nur dann empfangen, wenn ihnen eine Rolle zugewiesen wurde, die auf **[!UICONTROL Single Sign-on umgehen]**.

Das ist es! Jetzt sind alle Benutzer (mit Ausnahme von Benutzern mit der Berechtigung, Single Sign-On zu umgehen) auf die Verwendung der SSO-Anmeldung beschränkt.

>[!MORELIKETHIS]
>
>* [Single Sign-On zu einem Portal hinzufügen](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Verwendung einer universellen ID zur Anmeldung von Abonnements](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [Einladen von Marketo-Benutzern zu zwei Instanzen mit universeller ID](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)
