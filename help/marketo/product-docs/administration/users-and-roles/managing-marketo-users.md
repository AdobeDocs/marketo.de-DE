---
unique-page-id: 2359906
description: Verwalten von Marketo-Benutzern - Marketo-Dokumente - Produktdokumentation
title: Verwalten von Marketo-Benutzern
exl-id: 40506d3c-a7cb-45fb-bc10-021bd0c70806
feature: Users and Roles
source-git-commit: ab4358ac1d3e1aa1d3733fa5191c5d59022bdf9f
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Verwalten von Marketo-Benutzern {#managing-marketo-users}

>[!IMPORTANT]
>
>Dieser Artikel richtet sich nur an diejenigen, die _not_ use [Marketo mit Adobe Identity](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md){target="_blank"}. Wenn Sie dies tun, führen Sie die Schritte unter [diesem Artikel](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"}.

## Benutzer erstellen {#create-users}

1. Navigieren Sie zu **[!UICONTROL Admin]** Bereich.

   ![](assets/managing-marketo-users-1.png)

1. Klicks **[!UICONTROL Benutzer und Rollen]**.

   ![](assets/managing-marketo-users-2.png)

1. Klicks **[!UICONTROL Neuen Benutzer einladen]**.

   ![](assets/managing-marketo-users-3.png)

1. Geben Sie die **[!UICONTROL Email]**, **[!UICONTROL Vorname]**, und **[!UICONTROL Nachname]**.

   ![](assets/managing-marketo-users-4.png)

1. Geben Sie optional einen Grund für die Einladung ein und wählen Sie ein Ablaufdatum im **[!UICONTROL Zugriffsabläufe]** -Feld mithilfe der Datumsauswahl.

   ![](assets/managing-marketo-users-5.png)

1. Klicks **[!UICONTROL Nächste]**.

   ![](assets/managing-marketo-users-6.png)

   >[!TIP]
   >
   >Ein Ablaufdatum eignet sich hervorragend für kurzfristige externe Interessengruppen oder Berater, die nur für kurze Zeit Zugriff auf Marketo benötigen.

   >[!NOTE]
   >
   >Wenn das Ablaufdatum eintrifft, erhält der Benutzer eine Ablaufbenachrichtigung und sein Konto wird gesperrt.

1. Wählen Sie die **[!UICONTROL Rolle]** und klicken Sie auf **[!UICONTROL Nächste]**.

   ![](assets/managing-marketo-users-7.png)

1. Nehmen Sie bei Bedarf Änderungen an der Einladungsnachricht vor. Klicks **Siehend**.

   ![](assets/managing-marketo-users-8.png)

   >[!NOTE]
   >
   >Die E-Mail/Anmeldung muss eindeutig sein. Wenn Sie sie bereits in einer Sandbox-Instanz verwendet haben, müssen Sie eine andere in der Produktion verwenden und umgekehrt.

   ![](assets/managing-marketo-users-9.png)

   >[!NOTE]
   >
   >Einladungen laufen drei Tage nach dem Hinzufügen eines neuen Benutzers ab.

Der neue Benutzer wird jetzt im Tab Benutzer aufgelistet und erhält eine E-Mail mit Anweisungen zur Aktivierung seines Kontos.

## Benutzer löschen {#delete-users}

>[!NOTE]
>
>Wenn der Benutzer, den Sie löschen möchten, auch Dynamic Chat-Benutzer ist, müssen Sie [sie aus dem Dynamic Chat entfernen](/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#remove-a-chat-user){target="_blank"} in der Admin Console ein, bevor Sie sie im Marketo Engage löschen können.

1. Navigieren Sie zu **[!UICONTROL Admin]** Bereich.

   ![](assets/managing-marketo-users-10.png)

1. Klicks **[!UICONTROL Benutzer und Rollen]**.

   ![](assets/managing-marketo-users-11.png)

1. Wählen Sie den zu entfernenden Benutzer aus und klicken Sie auf **[!UICONTROL Benutzer löschen]**.

   ![](assets/managing-marketo-users-12.png)

1. Bestätigen durch Klicken auf **[!UICONTROL OK]**.

   ![](assets/managing-marketo-users-13.png)

## Zurücksetzen von Benutzerkennwörtern {#reset-user-passwords}

1. Navigieren Sie zu **[!UICONTROL Admin]** Bereich.

   ![](assets/managing-marketo-users-14.png)

1. Klicks **[!UICONTROL Benutzer und Rollen]**.

   ![](assets/managing-marketo-users-15.png)

1. Wählen Sie einen Benutzer aus und klicken Sie auf **[!UICONTROL Kennwort zurücksetzen]**.

   ![](assets/managing-marketo-users-16.png)

1. Klicks **[!UICONTROL Schließen]** , um die Eingabeaufforderung zu schließen.

   ![](assets/managing-marketo-users-17.png)

Der Benutzer erhält eine E-Mail mit Anweisungen zum Zurücksetzen des Kennworts.

>[!TIP]
>
>Wenn der Benutzer die E-Mail nicht in seinem Posteingang sieht, bitten Sie ihn, den Ordner &quot;Junk/Spam&quot;zu überprüfen.

## Berechtigungen ändern und Benutzerinformationen bearbeiten {#change-permissions-and-edit-user-information}

1. Navigieren Sie zu **[!UICONTROL Admin]** Bereich.

   ![](assets/managing-marketo-users-18.png)

1. Klicks **[!UICONTROL Benutzer und Rollen]**.

   ![](assets/managing-marketo-users-19.png)

1. Wählen Sie einen Benutzer aus und klicken Sie auf **[!UICONTROL Benutzer bearbeiten]**.

   ![](assets/managing-marketo-users-20.png)

1. Sie können Benutzerinformationen bearbeiten und die zugehörige Rolle ändern. Klicken Sie auf **[!UICONTROL Speichern]**.

   ![](assets/managing-marketo-users-21.png)

>[!CAUTION]
>
>Wenn Sie der einzige Administrator in Marketo sind, sollten Sie Ihre eigenen Administratorrechte nicht entfernen.

>[!NOTE]
>
>Wenn ein neuer Benutzer als Administrator eingeladen wird oder ein Administrator gelöscht wird, erhalten alle aktuellen Administratoren eine E-Mail-Benachrichtigung.

Fantastische Arbeit! Sie wissen jetzt, wie Sie einen Benutzer erstellen, einen Benutzer löschen, das Kennwort eines Benutzers zurücksetzen und Benutzer bearbeiten können.
