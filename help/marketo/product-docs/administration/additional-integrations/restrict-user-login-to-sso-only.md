---
unique-page-id: 2360358
description: Einschränken der Benutzeranmeldung auf "Nur SSO"- Marketo-Dokumente - Produktdokumentation
title: Benutzeranmeldung auf SSO beschränken
exl-id: 74915871-dcf5-478d-a5ae-b20c3d2de553
feature: Administration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 5%

---

# Benutzeranmeldung auf SSO beschränken {#restrict-user-login-to-sso-only}

Wenn Sie [SSO](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md) verwenden und sicherstellen möchten, dass Benutzer die SSO-Sicherheit nicht umgehen können, folgen Sie diesen Anweisungen.

>[!IMPORTANT]
>
>Dieser Artikel gilt nicht für [Adobe IMS-fähige](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md) Marketo-Abonnements.

>[!NOTE]
>
>**Erforderliche Administratorberechtigungen**

1. Wechseln Sie zum Bereich **[!UICONTROL Admin]** .

   ![](assets/restrict-user-login-to-sso-only-1.png)

1. Klicken Sie auf **[!UICONTROL Anmeldeeinstellung]s**.

   ![](assets/restrict-user-login-to-sso-only-2.png)

1. Klicken Sie auf **[!UICONTROL Sicherheitseinstellungen bearbeiten]**.

   ![](assets/restrict-user-login-to-sso-only-3.png)

1. Erweitern Sie die Einstellungen **[!UICONTROL Erweitert]** , aktivieren Sie die Option **[!UICONTROL SSO erforderlich]** und klicken Sie auf **[!UICONTROL Speichern]**.

![](assets/restrict-user-login-to-sso-only-4.png)

>[!NOTE]
>
>Es empfiehlt sich, die Benutzer einzuladen und die Einladung anzunehmen. _Nach_ der Annahme der Einladung sollten Administratoren sie dann auf &quot;[!UICONTROL SSO erforderlich]&quot;setzen.

>[!TIP]
>
>Wenn Sie **[!UICONTROL SSO erforderlich]** auswählen, können Sie eine [Benutzerrolle](/help/marketo/product-docs/administration/users-and-roles/create-delete-edit-and-change-a-user-role.md) aus dieser Einschränkung ausschließen, indem Sie beim Einrichten der Rolle die Option **[!UICONTROL Single Sign-On umgehen]** aktivieren. Auf diese Weise können sich Benutzer normal anmelden. Beispielsweise müssen sich Admin-Benutzer möglicherweise weiterhin über den Anmeldebildschirm bei Marketo anmelden.

>[!CAUTION]
>
>Wenn neue Benutzer eingeladen werden, erhalten sie Einladungs-E-Mails. Wenn jedoch **[!UICONTROL SSO erforderlich]** ausgewählt ist, erhalten diese E-Mails nicht, es sei denn, sie sind einer Rolle zugewiesen, die auf **[!UICONTROL Single Sign-On umgehen]** festgelegt ist.

Das ist es! Jetzt sind alle Benutzer (mit Ausnahme von Benutzern mit der Berechtigung, Single Sign-On zu umgehen) auf die Verwendung der SSO-Anmeldung beschränkt.

>[!MORELIKETHIS]
>
>* [Single Sign-On zu einem Portal hinzufügen](/help/marketo/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal.md)
>* [Verwenden einer universellen ID für die Anmeldung bei Abonnements](/help/marketo/product-docs/administration/settings/using-a-universal-id-for-subscription-login.md)
>* [Einladen von Marketo-Benutzern zu zwei Instanzen mit universeller ID](https://nation.marketo.com/t5/Knowledgebase/Inviting-Marketo-Users-to-Two-Instances-with-Universal-ID-UID/ta-p/251122)
