---
description: Installieren von Marketo für Microsoft Dynamics 2016/Dynamics 365 On-Premises Schritt 2 von 3 - Marketo Docs - Produktdokumentation
title: Installieren von Marketo für Microsoft Dynamics 2016/Dynamics 365 On-Premises Schritt 2 von 3
exl-id: c789b977-7ada-4f5d-8488-e1b58963f7e3
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# Schritt 2 von 3 Einrichten von Marketo für Dynamics (On-Premises 2016/Dynamics 365 On-Premises){#step-of-set-up-for-marketo-on-premises-2016}

Große Arbeit zum Abschluss der vorherigen Schritte. Lasst uns das durchgehen.

>[!PREREQUISITES]
>
>[Installieren von Marketo für Microsoft Dynamics 2016/Dynamics 365 On-Premises Schritt 1 von 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md)

## Neuen Benutzer erstellen {#create-a-new-user}

1. Melden Sie sich bei Dynamics an. Klicken Sie auf das Symbol Einstellungen und wählen Sie Erweiterte Einstellungen aus.

   ![](assets/step-2-of-3-marketo-on-premises-2016-1.png)

1. Klicks **Einstellungen** und wählen **Sicherheit**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-2.png)

1. Klicks **Benutzer**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-3.png)

1. Klicks **Neu**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-4.png)

1. Klicks **Hinzufügen und Lizenzieren von Benutzern**. Eine neue Registerkarte sollte geöffnet werden.

   ![](assets/step-2-of-3-marketo-on-premises-2016-5.png)

1. Klicks **Admin** oben auf der Seite. Eine neue Registerkarte sollte geöffnet werden.

   ![](assets/step-2-of-3-marketo-on-premises-2016-6.png)

1. Klicks **Benutzer hinzufügen**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-7.png)

1. Geben Sie alle Ihre Informationen ein. Wenn Sie fertig sind, klicken Sie auf **Hinzufügen**.

   ![](assets/step-2-of-3-marketo-on-premises-2016-8.png)

   >[!NOTE]
   >
   >Dieser Name muss ein dedizierter Synchronisierungsbenutzer und nicht das Konto eines vorhandenen CRM-Benutzers sein. Es muss sich nicht um eine tatsächliche E-Mail-Adresse handeln.

1. Geben Sie die E-Mail ein, um die neuen Benutzeranmeldeinformationen zu erhalten, klicken Sie auf E-Mail senden und schließen.

   ![](assets/step-2-of-3-marketo-on-premises-2016-9.png)

## Neue Client-Anwendung erstellen {#create-a-new-client-application}

Führen Sie die Schritte unter [diesem Microsoft-Artikel](https://docs.microsoft.com/en-us/windows-server/identity/ad-fs/development/enabling-oauth-confidential-clients-with-ad-fs#create-an-application-group-in-ad-fs-2016-or-later) , um eine neue Client-Anwendung zu erstellen und Berechtigungen zu erteilen. Beachten Sie die Client-ID/das Geheimnis der Dynamics Client-Anwendung.

## Benutzerrolle &quot;Synchronisierung zuweisen&quot; {#assign-sync-user-role}

Weisen Sie die Benutzerrolle &quot;Marketo Sync User&quot;nur dem Marketo-Synchronisierungsbenutzer zu. Sie müssen sie keinen anderen Benutzern zuweisen.

>[!NOTE]
>
>Dies gilt für die Marketo-Version 4.0.0.14 und höher. Bei früheren Versionen müssen alle Benutzer über die Benutzerrolle &quot;Synchronisieren&quot;verfügen. Informationen zum Upgrade Ihrer Marketo finden Sie unter [Upgrade der Marketo-Lösung für Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/update-the-marketo-solution-for-microsoft-dynamics.md).

>[!IMPORTANT]
>
>Die Spracheinstellung des Synchronisierungsbenutzers [sollte auf Englisch eingestellt sein](https://portal.dynamics365support.com/knowledgebase/article/KA-01201/en-us).

1. under **Einstellungen** klicken **Sicherheit**.

   ![](assets/assign1.png)

1. Klicks **Benutzer**.

   ![](assets/assign2.png)

1. Hier sehen Sie eine Liste der Benutzer. Wählen Sie den dedizierten Marketo Sync-Benutzer aus oder kontaktieren Sie Ihren [Active Directory Federation-Dienste](https://msdn.microsoft.com/en-us/library/bb897402.aspx)(ADFS) Administrator, um einen dedizierten Benutzer für Marketo zu erstellen.

   ![](assets/image2015-3-26-10-3a39-3a35.png)

1. Wählen Sie den Synchronisierungsbenutzer aus. Klicks **Rollen verwalten**.

   ![](assets/assign4.png)

   Markieren Sie Marketo Sync User und klicken Sie auf OK.

   ![](assets/assign5.png)

   >[!TIP]
   >
   >Wenn die Rolle nicht angezeigt wird, gehen Sie zurück zu [Schritt 1 von 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) und importieren Sie die Lösung.

   >[!NOTE]
   >
   >Alle vom Synchronisierungsbenutzer in Ihrem CRM-System vorgenommenen Aktualisierungen werden **not** wieder mit Marketo synchronisiert werden.

## Konfigurieren der Marketo-Lösung {#configure-marketo-solution}

Fast fertig! Wir haben nur einige letzte Konfigurationsschritte, bevor wir zum nächsten Artikel übergehen.

1. under **Einstellungen** klicken **Marketo-Konfiguration**.

   ![](assets/configure1.png)

   >[!NOTE]
   >
   >Wenn die Marketo-Konfiguration fehlt, versuchen Sie, die Seite zu aktualisieren. Wenn das Problem weiterhin besteht, [Marketo-Lösung veröffentlichen](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-1-of-3-install.md) oder versuchen Sie, sich ab- und wieder anzumelden.

1. Klicks **Standard**.

   ![](assets/configure2.png)

1. Klicken Sie auf **Marketo-Benutzer** und wählen Sie den Synchronisierungsbenutzer aus.

   ![](assets/configure3.png)

1. Klicken Sie unten rechts auf das Symbol Speichern .

   ![](assets/configure4.png)

1. Klicks **Alle Anpassungen veröffentlichen**.

   ![](assets/publish-all-customizations1.png)

## Bevor Sie mit Schritt 3 fortfahren {#before-proceeding-to-step}

* Wenn Sie die Anzahl der zu synchronisierenden Datensätze einschränken möchten, [Einrichten eines benutzerdefinierten Synchronisierungsfilters](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/create-a-custom-dynamics-sync-filter.md) jetzt.
* Führen Sie die [Überprüfen der Synchronisierung mit Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md) -Prozess. Es wird überprüft, ob Ihre ersten Setups ordnungsgemäß durchgeführt wurden.
* Melden Sie sich beim Marketo Sync User in Microsoft Dynamics CRM an.

>[!MORELIKETHIS]
>
>[Installieren von Marketo für Microsoft Dynamics 2016/Dynamics 365 On-Premises Schritt 3 von 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-3-of-3-connect.md)
