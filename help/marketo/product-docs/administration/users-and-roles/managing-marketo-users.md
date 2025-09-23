---
unique-page-id: 2359906
description: Verwalten von Marketo-Benutzern - Marketo-Dokumente - Produktdokumentation
title: Verwalten von Marketo-Benutzenden
exl-id: 40506d3c-a7cb-45fb-bc10-021bd0c70806
feature: Users and Roles
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 2%

---

# Verwalten von Marketo-Benutzenden {#managing-marketo-users}

>[!IMPORTANT]
>
>Dieser Artikel ist nur für diejenigen gedacht, die {_}Marketo_ Adobe Identity verwenden[. ](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md){target="_blank"} Wenn Sie dies tun, befolgen Sie bitte die Schritte in [diesem Artikel](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"}.

## Benutzer erstellen {#create-users}

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/managing-marketo-users-1.png)

1. Klicken Sie auf **[!UICONTROL Benutzer und Rollen]**.

   ![](assets/managing-marketo-users-2.png)

1. Klicken Sie **[!UICONTROL Neuen Benutzer einladen]**.

   ![](assets/managing-marketo-users-3.png)

1. Geben Sie **[!UICONTROL E]**, **[!UICONTROL Vorname]** und **[!UICONTROL Nachname]** ein.

   ![](assets/managing-marketo-users-4.png)

1. Geben Sie optional einen Grund für die Einladung ein und wählen Sie mithilfe der Datumsauswahl ein **[!UICONTROL im Feld]** Zugriff läuft ab aus.

   ![](assets/managing-marketo-users-5.png)

1. Klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/managing-marketo-users-6.png)

   >[!TIP]
   >
   >Ein Ablaufdatum ist ideal für kurzfristige externe Stakeholder oder Berater, die nur für kurze Zeit Zugriff auf Marketo benötigen.

   >[!NOTE]
   >
   >Wenn das Ablaufdatum eintrifft, erhält der Benutzer eine Ablaufbenachrichtigung, und sein Konto wird gesperrt.

1. Wählen Sie **[!UICONTROL gewünschte]** aus und klicken Sie auf **[!UICONTROL Weiter]**.

   ![](assets/managing-marketo-users-7.png)

1. Nehmen Sie gegebenenfalls Änderungen an der Einladungsnachricht vor. Klicken Sie **Send**.

   ![](assets/managing-marketo-users-8.png)

   >[!NOTE]
   >
   >Die E-Mail-Adresse/Anmeldung muss eindeutig sein. Wenn Sie sie bereits in einer Sandbox-Instanz verwendet haben, müssen Sie in der Produktion eine andere verwenden und umgekehrt.

   ![](assets/managing-marketo-users-9.png)

   >[!NOTE]
   >
   >Einladungen laufen drei Tage nach dem Hinzufügen eines neuen Benutzers ab.

Der neue Benutzer wird jetzt auf der Registerkarte Benutzer aufgeführt und erhält eine E-Mail mit Anweisungen zum Aktivieren seines Kontos.

## Benutzer löschen {#delete-users}

>[!NOTE]
>
>Wenn der Benutzer, den Sie löschen möchten, auch ein Dynamic Chat-Benutzer ist, müssen Sie ihn [aus Dynamic Chat entfernen](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#remove-a-chat-user){target="_blank"} in der Admin Console löschen, bevor Sie ihn in Marketo Engage löschen können.

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/managing-marketo-users-10.png)

1. Klicken Sie auf **[!UICONTROL Benutzer und Rollen]**.

   ![](assets/managing-marketo-users-11.png)

1. Wählen Sie den Benutzer aus, den Sie entfernen möchten, und klicken Sie auf **[!UICONTROL Benutzer löschen]**.

   ![](assets/managing-marketo-users-12.png)

1. Bestätigen Sie mit **[!UICONTROL OK]**.

   ![](assets/managing-marketo-users-13.png)

## Zurücksetzen von Benutzerkennwörtern {#reset-user-passwords}

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/managing-marketo-users-14.png)

1. Klicken Sie auf **[!UICONTROL Benutzer und Rollen]**.

   ![](assets/managing-marketo-users-15.png)

1. Wählen Sie einen Benutzer aus und klicken Sie auf **[!UICONTROL Kennwort zurücksetzen]**.

   ![](assets/managing-marketo-users-16.png)

1. Klicken Sie auf **[!UICONTROL Schließen]**, um die Eingabeaufforderung zu schließen.

   ![](assets/managing-marketo-users-17.png)

Der Benutzer erhält eine E-Mail mit Anweisungen zum Zurücksetzen des Kennworts.

>[!TIP]
>
>Wenn die E-Mail nicht in ihrem Posteingang angezeigt wird, bitten Sie sie, ihren Junk-/Spam-Ordner zu überprüfen.

## Ändern von Berechtigungen und Bearbeiten von Benutzerinformationen {#change-permissions-and-edit-user-information}

1. Navigieren Sie zum Bereich **[!UICONTROL Admin]**.

   ![](assets/managing-marketo-users-18.png)

1. Klicken Sie auf **[!UICONTROL Benutzer und Rollen]**.

   ![](assets/managing-marketo-users-19.png)

1. Wählen Sie einen Benutzer aus und klicken Sie auf **[!UICONTROL Benutzer bearbeiten]**.

   ![](assets/managing-marketo-users-20.png)

1. Sie können Benutzerinformationen bearbeiten und die zugehörige Rolle ändern. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/managing-marketo-users-21.png)

>[!CAUTION]
>
>Wenn Sie der einzige Administrator in Marketo sind, dürfen Sie Ihre eigenen Administratorrechte nicht entfernen.

>[!NOTE]
>
>Wenn ein neuer Benutzer als Administrator eingeladen wird oder wenn ein Administrator gelöscht wird, erhalten alle aktuellen Administratoren eine E-Mail-Benachrichtigung.

Tolle Arbeit! Sie wissen jetzt, wie Sie einen Benutzer erstellen, einen Benutzer löschen, das Kennwort eines Benutzers zurücksetzen und Benutzer bearbeiten können.
