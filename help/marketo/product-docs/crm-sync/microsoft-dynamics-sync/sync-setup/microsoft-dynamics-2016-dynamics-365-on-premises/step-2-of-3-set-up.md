---
description: Installieren von Marketo for [!DNL Microsoft Dynamics] 2016/[!DNL Dynamics] 365 On-Premise Schritt 2 von 3 - Dokumentation zu Marketo - Produktdokumentation
title: Installieren von Marketo for [!DNL Microsoft Dynamics] 2016/[!DNL Dynamics] 365 On-Premise Schritt 2 von 3
exl-id: c789b977-7ada-4f5d-8488-e1b58963f7e3
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 0%

---

# Schritt 2 von 3 Einrichten von Marketo for [!DNL Dynamics] (2016 On-Premise/[!DNL Dynamics] 365 On-Premise){#step-of-set-up-for-marketo-on-premises-2016}

Gute Arbeit beim Abschließen der vorherigen Schritte. Lassen Sie uns das immer wieder durchgehen.

>[!PREREQUISITES]
>
>[Installieren von Marketo for [!DNL Microsoft Dynamics] 2016/[!DNL Dynamics] 365 On-Premise, Schritt 1 von 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md)

## Neuen Benutzer erstellen {#create-a-new-user}

1. Melden Sie sich bei [!DNL Dynamics] an. Klicken Sie auf das Symbol Einstellungen und wählen Sie Erweiterte Einstellungen aus.

   ![](assets/step-2-of-3-marketo-on-premises-2016-1.png)

1. Klicken Sie **[!UICONTROL Einstellungen]** und wählen Sie **[!UICONTROL Sicherheit]** aus.

   ![](assets/step-2-of-3-marketo-on-premises-2016-2.png)

1. Klicken Sie auf **[!UICONTROL Benutzer]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-3.png)

1. Klicken Sie auf **[!UICONTROL Neu]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-4.png)

1. Klicken Sie **[!UICONTROL Benutzer hinzufügen und lizenzieren]**. Eine neue Registerkarte sollte geöffnet werden.

   ![](assets/step-2-of-3-marketo-on-premises-2016-5.png)

1. Klicken **[!UICONTROL oben]** der Seite auf „Admin“. Es sollte sich eine weitere neue Registerkarte öffnen.

   ![](assets/step-2-of-3-marketo-on-premises-2016-6.png)

1. Klicken Sie **[!UICONTROL Benutzer hinzufügen]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-7.png)

1. Geben Sie alle Ihre Informationen ein. Wenn Sie fertig sind, klicken Sie auf **[!UICONTROL Hinzufügen]**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-8.png)

   >[!NOTE]
   >
   >Dieser Name muss ein dedizierter Synchronisierungsbenutzer sein und nicht das Konto eines vorhandenen CRM-Benutzers. Es muss keine tatsächliche E-Mail-Adresse sein.

1. Geben Sie die E-Mail-Adresse ein, um die Anmeldeinformationen für den neuen Benutzer zu erhalten, und klicken Sie auf E-Mail senden und schließen.

   ![](assets/step-2-of-3-marketo-on-premises-2016-9.png)

## Neue Client-Anwendung erstellen {#create-a-new-client-application}

Führen Sie die Schritte in [diesem Artikel zu Microsoft](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/development/enabling-oauth-confidential-clients-with-ad-fs#create-an-application-group-in-ad-fs-2016-or-later) aus, um ein neues Client-Programm zu erstellen und Berechtigungen zu erteilen. Notieren Sie sich die Client-ID/den geheimen Schlüssel der [!DNL Dynamics]-Client-Anwendung.

## Assign Sync User Role {#assign-sync-user-role}

Weisen Sie die Rolle Marketo-Synchronisierungsbenutzer nur dem Marketo-Synchronisierungsbenutzer zu. Sie müssen sie keinem anderen Benutzer zuweisen.

>[!NOTE]
>
>Dies gilt für die Marketo-Version 4.0.0.14 und höher. Bei früheren Versionen müssen alle Benutzer über die Rolle „Benutzer synchronisieren“ verfügen. Informationen zum Upgrade Ihrer Marketo finden Sie unter [Upgrade der Marketo-Lösung für [!DNL Microsoft Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>Die Spracheinstellung des Synchronisierungsbenutzers [sollte auf Englisch festgelegt werden](https://learn.microsoft.com/en-us/power-platform/admin/enable-languages){target="_blank"}.

1. Klicken **[!UICONTROL unter „Einstellungen]** auf **[!UICONTROL Sicherheit]**.

   ![](assets/assign1.png)

1. Klicken Sie auf **[!UICONTROL Benutzer]**.

   ![](assets/assign2.png)

1. Hier wird eine Liste der Benutzer angezeigt. Wählen Sie den dedizierten Marketo-Synchronisierungsbenutzer aus oder wenden Sie sich an den Administrator [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} (ADFS), um einen dedizierten Benutzer für Marketo zu erstellen.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Wählen Sie den Synchronisierungsbenutzer aus. Klicken Sie **[!UICONTROL Rollen verwalten]**.

   ![](assets/assign4.png)

1. Markieren Sie Marketo Sync User und klicken Sie auf **[!UICONTROL OK]**.

   ![](assets/assign5.png)

   >[!TIP]
   >
   >Wenn Sie die Rolle nicht sehen, gehen Sie zurück zu [Schritt 1 von 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) und importieren Sie die Lösung.

   >[!NOTE]
   >
   >Alle Aktualisierungen, die der Synchronisierungsbenutzer in Ihrem CRM vorgenommen hat, _nicht_ wieder mit Marketo synchronisiert.

## Marketo-Lösung konfigurieren {#configure-marketo-solution}

Fast fertig! Wir haben nur noch ein paar letzte Konfigurationsschritte, bevor wir zum nächsten Artikel übergehen.

1. Klicken **[!UICONTROL unter „Einstellungen]** auf **[!UICONTROL Marketo Config]**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Wenn die Marketo-Konfiguration fehlt, versuchen Sie, die Seite zu aktualisieren. Wenn das Problem weiterhin besteht[ veröffentlichen Sie die Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md){target="_blank"}Lösung oder melden Sie sich ab und wieder an.

1. Klicken Sie auf **[!UICONTROL Standard]**.

   ![](assets/configure2.png)

1. Klicken Sie auf das Feld **[!UICONTROL Marketo-Benutzer]** und wählen Sie den Synchronisierungsbenutzer aus.

   ![](assets/configure3.png)

1. Klicken Sie auf das Symbol Speichern in der rechten unteren Ecke.

   ![](assets/configure4.png)

1. Klicken Sie **[!UICONTROL Alle Anpassungen veröffentlichen]**.

   ![](assets/publish-all-customizations1.png)

## Bevor Sie mit Schritt 3 fortfahren {#before-proceeding-to-step}

* Wenn Sie die Anzahl der zu synchronisierenden Datensätze einschränken möchten, richten [ jetzt einen benutzerdefinierten Synchronisierungsfilter ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md).
* Führen Sie den Prozess [validate [!DNL Microsoft Dynamics] sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) aus. Es stellt sicher, dass die anfänglichen Setups korrekt ausgeführt wurden.
* Melden Sie sich beim Marketo Sync User in [!DNL Microsoft Dynamics] CRM an.

>[!MORELIKETHIS]
>
>[Installieren von Marketo for [!DNL Microsoft Dynamics] 2016/[!DNL Dynamics] 365 On-Premise Schritt 3 von 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-3-of-3-connect.md)
